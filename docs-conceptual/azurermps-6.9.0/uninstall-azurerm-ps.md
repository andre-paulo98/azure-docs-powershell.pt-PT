---
title: Desinstalar o Azure PowerShell
description: Como realizar uma desinstalação completa do Azure PowerShell
ms.date: 09/11/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 385dd0281185cfb9e7bdd2c98e4c557659fff384
ms.sourcegitcommit: 19dffee617477001f98d43e39a50ce1fad087b74
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2018
ms.locfileid: "47179229"
---
# <a name="uninstall-the-azure-powershell-module"></a>Desinstalar o módulo do Azure PowerShell

Este artigo explica como desinstalar uma versão mais antiga do Azure PowerShell ou removê-la completamente do seu sistema. Se decidiu desinstalar completamente o Azure PowerShell, envie-nos os seus comentários através do cmdlet [Send-Feedback](/powershell/module/azurerm.profile/send-feedback).
Se encontrou um erro, agradecemos-se que [registe um problema no GitHub](https://github.com/azure/azure-powershell/issues).

## <a name="uninstall-msi"></a>Desinstalar o MSI

Se instalou o Azure PowerShell através do pacote de MSI, a desinstalação deve ser feita através do sistema do Windows, e não através do PowerShell.

| Plataforma | Instruções |
|----------|--------------|
| Windows 10 | Iniciar > Definições > Aplicações |
| Windows 7 </br>Windows 8 | Iniciar > Painel de Controlo > Programas > Desinstalar um programa |

Quando estiver neste ecrã, verá "Azure PowerShell" na lista de programas e poderá desinstalar a partir daí.

## <a name="uninstall-from-powershell"></a>Desinstalar a partir do PowerShell

Se instalou o Azure PowerShell através do PowerShellGet, pode utilizar o cmdlet [Uninstall-Module](/powershell/module/powershellget/uninstall-module). No entanto, `Uninstall-Module` desinstala apenas um módulo. Para remover completamente o Azure PowerShell, tem de desinstalar cada módulo individualmente. A desinstalação pode ser complicada se tiver mais de uma versão do Azure PowerShell instalada.

O script seguinte consulta a Galeria do PowerShell para obter uma lista dos submódulos dependentes. Em seguida, o script desinstala a versão correta de cada submódulo.

```powershell
function Uninstall-AllModules {
  param(
    [Parameter(Mandatory=$true)]
    [string]$TargetModule,

    [Parameter(Mandatory=$true)]
    [string]$Version,

    [switch]$Force
  )

  $AllModules = @()

  'Creating list of dependencies...'
  $target = Find-Module $TargetModule -RequiredVersion $version
  $target.Dependencies | ForEach-Object {
    $AllModules += New-Object -TypeName psobject -Property @{name=$_.name; version=$_.requiredversion}
  }
  $AllModules += New-Object -TypeName psobject -Property @{name=$TargetModule; version=$Version}

  foreach ($module in $AllModules) {
    Write-Host ('Uninstalling {0} version {1}' -f $module.name,$module.version)
    try {
      Uninstall-Module -Name $module.name -RequiredVersion $module.version -Force:$Force -ErrorAction Stop
    } catch {
      Write-Host ("`t" + $_.Exception.Message)
    }
  }
}
```

Para utilizar esta função, copie e cole o código na sua sessão do PowerShell. O exemplo a seguir mostra como executar a função para remover uma versão mais antiga do Azure PowerShell.

```powershell
Uninstall-AllModules -TargetModule AzureRM -Version 4.4.1 -Force
```

À medida que o script é executado, apresenta o nome e a versão de cada submódulo que está a ser desinstalado.

```output
Creating list of dependencies...
Uninstalling AzureRM.Profile version 3.4.1
Uninstalling Azure.Storage version 3.4.1
Uninstalling AzureRM.AnalysisServices version 0.4.7
Uninstalling Azure.AnalysisServices version 0.4.7
...
```

Execute este comando para cada versão do Azure PowerShell que deseja desinstalar.
