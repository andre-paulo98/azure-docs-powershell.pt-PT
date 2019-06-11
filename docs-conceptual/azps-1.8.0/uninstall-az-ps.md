---
title: Desinstalar o Azure PowerShell
description: Como realizar uma desinstalação completa do Azure PowerShell
ms.date: 05/10/2019
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: eaabd8014368f7ea8f4c9504e58d920dad8a6518
ms.sourcegitcommit: 020c69430358b13cbd99fedd5d56607c9b10047b
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/29/2019
ms.locfileid: "66365443"
---
# <a name="uninstall-the-azure-powershell-module"></a>Desinstalar o módulo do Azure PowerShell

Este artigo explica como desinstalar uma versão mais antiga do Azure PowerShell ou removê-la completamente do seu sistema. Se decidiu desinstalar completamente o Azure PowerShell, envie-nos os seus comentários através do cmdlet [Send-Feedback](/powershell/module/az.accounts/send-feedback).
Se encontrou um erro, agradecemos-se que [registe um problema no GitHub](https://github.com/azure/azure-powershell/issues) para o podermos resolver.

## <a name="uninstall-the-az-module"></a>Desinstalar o módulo do Az

Para desinstalar os módulos do Az, utilize o cmdlet [Uninstall-Module](/powershell/module/powershellget/uninstall-module). No entanto, `Uninstall-Module` desinstala apenas um módulo. Para remover completamente o Azure PowerShell, tem de desinstalar cada módulo individualmente. A desinstalação pode ser complicada se tiver mais de uma versão do Azure PowerShell instalada.

Para ver que versões do Azure PowerShell tem atualmente instaladas, execute o seguinte comando:

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions
```

```output
Version             Name                           Repository           Description
-------             ----                           ----------           -----------
0.7.0               Az                             PSGallery            Azure Resource Manager Module
1.0.0               Az                             PSGallery            Azure Resource Manager Module
```

<a name="uninstall-script"/>

O script seguinte consulta a Galeria do PowerShell para obter uma lista dos submódulos dependentes. Em seguida, o script desinstala a versão correta de cada submódulo. Precisa de ter acesso de administrador para executar este script num âmbito diferente de `Process` ou `CurrentUser`.

```powershell-interactive
function Uninstall-AllModules {
  param(
    [Parameter(Mandatory=$true)]
    [string]$TargetModule,

    [Parameter(Mandatory=$true)]
    [string]$Version,

    [switch]$Force,

    [switch]$WhatIf
  )
  
  $AllModules = @()
  
  'Creating list of dependencies...'
  $target = Find-Module $TargetModule -RequiredVersion $version
  $target.Dependencies | ForEach-Object {
    if ($_.requiredVersion) {
      $AllModules += New-Object -TypeName psobject -Property @{name=$_.name; version=$_.requiredVersion}
    }
    else { # Assume minimum version
      # Minimum version actually reports the installed dependency
      # which is used, not the actual "minimum dependency." Check to
      # see if the requested version was installed as a dependency earlier.
      $candidate = Get-InstalledModule $_.name -RequiredVersion $version
      if ($candidate) {
        $AllModules += New-Object -TypeName psobject -Property @{name=$_.name; version=$version}
      }
      else {
        Write-Warning ("Could not find uninstall candidate for {0}:{1} - module may require manual uninstall" -f $_.name,$version)
      }
    }
  }
  $AllModules += New-Object -TypeName psobject -Property @{name=$TargetModule; version=$Version}

  foreach ($module in $AllModules) {
    Write-Host ('Uninstalling {0} version {1}...' -f $module.name,$module.version)
    try {
      Uninstall-Module -Name $module.name -RequiredVersion $module.version -Force:$Force -ErrorAction Stop -WhatIf:$WhatIf
    } catch {
      Write-Host ("`t" + $_.Exception.Message)
    }
  }
}
```

Para utilizar esta função, copie e cole o código na sua sessão do PowerShell. O exemplo a seguir mostra como executar a função para remover uma versão mais antiga do Azure PowerShell.

```powershell-interactive
Uninstall-AllModules -TargetModule Az -Version 0.7.0 -Force
```

À medida que o script é executado, apresenta o nome e a versão de cada submódulo que está a ser desinstalado. Para executar o script para apenas ver o que seria eliminar, sem o remover, utilize a opção `-WhatIf`.

```output
Creating list of dependencies...
Uninstalling Az.Profile version 0.7.0
Uninstalling Az.Aks version 0.7.0
Uninstalling Az.AnalysisServices version 0.7.0
...
```

Execute este comando para cada versão do Azure PowerShell que deseja desinstalar. Para sua comodidade, o script que se segue desinstala todas as versões do Az __exceto__ a mais recente.

```powershell-interactive
$versions = (Get-InstalledModule Az -AllVersions | Select-Object Version)
$versions[1..($versions.Length-1)]  | foreach { Uninstall-AllModules -TargetModule Az -Version ($_.Version) -Force }
```

## <a name="uninstall-the-azurerm-module"></a>Desinstalar o módulo do AzureRM

Se tiver o módulo do Az instalado no seu sistema e quiser desinstalar o AzureRM, existem duas opções que não implicam a execução do script `Uninstall-AllModules` acima. O método utilizado depende da forma como instalou o módulo AzureRM.
Se não tiver a certeza do método de instalação original, siga os passos para primeiro desinstalar um MSI.

### <a name="uninstall-azure-powershell-msi"></a>Desinstalar o MSI do Azure PowerShell

Se instalou os módulos do AzureRM do Azure PowerShell através do pacote de MSI, a desinstalação deve ser feita através do sistema do Windows, e não através do PowerShell.

| Plataforma | Instruções |
|----------|--------------|
| Windows 10 | Iniciar > Definições > Aplicações |
| Windows 7 </br>Windows 8 | Iniciar > Painel de Controlo > Programas > Desinstalar um programa |

Quando estiver neste ecrã, verá __Azure PowerShell__ na lista de programas. Esta é a aplicação a desinstalar. Se não vir este programa na lista, instalou através de PowerShellGet e deve seguir o conjunto seguinte de instruções.

### <a name="uninstall-from-powershell"></a>Desinstalar a partir do PowerShell

Se instalou o AzureRM com o PowerShellGet, pode remover os módulos com o comando [Uninstall-AzureRM](/powershell/module/az.accounts/uninstall-azurerm), disponível como parte do módulo `Az.Accounts`. Esta ação remove _todos_ os módulos do AzureRM do seu computador, mas precisa de ter privilégios de administrador.

```powershell-interactive
Uninstall-AzureRm
```

Se não conseguir executar o comando `Uninstall-AzureRM` com êxito, utilize o [script `Uninstall-AllModules`](#uninstall-script) fornecido neste artigo com a seguinte invocação:

```powershell-interactive
$versions = (Get-InstalledModule AzureRM -AllVersions | Select-Object Version)
$versions | foreach { Uninstall-AllModules -TargetModule AzureRM -Version ($_.Version) -Force }
```