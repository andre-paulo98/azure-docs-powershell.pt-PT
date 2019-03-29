---
title: Desinstalar o Azure PowerShell
description: Como realizar uma desinstalação completa do Azure PowerShell
ms.date: 12/13/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 6a34ac1821c3cec359d0d64664d3f1689621b304
ms.sourcegitcommit: 8f59e11e5c991543964154d63648aa1e6ae22512
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/26/2019
ms.locfileid: "58475573"
---
# <a name="uninstall-the-azure-powershell-module"></a><span data-ttu-id="2609f-103">Desinstalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="2609f-103">Uninstall the Azure PowerShell module</span></span>

<span data-ttu-id="2609f-104">Este artigo explica como desinstalar uma versão mais antiga do Azure PowerShell ou removê-la completamente do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="2609f-104">This article tells you how to uninstall an older version of Azure PowerShell, or completely remove it from your system.</span></span> <span data-ttu-id="2609f-105">Se decidiu desinstalar completamente o Azure PowerShell, envie-nos os seus comentários através do cmdlet [Send-Feedback](/powershell/module/az.accounts/send-feedback).</span><span class="sxs-lookup"><span data-stu-id="2609f-105">If you've decided to completely uninstall the Azure PowerShell, give us some feedback through the [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet.</span></span>
<span data-ttu-id="2609f-106">Se encontrar um erro, agradecemos-se que [registe um problema no GitHub](https://github.com/azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="2609f-106">If you encounter a bug, we'd appreciate it if you [file a GitHub issue](https://github.com/azure/azure-powershell/issues).</span></span>

## <a name="uninstall-the-az-module"></a><span data-ttu-id="2609f-107">Desinstalar o módulo do Az</span><span class="sxs-lookup"><span data-stu-id="2609f-107">Uninstall the Az module</span></span>

<span data-ttu-id="2609f-108">Para desinstalar os módulos do Az, utilize o cmdlet [Uninstall-Module](/powershell/module/powershellget/uninstall-module).</span><span class="sxs-lookup"><span data-stu-id="2609f-108">To uninstall the Az modules, use the [Uninstall-Module](/powershell/module/powershellget/uninstall-module) cmdlet.</span></span> <span data-ttu-id="2609f-109">No entanto, `Uninstall-Module` desinstala apenas um módulo.</span><span class="sxs-lookup"><span data-stu-id="2609f-109">However, `Uninstall-Module` only uninstalls one module.</span></span> <span data-ttu-id="2609f-110">Para remover completamente o Azure PowerShell, tem de desinstalar cada módulo individualmente.</span><span class="sxs-lookup"><span data-stu-id="2609f-110">To remove Azure PowerShell completely, you must uninstall each module individually.</span></span> <span data-ttu-id="2609f-111">A desinstalação pode ser complicada se tiver mais de uma versão do Azure PowerShell instalada.</span><span class="sxs-lookup"><span data-stu-id="2609f-111">Uninstallation can be complicated if you have more than one version of Azure PowerShell installed.</span></span>

<span data-ttu-id="2609f-112">Para ver que versões do Azure PowerShell tem atualmente instaladas, execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="2609f-112">To check which versions of Azure PowerShell you currently have installed, run the following command:</span></span>

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions
```

```output
Version             Name                           Repository           Description
-------             ----                           ----------           -----------
0.7.0               Az                             PSGallery            Azure Resource Manager Module
1.0.0               Az                             PSGallery            Azure Resource Manager Module
```

<span data-ttu-id="2609f-113">O script seguinte consulta a Galeria do PowerShell para obter uma lista dos submódulos dependentes.</span><span class="sxs-lookup"><span data-stu-id="2609f-113">The following script queries the PowerShell Gallery to get a list of dependent submodules.</span></span> <span data-ttu-id="2609f-114">Em seguida, o script desinstala a versão correta de cada submódulo.</span><span class="sxs-lookup"><span data-stu-id="2609f-114">Then, the script uninstalls the correct version of each submodule.</span></span> <span data-ttu-id="2609f-115">Precisa de ter acesso de administrador para executar este script num âmbito diferente de `Process` ou `CurrentUser`.</span><span class="sxs-lookup"><span data-stu-id="2609f-115">You will need to have administrator access to run this script in a scope other than `Process` or `CurrentUser`.</span></span>

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

<span data-ttu-id="2609f-116">Para utilizar esta função, copie e cole o código na sua sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2609f-116">To use this function, copy and paste the code into your PowerShell session.</span></span> <span data-ttu-id="2609f-117">O exemplo a seguir mostra como executar a função para remover uma versão mais antiga do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2609f-117">The following example shows how to run the function to remove an older version of Azure PowerShell.</span></span>

```powershell-interactive
Uninstall-AllModules -TargetModule Az -Version 0.7.0 -Force
```

<span data-ttu-id="2609f-118">À medida que o script é executado, apresenta o nome e a versão de cada submódulo que está a ser desinstalado.</span><span class="sxs-lookup"><span data-stu-id="2609f-118">As the script runs, it will display the name and version of each submodule that is being uninstalled.</span></span> <span data-ttu-id="2609f-119">Para executar o script para apenas ver o que seria eliminar, sem o remover, utilize a opção `-WhatIf`.</span><span class="sxs-lookup"><span data-stu-id="2609f-119">To run the script to only see what would be deleted, without removing it, use the `-WhatIf` option.</span></span>

```output
Creating list of dependencies...
Uninstalling Az.Profile version 0.7.0
Uninstalling Az.Aks version 0.7.0
Uninstalling Az.AnalysisServices version 0.7.0
...
```

<span data-ttu-id="2609f-120">Execute este comando para cada versão do Azure PowerShell que deseja desinstalar.</span><span class="sxs-lookup"><span data-stu-id="2609f-120">Run this command for every version of Azure PowerShell that you want to uninstall.</span></span> <span data-ttu-id="2609f-121">Para sua comodidade, o script que se segue desinstala todas as versões do Az __exceto__ a mais recente.</span><span class="sxs-lookup"><span data-stu-id="2609f-121">For convenience, the following script will uninstall all versions of Az __except__ for the latest.</span></span>

```powershell-interactive
$versions = (Get-InstalledModule Az -AllVersions | Select-Object Version)
$versions[1..($versions.Length-1)]  | foreach { Uninstall-AllModules -TargetModule Az -Version ($_.Version) -Force }
```

## <a name="uninstall-the-azurerm-module"></a><span data-ttu-id="2609f-122">Desinstalar o módulo do AzureRM</span><span class="sxs-lookup"><span data-stu-id="2609f-122">Uninstall the AzureRM module</span></span>

<span data-ttu-id="2609f-123">Se tiver o módulo do Az instalado no seu sistema e quiser desinstalar o AzureRM, existem duas opções que não implicam a execução do script `Uninstall-AllModules` acima.</span><span class="sxs-lookup"><span data-stu-id="2609f-123">If you have the Az module installed on your system and would like to uninstall AzureRM, there are two options that don't require running the `Uninstall-AllModules` script above.</span></span> <span data-ttu-id="2609f-124">O método utilizado depende da forma como instalou o módulo AzureRM.</span><span class="sxs-lookup"><span data-stu-id="2609f-124">Which method you follow depends on how you installed the AzureRM module.</span></span>
<span data-ttu-id="2609f-125">Se não tiver a certeza, siga os passos para desinstalar um MSI primeiro.</span><span class="sxs-lookup"><span data-stu-id="2609f-125">If you're not sure, follow the steps for uninstalling an MSI first.</span></span>

### <a name="uninstall-azure-powershell-msi"></a><span data-ttu-id="2609f-126">Desinstalar o MSI do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="2609f-126">Uninstall Azure PowerShell MSI</span></span>

<span data-ttu-id="2609f-127">Se instalou os módulos do AzureRM do Azure PowerShell através do pacote de MSI, a desinstalação deve ser feita através do sistema do Windows, e não através do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2609f-127">If you installed the Azure PowerShell AzureRM modules using the MSI package, you must uninstall through the Windows system rather than PowerShell.</span></span>

| <span data-ttu-id="2609f-128">Plataforma</span><span class="sxs-lookup"><span data-stu-id="2609f-128">Platform</span></span> | <span data-ttu-id="2609f-129">Instruções</span><span class="sxs-lookup"><span data-stu-id="2609f-129">Instructions</span></span> |
|----------|--------------|
| <span data-ttu-id="2609f-130">Windows 10</span><span class="sxs-lookup"><span data-stu-id="2609f-130">Windows 10</span></span> | <span data-ttu-id="2609f-131">Iniciar > Definições > Aplicações</span><span class="sxs-lookup"><span data-stu-id="2609f-131">Start > Settings > Apps</span></span> |
| <span data-ttu-id="2609f-132">Windows 7</span><span class="sxs-lookup"><span data-stu-id="2609f-132">Windows 7</span></span> </br><span data-ttu-id="2609f-133">Windows 8</span><span class="sxs-lookup"><span data-stu-id="2609f-133">Windows 8</span></span> | <span data-ttu-id="2609f-134">Iniciar > Painel de Controlo > Programas > Desinstalar um programa</span><span class="sxs-lookup"><span data-stu-id="2609f-134">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="2609f-135">Quando estiver neste ecrã, verá __Azure PowerShell__ na lista de programas.</span><span class="sxs-lookup"><span data-stu-id="2609f-135">Once on this screen you should see __Azure PowerShell__ in the program listing.</span></span> <span data-ttu-id="2609f-136">Esta é a aplicação a desinstalar.</span><span class="sxs-lookup"><span data-stu-id="2609f-136">This is the app to uninstall.</span></span> <span data-ttu-id="2609f-137">Se não vir este programa na lista, instalou através de PowerShellGet e deve seguir o conjunto seguinte de instruções.</span><span class="sxs-lookup"><span data-stu-id="2609f-137">If you don't see this program listed, then you installed through PowerShellGet, and should follow the next set of instructions.</span></span>

### <a name="uninstall-from-powershell"></a><span data-ttu-id="2609f-138">Desinstalar a partir do PowerShell</span><span class="sxs-lookup"><span data-stu-id="2609f-138">Uninstall from PowerShell</span></span>

<span data-ttu-id="2609f-139">Se instalou o AzureRM com o PowerShellGet, pode remover os módulos com o comando [Uninstall-AzureRM](/powershell/module/az.accounts/uninstall-azurerm), disponível como parte do módulo `Az.Accounts`.</span><span class="sxs-lookup"><span data-stu-id="2609f-139">If you installed AzureRM with PowerShellGet, then you can remove the modules with the [Uninstall-AzureRM](/powershell/module/az.accounts/uninstall-azurerm) command, available as part of the `Az.Accounts` module.</span></span> <span data-ttu-id="2609f-140">Esta ação remove _todos_ os módulos do AzureRM do seu computador, mas precisa de ter privilégios de administrador.</span><span class="sxs-lookup"><span data-stu-id="2609f-140">This removes _all_ AzureRM modules from your machine, but requires administrator privileges.</span></span>

```powershell-interactive
Uninstall-AzureRm
```

<span data-ttu-id="2609f-141">Se não conseguir executar o comando `Uninstall-AzureRM` com êxito, utilize o script `Uninstall-AllModules` fornecido neste artigo.</span><span class="sxs-lookup"><span data-stu-id="2609f-141">If you can't successfully run the `Uninstall-AzureRM` command, use the `Uninstall-AllModules` script provided in this article instead.</span></span>