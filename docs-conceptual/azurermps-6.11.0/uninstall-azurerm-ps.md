---
title: Desinstalar o Azure PowerShell
description: Como realizar uma desinstalação completa do Azure PowerShell
ms.date: 09/11/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: bc017c40f955f2f4d99000bcde047d54eb3e155f
ms.sourcegitcommit: 5f946a535eccca0b3ddf3db8f617b32564a88938
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/25/2018
ms.locfileid: "50001410"
---
# <a name="uninstall-the-azure-powershell-module"></a><span data-ttu-id="c2f9b-103">Desinstalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c2f9b-103">Uninstall the Azure PowerShell module</span></span>

<span data-ttu-id="c2f9b-104">Este artigo explica como desinstalar uma versão mais antiga do Azure PowerShell ou removê-la completamente do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="c2f9b-104">This article tells you how to uninstall an older version of Azure PowerShell, or completely remove it from your system.</span></span> <span data-ttu-id="c2f9b-105">Se decidiu desinstalar completamente o Azure PowerShell, envie-nos os seus comentários através do cmdlet [Send-Feedback](/powershell/module/azurerm.profile/send-feedback).</span><span class="sxs-lookup"><span data-stu-id="c2f9b-105">If you've decided to completely uninstall the Azure PowerShell, give us some feedback through the [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet.</span></span>
<span data-ttu-id="c2f9b-106">Se encontrou um erro, agradecemos-se que [registe um problema no GitHub](https://github.com/azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="c2f9b-106">If you encountered a bug, we'd appreciate it if you [file a GitHub issue](https://github.com/azure/azure-powershell/issues).</span></span>

## <a name="uninstall-msi"></a><span data-ttu-id="c2f9b-107">Desinstalar o MSI</span><span class="sxs-lookup"><span data-stu-id="c2f9b-107">Uninstall MSI</span></span>

<span data-ttu-id="c2f9b-108">Se instalou o Azure PowerShell através do pacote de MSI, a desinstalação deve ser feita através do sistema do Windows, e não através do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c2f9b-108">If you installed Azure PowerShell using the MSI package, you must uninstall through the Windows system rather than PowerShell.</span></span>

| <span data-ttu-id="c2f9b-109">Plataforma</span><span class="sxs-lookup"><span data-stu-id="c2f9b-109">Platform</span></span> | <span data-ttu-id="c2f9b-110">Instruções</span><span class="sxs-lookup"><span data-stu-id="c2f9b-110">Instructions</span></span> |
|----------|--------------|
| <span data-ttu-id="c2f9b-111">Windows 10</span><span class="sxs-lookup"><span data-stu-id="c2f9b-111">Windows 10</span></span> | <span data-ttu-id="c2f9b-112">Iniciar > Definições > Aplicações</span><span class="sxs-lookup"><span data-stu-id="c2f9b-112">Start > Settings > Apps</span></span> |
| <span data-ttu-id="c2f9b-113">Windows 7</span><span class="sxs-lookup"><span data-stu-id="c2f9b-113">Windows 7</span></span> </br><span data-ttu-id="c2f9b-114">Windows 8</span><span class="sxs-lookup"><span data-stu-id="c2f9b-114">Windows 8</span></span> | <span data-ttu-id="c2f9b-115">Iniciar > Painel de Controlo > Programas > Desinstalar um programa</span><span class="sxs-lookup"><span data-stu-id="c2f9b-115">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="c2f9b-116">Quando estiver neste ecrã, verá "Azure PowerShell" na lista de programas e poderá desinstalar a partir daí.</span><span class="sxs-lookup"><span data-stu-id="c2f9b-116">Once on this screen you should see "Azure PowerShell" in the program listing, and can uninstall from there.</span></span>

## <a name="uninstall-from-powershell"></a><span data-ttu-id="c2f9b-117">Desinstalar a partir do PowerShell</span><span class="sxs-lookup"><span data-stu-id="c2f9b-117">Uninstall from PowerShell</span></span>

<span data-ttu-id="c2f9b-118">Se instalou o Azure PowerShell através do PowerShellGet, pode utilizar o cmdlet [Uninstall-Module](/powershell/module/powershellget/uninstall-module).</span><span class="sxs-lookup"><span data-stu-id="c2f9b-118">If you installed Azure PowerShell using PowerShellGet, you can use the [Uninstall-Module](/powershell/module/powershellget/uninstall-module) cmdlet.</span></span> <span data-ttu-id="c2f9b-119">No entanto, `Uninstall-Module` desinstala apenas um módulo.</span><span class="sxs-lookup"><span data-stu-id="c2f9b-119">However, `Uninstall-Module` only uninstalls one module.</span></span> <span data-ttu-id="c2f9b-120">Para remover completamente o Azure PowerShell, tem de desinstalar cada módulo individualmente.</span><span class="sxs-lookup"><span data-stu-id="c2f9b-120">To remove Azure PowerShell completely, you must uninstall each module individually.</span></span> <span data-ttu-id="c2f9b-121">A desinstalação pode ser complicada se tiver mais de uma versão do Azure PowerShell instalada.</span><span class="sxs-lookup"><span data-stu-id="c2f9b-121">Uninstallation can be complicated if you have more than one version of Azure PowerShell installed.</span></span>

<span data-ttu-id="c2f9b-122">O script seguinte consulta a Galeria do PowerShell para obter uma lista dos submódulos dependentes.</span><span class="sxs-lookup"><span data-stu-id="c2f9b-122">The following script queries the PowerShell Gallery to get a list of dependent submodules.</span></span> <span data-ttu-id="c2f9b-123">Em seguida, o script desinstala a versão correta de cada submódulo.</span><span class="sxs-lookup"><span data-stu-id="c2f9b-123">Then, the script uninstalls the correct version of each submodule.</span></span>

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

<span data-ttu-id="c2f9b-124">Para utilizar esta função, copie e cole o código na sua sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c2f9b-124">To use this function, copy and paste the code into your PowerShell session.</span></span> <span data-ttu-id="c2f9b-125">O exemplo a seguir mostra como executar a função para remover uma versão mais antiga do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c2f9b-125">The following example shows how to run the function to remove an older version of Azure PowerShell.</span></span>

```powershell
Uninstall-AllModules -TargetModule AzureRM -Version 4.4.1 -Force
```

<span data-ttu-id="c2f9b-126">À medida que o script é executado, apresenta o nome e a versão de cada submódulo que está a ser desinstalado.</span><span class="sxs-lookup"><span data-stu-id="c2f9b-126">As the script runs, it will display the name and version of each submodule that is being uninstalled.</span></span>

```output
Creating list of dependencies...
Uninstalling AzureRM.Profile version 3.4.1
Uninstalling Azure.Storage version 3.4.1
Uninstalling AzureRM.AnalysisServices version 0.4.7
Uninstalling Azure.AnalysisServices version 0.4.7
...
```

<span data-ttu-id="c2f9b-127">Execute este comando para cada versão do Azure PowerShell que deseja desinstalar.</span><span class="sxs-lookup"><span data-stu-id="c2f9b-127">Run this command for every version of Azure PowerShell that you want to uninstall.</span></span>
