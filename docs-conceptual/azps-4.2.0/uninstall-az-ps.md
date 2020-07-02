---
title: Desinstalar o Azure PowerShell
description: Como realizar uma desinstalação completa do Azure PowerShell
ms.date: 05/28/2020
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 4b40a3aebab84176a48bcdb0ef818cfa05dea269
ms.sourcegitcommit: 5523170e571fbd1dc93bd0fa4223aba3b324d3b0
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/25/2020
ms.locfileid: "85363361"
---
# <a name="uninstall-the-azure-powershell-module"></a><span data-ttu-id="e12cb-103">Desinstalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="e12cb-103">Uninstall the Azure PowerShell module</span></span>

<span data-ttu-id="e12cb-104">Este artigo explica como desinstalar uma versão mais antiga do Azure PowerShell ou removê-la completamente do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="e12cb-104">This article tells you how to uninstall an older version of Azure PowerShell, or completely remove it from your system.</span></span> <span data-ttu-id="e12cb-105">Se decidiu desinstalar completamente o Azure PowerShell, envie-nos os seus comentários através do cmdlet [Send-Feedback](/powershell/module/az.accounts/send-feedback).</span><span class="sxs-lookup"><span data-stu-id="e12cb-105">If you've decided to completely uninstall Azure PowerShell, give us some feedback through the [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet.</span></span> <span data-ttu-id="e12cb-106">Se encontrou um erro, agradecemos-se que [registe um problema no GitHub](https://github.com/azure/azure-powershell/issues) para o podermos resolver.</span><span class="sxs-lookup"><span data-stu-id="e12cb-106">If you encountered a bug, we'd appreciate it if you [file a GitHub issue](https://github.com/azure/azure-powershell/issues) so that it can be fixed.</span></span>

## <a name="uninstall-azure-powershell-from-msi"></a><span data-ttu-id="e12cb-107">Desinstale o Azure PowerShell do MSI</span><span class="sxs-lookup"><span data-stu-id="e12cb-107">Uninstall Azure PowerShell from MSI</span></span>

<span data-ttu-id="e12cb-108">Se instalou o Azure PowerShell através do pacote de MSI, a desinstalação deve ser feita através do sistema do Windows, e não através do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e12cb-108">If you installed Azure PowerShell using the MSI package, you must uninstall through the Windows system rather than PowerShell.</span></span>

|         <span data-ttu-id="e12cb-109">Plataforma</span><span class="sxs-lookup"><span data-stu-id="e12cb-109">Platform</span></span>         |                      <span data-ttu-id="e12cb-110">Instruções</span><span class="sxs-lookup"><span data-stu-id="e12cb-110">Instructions</span></span>                      |
| ------------------------ | ------------------------------------------------------ |
| <span data-ttu-id="e12cb-111">Windows 10</span><span class="sxs-lookup"><span data-stu-id="e12cb-111">Windows 10</span></span>               | <span data-ttu-id="e12cb-112">Iniciar > Definições > Aplicações</span><span class="sxs-lookup"><span data-stu-id="e12cb-112">Start > Settings > Apps</span></span>                                |
| <span data-ttu-id="e12cb-113">Windows 7</span><span class="sxs-lookup"><span data-stu-id="e12cb-113">Windows 7</span></span> </br><span data-ttu-id="e12cb-114">Windows 8</span><span class="sxs-lookup"><span data-stu-id="e12cb-114">Windows 8</span></span> | <span data-ttu-id="e12cb-115">Iniciar > Painel de Controlo > Programas > Desinstalar um programa</span><span class="sxs-lookup"><span data-stu-id="e12cb-115">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="e12cb-116">Quando estiver neste ecrã, verá **Azure PowerShell** na lista de programas.</span><span class="sxs-lookup"><span data-stu-id="e12cb-116">Once on this screen, you should see **Azure PowerShell** in the program listing.</span></span> <span data-ttu-id="e12cb-117">Esta é a aplicação a desinstalar.</span><span class="sxs-lookup"><span data-stu-id="e12cb-117">This is the app to uninstall.</span></span> <span data-ttu-id="e12cb-118">Se não vir este programa na lista, instalou através de PowerShellGet e deve seguir o conjunto seguinte de instruções.</span><span class="sxs-lookup"><span data-stu-id="e12cb-118">If you don't see this program listed, then you installed through PowerShellGet, and should follow the next set of instructions.</span></span>

## <a name="uninstall-azure-powershell-from-powershellget"></a><span data-ttu-id="e12cb-119">Desinstalar o Azure PowerShell do PowerShellGet</span><span class="sxs-lookup"><span data-stu-id="e12cb-119">Uninstall Azure PowerShell from PowerShellGet</span></span>

<span data-ttu-id="e12cb-120">Para desinstalar os módulos do Az, pode utilizar o cmdlet [Uninstall-Module](/powershell/module/powershellget/uninstall-module).</span><span class="sxs-lookup"><span data-stu-id="e12cb-120">To uninstall the Az modules, you can use the [Uninstall-Module](/powershell/module/powershellget/uninstall-module) cmdlet.</span></span> <span data-ttu-id="e12cb-121">No entanto, `Uninstall-Module` desinstala apenas um módulo.</span><span class="sxs-lookup"><span data-stu-id="e12cb-121">However, `Uninstall-Module` only uninstalls one module.</span></span> <span data-ttu-id="e12cb-122">Para remover completamente o Azure PowerShell, tem de desinstalar cada módulo individualmente.</span><span class="sxs-lookup"><span data-stu-id="e12cb-122">To remove Azure PowerShell completely, you must uninstall each module individually.</span></span> <span data-ttu-id="e12cb-123">A desinstalação pode ser complicada se tiver mais de uma versão do Azure PowerShell instalada.</span><span class="sxs-lookup"><span data-stu-id="e12cb-123">Uninstallation can be complicated if you have more than one version of Azure PowerShell installed.</span></span>

<span data-ttu-id="e12cb-124">Para ver que versões do Azure PowerShell instalou, execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="e12cb-124">To check which versions of Azure PowerShell you've installed, run the following command:</span></span>

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

<span data-ttu-id="e12cb-125">O script seguinte consulta a Galeria do PowerShell para obter uma lista dos submódulos dependentes.</span><span class="sxs-lookup"><span data-stu-id="e12cb-125">The following script queries the PowerShell Gallery to get a list of dependent submodules.</span></span> <span data-ttu-id="e12cb-126">Em seguida, o script desinstala a versão correta de cada submódulo.</span><span class="sxs-lookup"><span data-stu-id="e12cb-126">Then, the script uninstalls the correct version of each submodule.</span></span> <span data-ttu-id="e12cb-127">Precisa de ter acesso de administrador para executar este script num âmbito diferente de **Process** ou **CurrentUser**.</span><span class="sxs-lookup"><span data-stu-id="e12cb-127">You need to have administrator access to run this script in a scope other than **Process** or **CurrentUser**.</span></span>

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

<span data-ttu-id="e12cb-128">Para utilizar esta função, copie e cole o código na sua sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e12cb-128">To use this function, copy and paste the code into your PowerShell session.</span></span> <span data-ttu-id="e12cb-129">O exemplo a seguir mostra como executar a função para remover uma versão mais antiga do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e12cb-129">The following example shows how to run the function to remove an older version of Azure PowerShell.</span></span>

```powershell-interactive
Uninstall-AzModule -Name Az -Version 1.8.0
```

<span data-ttu-id="e12cb-130">À medida que o script é executado, apresenta o **Nome**, **Versão** e **Estado** de cada submódulo que está a ser desinstalado.</span><span class="sxs-lookup"><span data-stu-id="e12cb-130">As the script runs, it displays the **Name**, **Version**, and **State** of each submodule that is being uninstalled.</span></span> <span data-ttu-id="e12cb-131">Para executar o script de forma a apenas ver o que seria eliminado, sem o remover, especifique o parâmetro `-WhatIf`.</span><span class="sxs-lookup"><span data-stu-id="e12cb-131">To run the script to only see what would be deleted, without removing it, specify the `-WhatIf` parameter.</span></span>

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
> <span data-ttu-id="e12cb-132">Se não puder corresponder este script a uma dependência exata com a mesma versão para desinstalar, não irá desinstalar _nenhuma_ versão dessa dependência.</span><span class="sxs-lookup"><span data-stu-id="e12cb-132">If this script can't match an exact dependency with the same version to uninstall, it won't uninstall _any_ version of that dependency.</span></span> <span data-ttu-id="e12cb-133">Tal acontece porque podem existir outras versões do módulo de destino no seu sistema que dependem destas dependências.</span><span class="sxs-lookup"><span data-stu-id="e12cb-133">This is because there may be other versions of the target module on your system which rely on these dependencies.</span></span>

<span data-ttu-id="e12cb-134">Execute o exemplo seguinte para cada versão do Azure PowerShell que queira desinstalar.</span><span class="sxs-lookup"><span data-stu-id="e12cb-134">Run the following example for every version of Azure PowerShell that you want to uninstall.</span></span> <span data-ttu-id="e12cb-135">Para sua comodidade, o script que se segue desinstala todas as versões do Az, **exceto** a mais recente.</span><span class="sxs-lookup"><span data-stu-id="e12cb-135">For convenience, the following script uninstalls all versions of Az **except** for the latest.</span></span>

```powershell-interactive
$Modules = Get-InstalledModule -Name Az -AllVersions | 
    Sort-Object -Property Version -Descending | 
        Select-Object -Skip 1
$Modules | ForEach-Object {Uninstall-AzModule -Name $_.Name -Version $_.Version}
```

## <a name="uninstall-the-azurerm-module"></a><span data-ttu-id="e12cb-136">Desinstalar o módulo do AzureRM</span><span class="sxs-lookup"><span data-stu-id="e12cb-136">Uninstall the AzureRM module</span></span>

<span data-ttu-id="e12cb-137">Se tiver o módulo do Az instalado no seu sistema e quiser desinstalar o AzureRM, existem duas opções que não implicam a execução do script `Uninstall-AzModule` acima.</span><span class="sxs-lookup"><span data-stu-id="e12cb-137">If you have the Az module installed on your system and would like to uninstall AzureRM, there are two options that don't require running the `Uninstall-AzModule` script above.</span></span> <span data-ttu-id="e12cb-138">O método utilizado depende da forma como instalou o módulo AzureRM.</span><span class="sxs-lookup"><span data-stu-id="e12cb-138">Which method you follow depends on how you installed the AzureRM module.</span></span> <span data-ttu-id="e12cb-139">Se não tiver a certeza do método de instalação original, siga os passos para primeiro desinstalar um MSI.</span><span class="sxs-lookup"><span data-stu-id="e12cb-139">If you're not sure of your original install method, follow the steps for uninstalling an MSI first.</span></span>

### <a name="uninstall-azure-powershell-msi"></a><span data-ttu-id="e12cb-140">Desinstalar o MSI do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="e12cb-140">Uninstall Azure PowerShell MSI</span></span>

<span data-ttu-id="e12cb-141">Se instalou os módulos do AzureRM do Azure PowerShell através do pacote de MSI, a desinstalação deve ser feita através do sistema do Windows, e não através do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e12cb-141">If you installed the Azure PowerShell AzureRM modules using the MSI package, you must uninstall through the Windows system rather than PowerShell.</span></span>

|         <span data-ttu-id="e12cb-142">Plataforma</span><span class="sxs-lookup"><span data-stu-id="e12cb-142">Platform</span></span>         |                      <span data-ttu-id="e12cb-143">Instruções</span><span class="sxs-lookup"><span data-stu-id="e12cb-143">Instructions</span></span>                      |
| ------------------------ | ------------------------------------------------------ |
| <span data-ttu-id="e12cb-144">Windows 10</span><span class="sxs-lookup"><span data-stu-id="e12cb-144">Windows 10</span></span>               | <span data-ttu-id="e12cb-145">Iniciar > Definições > Aplicações</span><span class="sxs-lookup"><span data-stu-id="e12cb-145">Start > Settings > Apps</span></span>                                |
| <span data-ttu-id="e12cb-146">Windows 7</span><span class="sxs-lookup"><span data-stu-id="e12cb-146">Windows 7</span></span> </br><span data-ttu-id="e12cb-147">Windows 8</span><span class="sxs-lookup"><span data-stu-id="e12cb-147">Windows 8</span></span> | <span data-ttu-id="e12cb-148">Iniciar > Painel de Controlo > Programas > Desinstalar um programa</span><span class="sxs-lookup"><span data-stu-id="e12cb-148">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="e12cb-149">Quando estiver neste ecrã, verá **Azure PowerShell** ou **Microsoft Azure PowerShell - Month Year** na lista de programas.</span><span class="sxs-lookup"><span data-stu-id="e12cb-149">Once on this screen, you should see **Azure PowerShell** or **Microsoft Azure PowerShell - Month Year** in the program listing.</span></span> <span data-ttu-id="e12cb-150">Esta é a aplicação a desinstalar.</span><span class="sxs-lookup"><span data-stu-id="e12cb-150">This is the app to uninstall.</span></span> <span data-ttu-id="e12cb-151">Se não vir este programa na lista, instalou através de PowerShellGet e deve seguir o conjunto seguinte de instruções.</span><span class="sxs-lookup"><span data-stu-id="e12cb-151">If you don't see this program listed, then you installed through PowerShellGet, and should follow the next set of instructions.</span></span>

### <a name="uninstall-from-powershell"></a><span data-ttu-id="e12cb-152">Desinstalar a partir do PowerShell</span><span class="sxs-lookup"><span data-stu-id="e12cb-152">Uninstall from PowerShell</span></span>

<span data-ttu-id="e12cb-153">Se instalou o AzureRM com o PowerShellGet, pode remover os módulos com o cmdlet [Uninstall-AzureRM](/powershell/module/az.accounts/uninstall-azurerm), disponível como parte do módulo `Az.Accounts`.</span><span class="sxs-lookup"><span data-stu-id="e12cb-153">If you installed AzureRM with PowerShellGet, then you can remove the modules with the [Uninstall-AzureRM](/powershell/module/az.accounts/uninstall-azurerm) cmdlet, available as part of the `Az.Accounts` module.</span></span> <span data-ttu-id="e12cb-154">O exemplo seguinte remove _todos_ os módulos do AzureRM do seu computador, mas precisa de ter privilégios de administrador.</span><span class="sxs-lookup"><span data-stu-id="e12cb-154">The following example removes _all_ AzureRM modules from your machine but requires administrator privileges.</span></span>

```powershell-interactive
Uninstall-AzureRm
```

<span data-ttu-id="e12cb-155">Se não conseguir executar o comando `Uninstall-AzureRM` com êxito, utilize o [script `Uninstall-AzModule`](#uninstall-script) fornecido neste artigo com a seguinte invocação:</span><span class="sxs-lookup"><span data-stu-id="e12cb-155">If you can't successfully run the `Uninstall-AzureRM` command, use the [`Uninstall-AzModule` script](#uninstall-script) provided in this article with the following invocation:</span></span>

```powershell-interactive
$Modules = Get-InstalledModule -Name AzureRM -AllVersions
$Modules | ForEach-Object {Uninstall-AzModule -Name $_.Name -Version $_.Version}
```
