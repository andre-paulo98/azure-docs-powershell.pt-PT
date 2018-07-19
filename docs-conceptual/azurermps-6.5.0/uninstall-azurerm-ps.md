---
title: Desinstalar o Azure PowerShell
description: Como realizar uma desinstalação completa do Azure PowerShell
ms.date: 06/20/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 92af0fdd8db451e2f0f092d66a3e296ad8d6a09e
ms.sourcegitcommit: 8b882d1c27d9e323447ff85f56d11bbf5e244d7f
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/18/2018
ms.locfileid: "39110352"
---
# <a name="uninstall-the-azure-powershell-module"></a><span data-ttu-id="fea8f-103">Desinstalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="fea8f-103">Uninstall the Azure PowerShell module</span></span>

<span data-ttu-id="fea8f-104">Este artigo explica como desinstalar uma versão mais antiga do Azure PowerShell ou removê-la completamente do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="fea8f-104">This article tells you how to uninstall an older version of Azure PowerShell, or completely remove it from your system.</span></span> <span data-ttu-id="fea8f-105">Se decidiu desinstalar completamente o Azure PowerShell, envie-nos os seus comentários através do cmdlet [Send-Feedback](/powershell/module/azurerm.profile/send-feedback).</span><span class="sxs-lookup"><span data-stu-id="fea8f-105">If you've decided to completely uninstall the Azure PowerShell, please give us some feedback through the [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet.</span></span>
<span data-ttu-id="fea8f-106">Se encontrou um erro, agradecemos-se que [registe um problema no GitHub](https://github.com/azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="fea8f-106">If you encountered a bug, we'd appreciate it if you [file a GitHub issue](https://github.com/azure/azure-powershell/issues).</span></span>

## <a name="uninstall-msi"></a><span data-ttu-id="fea8f-107">Desinstalar o MSI</span><span class="sxs-lookup"><span data-stu-id="fea8f-107">Uninstall MSI</span></span>

<span data-ttu-id="fea8f-108">Se instalou o Azure PowerShell através do pacote de MSI, a desinstalação deve ser feita através do sistema do Windows, e não através do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fea8f-108">If you installed Azure PowerShell using the MSI package, you must uninstall through the Windows system rather than PowerShell.</span></span>

| <span data-ttu-id="fea8f-109">Plataforma</span><span class="sxs-lookup"><span data-stu-id="fea8f-109">Platform</span></span> | <span data-ttu-id="fea8f-110">Instruções</span><span class="sxs-lookup"><span data-stu-id="fea8f-110">Instructions</span></span> |
|----------|--------------|
| <span data-ttu-id="fea8f-111">Windows 10</span><span class="sxs-lookup"><span data-stu-id="fea8f-111">Windows 10</span></span> | <span data-ttu-id="fea8f-112">Iniciar > Definições > Aplicações</span><span class="sxs-lookup"><span data-stu-id="fea8f-112">Start > Settings > Apps</span></span> |
| <span data-ttu-id="fea8f-113">Windows 7</span><span class="sxs-lookup"><span data-stu-id="fea8f-113">Windows 7</span></span> </br><span data-ttu-id="fea8f-114">Windows 8</span><span class="sxs-lookup"><span data-stu-id="fea8f-114">Windows 8</span></span> | <span data-ttu-id="fea8f-115">Iniciar > Painel de Controlo > Programas > Desinstalar um programa</span><span class="sxs-lookup"><span data-stu-id="fea8f-115">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="fea8f-116">Quando estiver neste ecrã, verá "Azure PowerShell" na lista de programas e poderá desinstalar a partir daí.</span><span class="sxs-lookup"><span data-stu-id="fea8f-116">Once on this screen you should see "Azure PowerShell" in the program listing, and can uninstall from there.</span></span>

## <a name="uninstall-from-powershell"></a><span data-ttu-id="fea8f-117">Desinstalar a partir do PowerShell</span><span class="sxs-lookup"><span data-stu-id="fea8f-117">Uninstall from PowerShell</span></span>

<span data-ttu-id="fea8f-118">Se instalou o Azure PowerShell através do PowerShellGet, pode utilizar o cmdlet [Uninstall-Module](/powershell/module/powershellget/uninstall-module).</span><span class="sxs-lookup"><span data-stu-id="fea8f-118">If you installed Azure PowerShell using PowerShellGet, you can use the [Uninstall-Module](/powershell/module/powershellget/uninstall-module) cmdlet.</span></span> <span data-ttu-id="fea8f-119">No entanto, `Uninstall-Module` desinstala apenas um módulo.</span><span class="sxs-lookup"><span data-stu-id="fea8f-119">However, `Uninstall-Module` only uninstalls one module.</span></span> <span data-ttu-id="fea8f-120">Para remover completamente o Azure PowerShell, tem de desinstalar cada módulo individualmente.</span><span class="sxs-lookup"><span data-stu-id="fea8f-120">To remove Azure PowerShell completely, you must uninstall each module individually.</span></span> <span data-ttu-id="fea8f-121">A desinstalação pode ser complicada se tiver várias versões do Azure PowerShell instaladas.</span><span class="sxs-lookup"><span data-stu-id="fea8f-121">Uninstallation can be complicated if you have multiple versions of Azure PowerShell installed.</span></span>

<span data-ttu-id="fea8f-122">O script a seguir pode ser utilizado para remover completamente uma versão única do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fea8f-122">The following script can be used to completely remove a single version of Azure PowerShell.</span></span> <span data-ttu-id="fea8f-123">O script consulta a Galeria do PowerShell para obter uma lista dos submódulos dependentes.</span><span class="sxs-lookup"><span data-stu-id="fea8f-123">The script queries the PowerShell Gallery to get a list of dependent submodules.</span></span> <span data-ttu-id="fea8f-124">Em seguida, o script desinstala a versão correta de cada submódulo.</span><span class="sxs-lookup"><span data-stu-id="fea8f-124">Then, the script uninstalls the correct version of each submodule.</span></span>

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

<span data-ttu-id="fea8f-125">Para utilizar esta função, copie e cole o código na sua sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fea8f-125">To use this function, copy and paste the code into your PowerShell session.</span></span> <span data-ttu-id="fea8f-126">O exemplo a seguir mostra como executar a função para remover uma versão mais antiga do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fea8f-126">The following example shows how to run the function to remove an older version of Azure PowerShell.</span></span>

```powershell
Uninstall-AllModules -TargetModule AzureRM -Version 4.4.1 -Force
```

<span data-ttu-id="fea8f-127">À medida que o script é executado, apresenta o nome e a versão de cada submódulo que está a ser desinstalado.</span><span class="sxs-lookup"><span data-stu-id="fea8f-127">As the script runs, it will display the name and version of each submodule that is being uninstalled.</span></span>

```output
Creating list of dependencies...
Uninstalling AzureRM.Profile version 3.4.1
Uninstalling Azure.Storage version 3.4.1
Uninstalling AzureRM.AnalysisServices version 0.4.7
Uninstalling Azure.AnalysisServices version 0.4.7
...
```

<span data-ttu-id="fea8f-128">Execute este comando para cada versão do Azure PowerShell que deseja desinstalar.</span><span class="sxs-lookup"><span data-stu-id="fea8f-128">Run this command for every version of Azure PowerShell that you want to uninstall.</span></span>
