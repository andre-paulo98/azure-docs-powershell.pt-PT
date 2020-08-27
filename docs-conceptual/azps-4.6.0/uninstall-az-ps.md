---
title: Desinstalar o Azure PowerShell
description: Como realizar uma desinstalação completa do Azure PowerShell
ms.date: 05/28/2020
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: d99b40121deca0a4817c3a6364ad55020dadbda1
ms.sourcegitcommit: b94a3f00c147144b0ef7f8cf8d0f151e04674b89
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/25/2020
ms.locfileid: "88821744"
---
# <a name="uninstall-the-azure-powershell-module"></a>Desinstalar o módulo do Azure PowerShell

Este artigo explica como desinstalar uma versão mais antiga do Azure PowerShell ou removê-la completamente do seu sistema. Se decidiu desinstalar completamente o Azure PowerShell, envie-nos os seus comentários através do cmdlet [Send-Feedback](/powershell/module/az.accounts/send-feedback). Se encontrou um erro, agradecemos-se que [registe um problema no GitHub](https://github.com/azure/azure-powershell/issues) para o podermos resolver.

## <a name="uninstall-the-az-powershell-module-from-msi"></a>Desinstalar o módulo do Az PowerShell a partir do MSI

Se instalou o módulo do Az PowerShell através do pacote de MSI, tem de fazer a desinstalação através do sistema Windows e não através do PowerShell.

|         Plataforma         |                      Instruções                      |
| ------------------------ | ------------------------------------------------------ |
| Windows 10               | Iniciar > Definições > Aplicações                                |
| Windows 7 </br>Windows 8 | Iniciar > Painel de Controlo > Programas > Desinstalar um programa |

Quando estiver neste ecrã, verá **Azure PowerShell** na lista de programas. Esta é a aplicação a desinstalar. Se não vir este programa na lista, instalou através de PowerShellGet e deve seguir o conjunto seguinte de instruções.

## <a name="uninstall-the-az-powershell-module-from-powershellget"></a>Desinstalar o módulo do Az PowerShell a partir do PowerShellGet

Para desinstalar os módulos do Az, pode utilizar o cmdlet [Uninstall-Module](/powershell/module/powershellget/uninstall-module). No entanto, `Uninstall-Module` desinstala apenas um módulo. Para remover completamente o módulo do Az PowerShell, tem de desinstalar cada módulo individualmente. A desinstalação pode ser complicada se tiver mais de uma versão do Azure PowerShell instalada.

Para ver que versões do módulo do Az PowerShell instalou, execute o seguinte comando:

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions
```

```output
Version             Name                           Repository           Description
-------             ----                           ----------           -----------
3.8.0               Az                             PSGallery            Microsoft Azure PowerShell
4.1.0               Az                             PSGallery            Microsoft Azure PowerShell
```

<a name="uninstall-script"/>

O script seguinte consulta a Galeria do PowerShell para obter uma lista dos submódulos dependentes. Em seguida, o script desinstala a versão correta de cada submódulo. Precisa de ter acesso de administrador para executar este script num âmbito diferente de **Processo** ou **Utilizador Atual**.

```powershell-interactive
function Uninstall-AzModule {
  [CmdletBinding(SupportsShouldProcess)]
  param(
    [ValidateNotNullOrEmpty()]
    [ValidateSet('Az','AzureRM','Azure')]
    [string]$Name = 'Az',

    [Parameter(Mandatory)]
    [string]$Version,

    [switch]$AllowPrerelease
  )

  $Params = @{}

  if ($PSBoundParameters.AllowPrerelease) {
    $Params.AllowPrerelease = $true
  }

  $IsAdmin = ([Security.Principal.WindowsPrincipal] [Security.Principal.WindowsIdentity]::GetCurrent()).IsInRole([Security.Principal.WindowsBuiltInRole] 'Administrator')

  if (-not(Get-InstalledModule -Name $Name -RequiredVersion $Version -ErrorAction SilentlyContinue -OutVariable RootModule @Params)) {

    Write-Warning -Message "Uninstall aborted. $Name version $Version not found."

  } elseif (($RootModule.InstalledLocation -notlike "*$env:USERPROFILE*") -and ($IsAdmin -eq $false)) {

    Write-Warning -Message "Uninstall aborted. $Name version $Version exists in a system path. PowerShell must be run elevated as an admin to remove it."

  } elseif ((Get-Process -Name powershell, pwsh -OutVariable Sessions -ErrorAction SilentlyContinue).Count -gt 1) {

    Write-Warning -Message "Uninstall aborted. Please close all other PowerShell sessions before continuing. There are currently $($Sessions.Count) PowerShell sessions running."

  } else {
    Write-Verbose -Message 'Creating list of dependencies...'
    $target = Find-Module -Name $Name -RequiredVersion $Version @Params

    $AllModules = @([pscustomobject]@{
      Name = $Name
      Version = $Version
    })

    $AllModules += foreach ($dependency in $target.Dependencies) {
      switch ($dependency.keys) {
        {$_ -contains 'RequiredVersion'} {$UninstallVersion = $dependency.RequiredVersion; break}
        {$_ -contains 'MinimumVersion'} {$UninstallVersion = $dependency.MinimumVersion; break}
      }

      [pscustomobject]@{
        Name = $dependency.Name
        Version = $UninstallVersion
      }
    }

    [int]$i = 100 / $AllModules.Count

    foreach ($module in $AllModules) {
      Write-Progress -Activity 'Uninstallation in Progress' -Status "$i% Complete:" -PercentComplete $i
      $i++

      if (Get-InstalledModule -Name $module.Name -RequiredVersion $module.Version -ErrorAction SilentlyContinue @Params) {
        Write-Verbose -Message "Uninstalling $($module.Name) version $($module.Version)"

        Remove-Module -FullyQualifiedName @{ModuleName=$module.Name;ModuleVersion=$module.Version} -ErrorAction SilentlyContinue

        try {
          if ($PSCmdlet.ShouldProcess("$($module.Name) version $($module.Version)")) {
            Uninstall-Module -Name $module.Name -RequiredVersion $module.Version -Force -ErrorAction Stop @Params
          }
          $State = 'Uninstalled'
        } Catch {
          $State = 'Manual uninstall required'
          Write-Verbose -Message "$($module.Name) version: $($module.Version) may require manual uninstallation."
        }

      } else {
        $State = 'Not found'
        Write-Verbose -Message "$($module.Name) version: $($module.Version) not found."
      }

      if (-not $PSBoundParameters.WhatIf) {
        [pscustomobject]@{
          ModuleName = $module.Name
          Version = $module.Version
          State = $State
        }
      }

    }
  }
}
```

Para utilizar esta função, copie e cole o código na sua sessão do PowerShell. O exemplo seguinte mostra como executar a função para remover uma versão mais antiga do módulo do Az PowerShell e os respetivos submódulos.

```powershell-interactive
Uninstall-AzModule -Name Az -Version 1.8.0
```

À medida que o script é executado, apresenta o **Nome**, **Versão** e **Estado** de cada submódulo que está a ser desinstalado. Para executar o script de forma a apenas ver o que seria eliminado, sem o remover, especifique o parâmetro `-WhatIf`.

```output
ModuleName              Version  State
----------              -------  -----
Az.Accounts             1.5.1    Not found
Az.Aks                  1.0.1    Uninstalled
Az.AnalysisServices     1.1.0    Uninstalled
Az.ApiManagement        1.0.0    Uninstalled
Az.ApplicationInsights  1.0.0    Uninstalled
...
```

> [!IMPORTANT]
> Se não puder corresponder este script a uma dependência exata com a mesma versão para desinstalar, não irá desinstalar _nenhuma_ versão dessa dependência. Tal acontece porque podem existir outras versões do módulo de destino no seu sistema que dependem destas dependências.

Execute o exemplo seguinte para cada versão do módulo do Az PowerShell que queira desinstalar.
Para sua comodidade, o script que se segue desinstala todas as versões do Az, **exceto** a mais recente.

```powershell-interactive
$Modules = Get-InstalledModule -Name Az -AllVersions |
    Sort-Object -Property Version -Descending |
        Select-Object -Skip 1
$Modules | ForEach-Object {Uninstall-AzModule -Name $_.Name -Version $_.Version}
```

## <a name="uninstall-the-azurerm-module"></a>Desinstalar o módulo do AzureRM

Se tiver o módulo do Az instalado no seu sistema e quiser desinstalar o AzureRM, existem duas opções. O método utilizado depende da forma como instalou o módulo AzureRM. Se não tiver a certeza do método de instalação original, siga os passos para primeiro desinstalar um MSI.

### <a name="uninstall-the-azurerm-powershell-module-from-msi"></a>Desinstalar o módulo do AzureRM PowerShell a partir do MSI

Se instalou o módulo do AzureRM PowerShell através do pacote de MSI, tem de fazer a desinstalação através do sistema Windows e não através do PowerShell.

|         Plataforma         |                      Instruções                      |
| ------------------------ | ------------------------------------------------------ |
| Windows 10               | Iniciar > Definições > Aplicações                                |
| Windows 7 </br>Windows 8 | Iniciar > Painel de Controlo > Programas > Desinstalar um programa |

Quando estiver neste ecrã, verá **Azure PowerShell** ou **Microsoft Azure PowerShell - Month Year** na lista de programas. Esta é a aplicação a desinstalar. Se não vir este programa na lista, instalou através de PowerShellGet e deve seguir o conjunto seguinte de instruções.

### <a name="uninstall-the-azurerm-powershell-module-from-powershellget"></a>Desinstalar o módulo do AzureRM PowerShell a partir do PowerShellGet

Se instalou o AzureRM com o PowerShellGet, pode remover os módulos com o cmdlet [Uninstall-AzureRM](/powershell/module/az.accounts/uninstall-azurerm), disponível como parte do módulo `Az.Accounts`. O exemplo seguinte remove _todos_ os módulos do AzureRM do seu computador. Requer privilégios de administrador.

```powershell-interactive
Uninstall-AzureRm
```
