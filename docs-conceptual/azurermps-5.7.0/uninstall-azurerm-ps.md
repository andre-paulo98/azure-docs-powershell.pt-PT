---
title: Desinstalar o Azure PowerShell
description: Como realizar uma desinstalação completa do Azure PowerShell
ms.date: 06/10/2019
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: cc0b6a4369116e92b8200ffbc0838d6ee2991263
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/05/2020
ms.locfileid: "67037688"
---
# <a name="uninstall-the-azure-powershell-module"></a><span data-ttu-id="28cb9-103">Desinstalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="28cb9-103">Uninstall the Azure PowerShell module</span></span>

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

<span data-ttu-id="28cb9-104">Este artigo explica como desinstalar uma versão mais antiga do Azure PowerShell ou removê-la completamente do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="28cb9-104">This article tells you how to uninstall an older version of Azure PowerShell, or completely remove it from your system.</span></span> <span data-ttu-id="28cb9-105">Se decidiu desinstalar completamente o Azure PowerShell, envie-nos os seus comentários através do cmdlet [Send-Feedback](/powershell/module/azurerm.profile/send-feedback).</span><span class="sxs-lookup"><span data-stu-id="28cb9-105">If you've decided to completely uninstall the Azure PowerShell, please give us some feedback through the [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet.</span></span>
<span data-ttu-id="28cb9-106">Se encontrou um erro, agradecemos-se que [registe um problema no GitHub](https://github.com/azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="28cb9-106">If you encountered a bug, we'd appreciate it if you [file a GitHub issue](https://github.com/azure/azure-powershell/issues).</span></span>

## <a name="uninstall-msi-or-web-platform-installer"></a><span data-ttu-id="28cb9-107">Desinstalar o MSI ou o Instalador da Plataforma Web</span><span class="sxs-lookup"><span data-stu-id="28cb9-107">Uninstall MSI or Web Platform Installer</span></span>

<span data-ttu-id="28cb9-108">Se instalou o Azure PowerShell com o pacote MSI ou o Instalador da Plataforma Web, deverá desinstalar o sistema do Windows, em vez do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="28cb9-108">If you installed Azure PowerShell using the MSI package or the Web Platform Installer, you must uninstall through the Windows system rather than PowerShell.</span></span>

| <span data-ttu-id="28cb9-109">Plataforma</span><span class="sxs-lookup"><span data-stu-id="28cb9-109">Platform</span></span> | <span data-ttu-id="28cb9-110">Instruções</span><span class="sxs-lookup"><span data-stu-id="28cb9-110">Instructions</span></span> |
|----------|--------------|
| <span data-ttu-id="28cb9-111">Windows 10</span><span class="sxs-lookup"><span data-stu-id="28cb9-111">Windows 10</span></span> | <span data-ttu-id="28cb9-112">Iniciar > Definições > Aplicações</span><span class="sxs-lookup"><span data-stu-id="28cb9-112">Start > Settings > Apps</span></span> |
| <span data-ttu-id="28cb9-113">Windows 7</span><span class="sxs-lookup"><span data-stu-id="28cb9-113">Windows 7</span></span> </br><span data-ttu-id="28cb9-114">Windows 8</span><span class="sxs-lookup"><span data-stu-id="28cb9-114">Windows 8</span></span> | <span data-ttu-id="28cb9-115">Iniciar > Painel de Controlo > Programas > Desinstalar um programa</span><span class="sxs-lookup"><span data-stu-id="28cb9-115">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="28cb9-116">Quando estiver neste ecrã, verá "Azure PowerShell" na lista de programas e poderá desinstalar a partir daí.</span><span class="sxs-lookup"><span data-stu-id="28cb9-116">Once on this screen you should see "Azure PowerShell" in the program listing, and can uninstall from there.</span></span>

## <a name="uninstall-from-powershell"></a><span data-ttu-id="28cb9-117">Desinstalar a partir do PowerShell</span><span class="sxs-lookup"><span data-stu-id="28cb9-117">Uninstall from PowerShell</span></span>

<span data-ttu-id="28cb9-118">Se instalou o Azure PowerShell através do PowerShellGet, pode utilizar o cmdlet [Uninstall-Module](/powershell/module/powershellget/uninstall-module).</span><span class="sxs-lookup"><span data-stu-id="28cb9-118">If you installed Azure PowerShell using PowerShellGet, you can use the [Uninstall-Module](/powershell/module/powershellget/uninstall-module) cmdlet.</span></span> <span data-ttu-id="28cb9-119">No entanto, `Uninstall-Module` desinstala apenas um módulo.</span><span class="sxs-lookup"><span data-stu-id="28cb9-119">However, `Uninstall-Module` only uninstalls one module.</span></span> <span data-ttu-id="28cb9-120">Para remover completamente o Azure PowerShell, tem de desinstalar cada módulo individualmente.</span><span class="sxs-lookup"><span data-stu-id="28cb9-120">To remove Azure PowerShell completely, you must uninstall each module individually.</span></span> <span data-ttu-id="28cb9-121">A desinstalação pode ser complicada se tiver várias versões do Azure PowerShell instaladas.</span><span class="sxs-lookup"><span data-stu-id="28cb9-121">Uninstallation can be complicated if you have multiple versions of Azure PowerShell installed.</span></span>

<span data-ttu-id="28cb9-122">O script a seguir pode servir para remover completamente uma versão única do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="28cb9-122">You use the following script can be used to completely remove a single version of Azure PowerShell.</span></span> <span data-ttu-id="28cb9-123">O script consulta a Galeria do PowerShell para obter uma lista dos submódulos dependentes.</span><span class="sxs-lookup"><span data-stu-id="28cb9-123">The script queries the PowerShell Gallery to get a list of dependent submodules.</span></span> <span data-ttu-id="28cb9-124">Em seguida, o script desinstala a versão correta de cada submódulo.</span><span class="sxs-lookup"><span data-stu-id="28cb9-124">Then, the script uninstalls the correct version of each submodule.</span></span>

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
    if ($_.PSObject.Properties.Name -contains 'requiredVersion') {
      $AllModules += New-Object -TypeName psobject -Property @{name=$_.name; version=$_.requiredVersion}
    }
    else { # Assume minimum version
      # Minimum version actually reports the installed dependency
      # which is used, not the actual "minimum dependency." Check to
      # see if the requested version was installed as a dependency earlier.
      $candidate = Get-InstalledModule $_.name -RequiredVersion $version -ErrorAction Ignore
      if ($candidate) {
        $AllModules += New-Object -TypeName psobject -Property @{name=$_.name; version=$version}
      }
      else {
        $availableModules = Get-InstalledModule $_.name -AllVersions
        Write-Warning ("Could not find uninstall candidate for {0}:{1} - module may require manual uninstall. Available versions are: {2}" -f $_.name,$version,($availableModules.Version -join ', '))
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

<span data-ttu-id="28cb9-125">Para utilizar esta função, copie e cole o código na sua sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="28cb9-125">To use this function, copy and paste the code into your PowerShell session.</span></span> <span data-ttu-id="28cb9-126">O exemplo a seguir mostra como executar a função para remover uma versão mais antiga do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="28cb9-126">The following example shows how to run the function to remove an older version of Azure PowerShell.</span></span>

```powershell-interactive
Uninstall-AllModules -TargetModule AzureRM -Version 4.4.1 -Force
```

<span data-ttu-id="28cb9-127">À medida que o script é executado, apresenta o nome e a versão de cada submódulo que está a ser desinstalado.</span><span class="sxs-lookup"><span data-stu-id="28cb9-127">As the script runs, it will display the name and version of each submodule that is being uninstalled.</span></span> <span data-ttu-id="28cb9-128">Para executar o script para apenas ver o que seria eliminar, sem o remover, utilize a opção `-WhatIf`.</span><span class="sxs-lookup"><span data-stu-id="28cb9-128">To run the script to only see what would be deleted, without removing it, use the `-WhatIf` option.</span></span>

```output
Creating list of dependencies...
Uninstalling AzureRM.Profile version 3.4.1
Uninstalling Azure.Storage version 3.4.1
Uninstalling AzureRM.AnalysisServices version 0.4.7
Uninstalling Azure.AnalysisServices version 0.4.7
...
```

> [!NOTE]
> <span data-ttu-id="28cb9-129">Se não puder corresponder este script a uma dependência exata com a mesma versão para desinstalar, não irá desinstalar _qualquer_ versão dessa dependência.</span><span class="sxs-lookup"><span data-stu-id="28cb9-129">If this script can't match an exact dependency with the same version to uninstall, it won't uninstall _any_ version of that dependecy.</span></span> <span data-ttu-id="28cb9-130">Tal acontece porque podem existir outras versões do módulo de destino no seu sistema que dependem destas dependências.</span><span class="sxs-lookup"><span data-stu-id="28cb9-130">This is because there may be other versions of the target module on your system which rely on these dependencies.</span></span> <span data-ttu-id="28cb9-131">Neste caso, são listadas as versões disponíveis da dependência.</span><span class="sxs-lookup"><span data-stu-id="28cb9-131">In this case, the available versions of the dependency are listed.</span></span>
> <span data-ttu-id="28cb9-132">Em seguida, pode remover as versões antigas manualmente com `Uninstall-Module`.</span><span class="sxs-lookup"><span data-stu-id="28cb9-132">You can then remove any old versions manually with `Uninstall-Module`.</span></span>


<span data-ttu-id="28cb9-133">Execute este comando para cada versão do Azure PowerShell que deseja desinstalar.</span><span class="sxs-lookup"><span data-stu-id="28cb9-133">Run this command for every version of Azure PowerShell that you want to uninstall.</span></span> <span data-ttu-id="28cb9-134">Para sua conveniência, o seguinte script desinstala todas as versões do AzureRM __exceto__ a última.</span><span class="sxs-lookup"><span data-stu-id="28cb9-134">For convenience, the following script will uninstall all versions of AzureRM __except__ for the latest.</span></span>

```powershell-interactive
$versions = (get-installedmodule AzureRM -AllVersions | Select-Object Version)
$versions[0..($versions.Length-2)]  | foreach { Uninstall-AllModules -TargetModule AzureRM -Version ($_.Version) -Force }
```
