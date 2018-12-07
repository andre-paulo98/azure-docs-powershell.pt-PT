---
title: Desinstalar o Azure PowerShell
description: Como realizar uma desinstalação completa do Azure PowerShell
ms.date: 11/30/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: a35814f4411dd9cab75fa36bd13ff087cdec8f9b
ms.sourcegitcommit: 93f93b90ef88c2659be95f3acaba514fe9639169
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/05/2018
ms.locfileid: "52826702"
---
# <a name="uninstall-the-azure-powershell-module"></a><span data-ttu-id="2dbd7-103">Desinstalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="2dbd7-103">Uninstall the Azure PowerShell module</span></span>

<span data-ttu-id="2dbd7-104">Este artigo explica como desinstalar uma versão mais antiga do Azure PowerShell ou removê-la completamente do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="2dbd7-104">This article tells you how to uninstall an older version of Azure PowerShell, or completely remove it from your system.</span></span> <span data-ttu-id="2dbd7-105">Se decidiu desinstalar completamente o Azure PowerShell, envie-nos os seus comentários através do cmdlet [Send-Feedback](/powershell/module/azurerm.profile/send-feedback).</span><span class="sxs-lookup"><span data-stu-id="2dbd7-105">If you've decided to completely uninstall the Azure PowerShell, give us some feedback through the [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet.</span></span>
<span data-ttu-id="2dbd7-106">Se encontrar um erro, agradecemos-se que [registe um problema no GitHub](https://github.com/azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="2dbd7-106">If you encounter a bug, we'd appreciate it if you [file a GitHub issue](https://github.com/azure/azure-powershell/issues).</span></span>

## <a name="uninstall-from-powershell"></a><span data-ttu-id="2dbd7-107">Desinstalar a partir do PowerShell</span><span class="sxs-lookup"><span data-stu-id="2dbd7-107">Uninstall from PowerShell</span></span>

<span data-ttu-id="2dbd7-108">Se instalou o Azure PowerShell através do PowerShellGet, pode utilizar o cmdlet [Uninstall-Module](/powershell/module/powershellget/uninstall-module).</span><span class="sxs-lookup"><span data-stu-id="2dbd7-108">If you installed Azure PowerShell using PowerShellGet, you can use the [Uninstall-Module](/powershell/module/powershellget/uninstall-module) cmdlet.</span></span> <span data-ttu-id="2dbd7-109">No entanto, `Uninstall-Module` desinstala apenas um módulo.</span><span class="sxs-lookup"><span data-stu-id="2dbd7-109">However, `Uninstall-Module` only uninstalls one module.</span></span> <span data-ttu-id="2dbd7-110">Para remover completamente o Azure PowerShell, tem de desinstalar cada módulo individualmente.</span><span class="sxs-lookup"><span data-stu-id="2dbd7-110">To remove Azure PowerShell completely, you must uninstall each module individually.</span></span> <span data-ttu-id="2dbd7-111">A desinstalação pode ser complicada se tiver mais de uma versão do Azure PowerShell instalada.</span><span class="sxs-lookup"><span data-stu-id="2dbd7-111">Uninstallation can be complicated if you have more than one version of Azure PowerShell installed.</span></span>

<span data-ttu-id="2dbd7-112">Para ver que versões do Azure PowerShell tem atualmente instaladas, execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="2dbd7-112">To check which versions of Azure PowerShell you currently have installed, run the following command:</span></span>

```powershell-interactive
Get-InstalledModule -Name AzureRM -AllVersions
```

```output
Version              Name                                Repository           Description
-------              ----                                ----------           -----------
6.11.0               AzureRM                             PSGallery            Azure Resource Manager Module
6.13.1               AzureRM                             PSGallery            Azure Resource Manager Module
```

<span data-ttu-id="2dbd7-113">O script seguinte consulta a Galeria do PowerShell para obter uma lista dos submódulos dependentes.</span><span class="sxs-lookup"><span data-stu-id="2dbd7-113">The following script queries the PowerShell Gallery to get a list of dependent submodules.</span></span> <span data-ttu-id="2dbd7-114">Em seguida, o script desinstala a versão correta de cada submódulo.</span><span class="sxs-lookup"><span data-stu-id="2dbd7-114">Then, the script uninstalls the correct version of each submodule.</span></span> <span data-ttu-id="2dbd7-115">Precisa de ter acesso de administrador para executar este script num âmbito diferente de `Process` ou `CurrentUser`.</span><span class="sxs-lookup"><span data-stu-id="2dbd7-115">You will need to have administrator access to run this script in a scope other than `Process` or `CurrentUser`.</span></span>

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

<span data-ttu-id="2dbd7-116">Para utilizar esta função, copie e cole o código na sua sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2dbd7-116">To use this function, copy and paste the code into your PowerShell session.</span></span> <span data-ttu-id="2dbd7-117">O exemplo a seguir mostra como executar a função para remover uma versão mais antiga do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2dbd7-117">The following example shows how to run the function to remove an older version of Azure PowerShell.</span></span>

```powershell-interactive
Uninstall-AllModules -TargetModule AzureRM -Version 4.4.1 -Force
```

<span data-ttu-id="2dbd7-118">À medida que o script é executado, apresenta o nome e a versão de cada submódulo que está a ser desinstalado.</span><span class="sxs-lookup"><span data-stu-id="2dbd7-118">As the script runs, it will display the name and version of each submodule that is being uninstalled.</span></span> <span data-ttu-id="2dbd7-119">Para executar o script para apenas ver o que seria eliminar, sem o remover, utilize a opção `-WhatIf`.</span><span class="sxs-lookup"><span data-stu-id="2dbd7-119">To run the script to only see what would be deleted, without removing it, use the `-WhatIf` option.</span></span>

```output
Creating list of dependencies...
Uninstalling AzureRM.Profile version 3.4.1
Uninstalling Azure.Storage version 3.4.1
Uninstalling AzureRM.AnalysisServices version 0.4.7
Uninstalling Azure.AnalysisServices version 0.4.7
...
```

<span data-ttu-id="2dbd7-120">Execute este comando para cada versão do Azure PowerShell que deseja desinstalar.</span><span class="sxs-lookup"><span data-stu-id="2dbd7-120">Run this command for every version of Azure PowerShell that you want to uninstall.</span></span> <span data-ttu-id="2dbd7-121">Para sua conveniência, o seguinte script desinstala todas as versões do AzureRM __exceto__ a última.</span><span class="sxs-lookup"><span data-stu-id="2dbd7-121">For convenience, the following script will uninstall all versions of AzureRM __except__ for the latest.</span></span>

```powershell-interactive
$versions = (get-installedmodule AzureRM -AllVersions | Select-Object Version)
$versions[1..($versions.Length-1)]  | foreach { Uninstall-AllModules -TargetModule AzureRM -Version ($_.Version) -Force }
```

## <a name="uninstall-msi"></a><span data-ttu-id="2dbd7-122">Desinstalar o MSI</span><span class="sxs-lookup"><span data-stu-id="2dbd7-122">Uninstall MSI</span></span>

<span data-ttu-id="2dbd7-123">Se instalou o Azure PowerShell através do pacote de MSI, a desinstalação deve ser feita através do sistema do Windows, e não através do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2dbd7-123">If you installed Azure PowerShell using the MSI package, you must uninstall through the Windows system rather than PowerShell.</span></span>

| <span data-ttu-id="2dbd7-124">Plataforma</span><span class="sxs-lookup"><span data-stu-id="2dbd7-124">Platform</span></span> | <span data-ttu-id="2dbd7-125">Instruções</span><span class="sxs-lookup"><span data-stu-id="2dbd7-125">Instructions</span></span> |
|----------|--------------|
| <span data-ttu-id="2dbd7-126">Windows 10</span><span class="sxs-lookup"><span data-stu-id="2dbd7-126">Windows 10</span></span> | <span data-ttu-id="2dbd7-127">Iniciar > Definições > Aplicações</span><span class="sxs-lookup"><span data-stu-id="2dbd7-127">Start > Settings > Apps</span></span> |
| <span data-ttu-id="2dbd7-128">Windows 7</span><span class="sxs-lookup"><span data-stu-id="2dbd7-128">Windows 7</span></span> </br><span data-ttu-id="2dbd7-129">Windows 8</span><span class="sxs-lookup"><span data-stu-id="2dbd7-129">Windows 8</span></span> | <span data-ttu-id="2dbd7-130">Iniciar > Painel de Controlo > Programas > Desinstalar um programa</span><span class="sxs-lookup"><span data-stu-id="2dbd7-130">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="2dbd7-131">Quando estiver neste ecrã, verá "Azure PowerShell" na lista de programas e poderá desinstalar a partir daí.</span><span class="sxs-lookup"><span data-stu-id="2dbd7-131">Once on this screen you should see "Azure PowerShell" in the program listing, and can uninstall from there.</span></span>
