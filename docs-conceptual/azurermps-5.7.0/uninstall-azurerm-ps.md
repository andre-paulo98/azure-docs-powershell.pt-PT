---
title: Desinstalar o Azure PowerShell
description: Como realizar uma desinstalação completa do Azure PowerShell
ms.date: 06/20/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 3828a6f9d60a68c2837cc201a50d8707324f4f0a
ms.sourcegitcommit: 06f9206e025afa7207d4657c8f57c94ddb74817a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/07/2018
ms.locfileid: "51211235"
---
# <a name="uninstall-the-azure-powershell-module"></a><span data-ttu-id="ddcfa-103">Desinstalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="ddcfa-103">Uninstall the Azure PowerShell module</span></span>

<span data-ttu-id="ddcfa-104">Este artigo explica como desinstalar uma versão mais antiga do Azure PowerShell ou removê-la completamente do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-104">This article tells you how to uninstall an older version of Azure PowerShell, or completely remove it from your system.</span></span> <span data-ttu-id="ddcfa-105">Se decidiu desinstalar completamente o Azure PowerShell, envie-nos os seus comentários através do cmdlet [Send-Feedback](/powershell/module/azurerm.profile/send-feedback).</span><span class="sxs-lookup"><span data-stu-id="ddcfa-105">If you've decided to completely uninstall the Azure PowerShell, please give us some feedback through the [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet.</span></span>
<span data-ttu-id="ddcfa-106">Se encontrou um erro, agradecemos-se que [registe um problema no GitHub](https://github.com/azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="ddcfa-106">If you encountered a bug, we'd appreciate it if you [file a GitHub issue](https://github.com/azure/azure-powershell/issues).</span></span>

## <a name="uninstall-msi-or-web-platform-installer"></a><span data-ttu-id="ddcfa-107">Desinstalar o MSI ou o Instalador da Plataforma Web</span><span class="sxs-lookup"><span data-stu-id="ddcfa-107">Uninstall MSI or Web Platform Installer</span></span>

<span data-ttu-id="ddcfa-108">Se instalou o Azure PowerShell com o pacote MSI ou o Instalador da Plataforma Web, deverá desinstalar o sistema do Windows, em vez do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-108">If you installed Azure PowerShell using the MSI package or the Web Platform Installer, you must uninstall through the Windows system rather than PowerShell.</span></span>

| <span data-ttu-id="ddcfa-109">Plataforma</span><span class="sxs-lookup"><span data-stu-id="ddcfa-109">Platform</span></span> | <span data-ttu-id="ddcfa-110">Instruções</span><span class="sxs-lookup"><span data-stu-id="ddcfa-110">Instructions</span></span> |
|----------|--------------|
| <span data-ttu-id="ddcfa-111">Windows 10</span><span class="sxs-lookup"><span data-stu-id="ddcfa-111">Windows 10</span></span> | <span data-ttu-id="ddcfa-112">Iniciar > Definições > Aplicações</span><span class="sxs-lookup"><span data-stu-id="ddcfa-112">Start > Settings > Apps</span></span> |
| <span data-ttu-id="ddcfa-113">Windows 7</span><span class="sxs-lookup"><span data-stu-id="ddcfa-113">Windows 7</span></span> </br><span data-ttu-id="ddcfa-114">Windows 8</span><span class="sxs-lookup"><span data-stu-id="ddcfa-114">Windows 8</span></span> | <span data-ttu-id="ddcfa-115">Iniciar > Painel de Controlo > Programas > Desinstalar um programa</span><span class="sxs-lookup"><span data-stu-id="ddcfa-115">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="ddcfa-116">Quando estiver neste ecrã, verá "Azure PowerShell" na lista de programas e poderá desinstalar a partir daí.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-116">Once on this screen you should see "Azure PowerShell" in the program listing, and can uninstall from there.</span></span>

## <a name="uninstall-from-powershell"></a><span data-ttu-id="ddcfa-117">Desinstalar a partir do PowerShell</span><span class="sxs-lookup"><span data-stu-id="ddcfa-117">Uninstall from PowerShell</span></span>

<span data-ttu-id="ddcfa-118">Se instalou o Azure PowerShell através do PowerShellGet, pode utilizar o cmdlet [Uninstall-Module](/powershell/module/powershellget/uninstall-module).</span><span class="sxs-lookup"><span data-stu-id="ddcfa-118">If you installed Azure PowerShell using PowerShellGet, you can use the [Uninstall-Module](/powershell/module/powershellget/uninstall-module) cmdlet.</span></span> <span data-ttu-id="ddcfa-119">No entanto, `Uninstall-Module` desinstala apenas um módulo.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-119">However, `Uninstall-Module` only uninstalls one module.</span></span> <span data-ttu-id="ddcfa-120">Para remover completamente o Azure PowerShell, tem de desinstalar cada módulo individualmente.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-120">To remove Azure PowerShell completely, you must uninstall each module individually.</span></span> <span data-ttu-id="ddcfa-121">A desinstalação pode ser complicada se tiver várias versões do Azure PowerShell instaladas.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-121">Uninstallation can be complicated if you have multiple versions of Azure PowerShell installed.</span></span>

<span data-ttu-id="ddcfa-122">O script a seguir pode servir para remover completamente uma versão única do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-122">You use the following script can be used to completely remove a single version of Azure PowerShell.</span></span> <span data-ttu-id="ddcfa-123">O script consulta a Galeria do PowerShell para obter uma lista dos submódulos pendentes.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-123">The script queries the PowerShell Gallery to get a list of dependent submodules.</span></span> <span data-ttu-id="ddcfa-124">Em seguida, o script desinstala a versão correta de cada submódulo.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-124">Then, the script uninstalls the correct version of each submodule.</span></span>

```powershell-interactive
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

<span data-ttu-id="ddcfa-125">Para utilizar esta função, copie e cole o código na sua sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-125">To use this function, copy and paste the code into your PowerShell session.</span></span> <span data-ttu-id="ddcfa-126">O exemplo a seguir mostra como executar a função para remover uma versão mais antiga do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-126">The following example shows how to run the function to remove an older version of Azure PowerShell.</span></span>

```powershell-interactive
Uninstall-AllModules -TargetModule AzureRM -Version 4.4.1 -Force
```

<span data-ttu-id="ddcfa-127">À medida que o script é executado, apresenta o nome e a versão de cada submódulo que está a ser desinstalado.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-127">As the script runs, it will display the name and version of each submodule that is being uninstalled.</span></span>

```output
Creating list of dependencies...
Uninstalling AzureRM.Profile version 3.4.1
Uninstalling Azure.Storage version 3.4.1
Uninstalling AzureRM.AnalysisServices version 0.4.7
Uninstalling Azure.AnalysisServices version 0.4.7
...
```

<span data-ttu-id="ddcfa-128">Execute este comando para cada versão do Azure PowerShell que deseja desinstalar.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-128">Run this command for every version of Azure PowerShell that you want to uninstall.</span></span>