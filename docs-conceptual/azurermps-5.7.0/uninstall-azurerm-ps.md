---
title: Desinstalar o Azure PowerShell
description: Como realizar uma desinstalação completa do Azure PowerShell
ms.date: 06/20/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 052a150afa6cd90ca5babdce2aa7e3b4ff0b893b
ms.sourcegitcommit: 4c775721461210431bd913f28d1f1e6f1976880a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/28/2018
ms.locfileid: "37091654"
---
# <a name="uninstall-the-azure-powershell-module"></a>Desinstalar o módulo do Azure PowerShell

Este artigo explica como desinstalar uma versão mais antiga do Azure PowerShell ou removê-la completamente do seu sistema. Se decidiu desinstalar completamente o Azure PowerShell, dê-nos algum feedback através do cmdlet [Send-Feedback](/powershell/module/azurerm.profile/send-feedback). Se encontrou um erro, agradecemos-se que [registe um problema no GitHub](https://github.com/azure/azure-powershell/issues).

# <a name="uninstall-msi-or-web-platform-installer"></a>Desinstalar o MSI ou o Instalador da Plataforma Web 

Se instalou o Azure PowerShell com o pacote MSI ou o Instalador da Plataforma Web, deverá desinstalar o sistema do Windows, em vez do PowerShell.
 
| Plataforma | Instruções |
|----------|--------------|
| Windows 10 | Iniciar > Definições > Aplicações |
| Windows 7 </br>Windows 8 | Iniciar > Painel de Controlo > Programas > Desinstalar um programa |

Quando estiver no ecrã, verá "Azure PowerShell" na lista de programas e poderá desinstalar a partir daí.

# <a name="uninstall-from-powershell"></a>Desinstalar do PowerShell

Se instalou o Azure PowerShell com o PowerShellGet, pode utilizar o cmdlet [Uninstall-Module](/powershell/module/powershellget/uninstall-module). No entanto, `Uninstall-Module` desinstala apenas um módulo. Para retirar o Azure PowerShell completamente, tem de desinstalar cada módulo individualmente. A desinstalação pode ser complicada se tiver várias versões do Azure PowerShell instaladas.

O script a seguir pode servir para remover completamente uma versão única do Azure PowerShell. O script consulta a Galeria do PowerShell para obter uma lista dos submódulos pendentes. Em seguida, o script desinstala a versão correta de cada submódulo.

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

À medida que o script é executado, apresenta o nome e a versão de cada submódulo que é desinstalado.

```output
Creating list of dependencies...
Uninstalling AzureRM.Profile version 3.4.1
Uninstalling Azure.Storage version 3.4.1
Uninstalling AzureRM.AnalysisServices version 0.4.7
Uninstalling Azure.AnalysisServices version 0.4.7
...
```

Execute este comando para cada versão do Azure PowerShell que deseja desinstalar.