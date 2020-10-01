---
title: Desinstalar o Azure PowerShell
description: Como realizar uma desinstalação completa do Azure PowerShell
ms.date: 09/15/2020
ms.devlang: powershell
ms.topic: conceptual
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: 7f831bdf6d6144640e036d72900958847283acf1
ms.sourcegitcommit: 5fcf17330d6f335561640a5ee3d98c59f7baab94
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/26/2020
ms.locfileid: "91381501"
---
# <a name="how-to-uninstall-azure-powershell-modules"></a><span data-ttu-id="55c2b-103">Como desinstalar módulos do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="55c2b-103">How to uninstall Azure PowerShell modules</span></span>

<span data-ttu-id="55c2b-104">Este artigo explica como desinstalar uma versão mais antiga do Azure PowerShell ou removê-la completamente do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="55c2b-104">This article tells you how to uninstall an older version of Azure PowerShell, or completely remove it from your system.</span></span> <span data-ttu-id="55c2b-105">Se decidiu desinstalar completamente o Azure PowerShell, envie-nos os seus comentários através do cmdlet [Send-Feedback](/powershell/module/az.accounts/send-feedback).</span><span class="sxs-lookup"><span data-stu-id="55c2b-105">If you've decided to completely uninstall Azure PowerShell, give us some feedback through the [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet.</span></span> <span data-ttu-id="55c2b-106">Se encontrou um erro, agradecemos-se que [registe um problema no GitHub](https://github.com/azure/azure-powershell/issues) para o podermos resolver.</span><span class="sxs-lookup"><span data-stu-id="55c2b-106">If you encountered a bug, we'd appreciate it if you [file a GitHub issue](https://github.com/azure/azure-powershell/issues) so that it can be fixed.</span></span>

## <a name="uninstall-the-az-module"></a><span data-ttu-id="55c2b-107">Desinstalar o módulo do Az</span><span class="sxs-lookup"><span data-stu-id="55c2b-107">Uninstall the Az module</span></span>

<span data-ttu-id="55c2b-108">Se tiver o módulo Az instalado no seu sistema e quiser desinstalá-lo, existem duas opções.</span><span class="sxs-lookup"><span data-stu-id="55c2b-108">If you have the Az module installed on your system and would like to uninstall it, there are two options.</span></span> <span data-ttu-id="55c2b-109">O método utilizado depende da forma como instalou o módulo Az.</span><span class="sxs-lookup"><span data-stu-id="55c2b-109">Which method you follow depends on how you installed the Az module.</span></span> <span data-ttu-id="55c2b-110">Se não tiver a certeza do método de instalação original, siga os passos do MSI para primeiro desinstalar.</span><span class="sxs-lookup"><span data-stu-id="55c2b-110">If you're not sure of your original installation method, follow the MSI steps for uninstalling first.</span></span>

### <a name="option-1-uninstall-the-az-powershell-module-from-msi"></a><span data-ttu-id="55c2b-111">Opção 1: Desinstalar o módulo do Az PowerShell a partir do MSI</span><span class="sxs-lookup"><span data-stu-id="55c2b-111">Option 1: Uninstall the Az PowerShell module from MSI</span></span>

<span data-ttu-id="55c2b-112">Se instalou o módulo do Az PowerShell através do pacote de MSI, tem de fazer a desinstalação através do sistema Windows e não através do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="55c2b-112">If you installed Az PowerShell module using the MSI package, you must uninstall through the Windows system rather than PowerShell.</span></span>

|         <span data-ttu-id="55c2b-113">Plataforma</span><span class="sxs-lookup"><span data-stu-id="55c2b-113">Platform</span></span>         |                      <span data-ttu-id="55c2b-114">Instruções</span><span class="sxs-lookup"><span data-stu-id="55c2b-114">Instructions</span></span>                      |
| ------------------------ | ------------------------------------------------------ |
| <span data-ttu-id="55c2b-115">Windows 10</span><span class="sxs-lookup"><span data-stu-id="55c2b-115">Windows 10</span></span>               | <span data-ttu-id="55c2b-116">Iniciar > Definições > Aplicações</span><span class="sxs-lookup"><span data-stu-id="55c2b-116">Start > Settings > Apps</span></span>                                |
| <span data-ttu-id="55c2b-117">Windows 7</span><span class="sxs-lookup"><span data-stu-id="55c2b-117">Windows 7</span></span> </br><span data-ttu-id="55c2b-118">Windows 8</span><span class="sxs-lookup"><span data-stu-id="55c2b-118">Windows 8</span></span> | <span data-ttu-id="55c2b-119">Iniciar > Painel de Controlo > Programas > Desinstalar um programa</span><span class="sxs-lookup"><span data-stu-id="55c2b-119">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="55c2b-120">Quando estiver neste ecrã, verá **Azure PowerShell** na lista de programas.</span><span class="sxs-lookup"><span data-stu-id="55c2b-120">Once on this screen, you should see **Azure PowerShell** in the program listing.</span></span> <span data-ttu-id="55c2b-121">Esta é a aplicação a desinstalar.</span><span class="sxs-lookup"><span data-stu-id="55c2b-121">This is the app to uninstall.</span></span> <span data-ttu-id="55c2b-122">Se não vir este programa na lista, instalou através de PowerShellGet e deve seguir o conjunto seguinte de instruções.</span><span class="sxs-lookup"><span data-stu-id="55c2b-122">If you don't see this program listed, then you installed through PowerShellGet, and should follow the next set of instructions.</span></span>

### <a name="option-2-uninstall-the-az-powershell-module-from-powershellget"></a><span data-ttu-id="55c2b-123">Opção 2: Desinstalar o módulo do Az PowerShell a partir do PowerShellGet</span><span class="sxs-lookup"><span data-stu-id="55c2b-123">Option 2: Uninstall the Az PowerShell module from PowerShellGet</span></span>

<span data-ttu-id="55c2b-124">Para desinstalar os módulos do Az, pode utilizar o cmdlet [Uninstall-Module](/powershell/module/powershellget/uninstall-module).</span><span class="sxs-lookup"><span data-stu-id="55c2b-124">To uninstall the Az modules, you can use the [Uninstall-Module](/powershell/module/powershellget/uninstall-module) cmdlet.</span></span> <span data-ttu-id="55c2b-125">No entanto, `Uninstall-Module` desinstala apenas um módulo.</span><span class="sxs-lookup"><span data-stu-id="55c2b-125">However, `Uninstall-Module` only uninstalls one module.</span></span> <span data-ttu-id="55c2b-126">Para remover completamente o módulo do Az PowerShell, tem de desinstalar cada módulo individualmente.</span><span class="sxs-lookup"><span data-stu-id="55c2b-126">To remove the Az PowerShell module completely, you must uninstall each module individually.</span></span> <span data-ttu-id="55c2b-127">A desinstalação pode ser complicada se tiver mais de uma versão do Azure PowerShell instalada.</span><span class="sxs-lookup"><span data-stu-id="55c2b-127">Uninstallation can be complicated if you have more than one version of Azure PowerShell installed.</span></span>

<span data-ttu-id="55c2b-128">Para ver que versões do módulo do Az PowerShell instalou, execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="55c2b-128">To check which versions of the Az PowerShell module you've installed, run the following command:</span></span>

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions
```

```output
Version             Name                           Repository           Description
-------             ----                           ----------           -----------
3.8.0               Az                             PSGallery            Microsoft Azure PowerShell
4.1.0               Az                             PSGallery            Microsoft Azure PowerShell
```

<span data-ttu-id="55c2b-129">O script seguinte consulta a Galeria do PowerShell para obter uma lista dos submódulos dependentes.</span><span class="sxs-lookup"><span data-stu-id="55c2b-129">The following script queries the PowerShell Gallery to get a list of dependent submodules.</span></span> <span data-ttu-id="55c2b-130">Em seguida, o script desinstala a versão correta de cada submódulo.</span><span class="sxs-lookup"><span data-stu-id="55c2b-130">Then, the script uninstalls the correct version of each submodule.</span></span> <span data-ttu-id="55c2b-131">Precisa de ter acesso de administrador para executar este script num âmbito diferente de **Processo** ou **Utilizador Atual**.</span><span class="sxs-lookup"><span data-stu-id="55c2b-131">You need to have administrator access to run this script in a scope other than **Process** or **Current User**.</span></span>

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

<span data-ttu-id="55c2b-132">Para utilizar esta função, copie e cole o código na sua sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="55c2b-132">To use this function, copy and paste the code into your PowerShell session.</span></span> <span data-ttu-id="55c2b-133">O exemplo seguinte mostra como executar a função para remover uma versão mais antiga do módulo do Az PowerShell e os respetivos submódulos.</span><span class="sxs-lookup"><span data-stu-id="55c2b-133">The following example shows how to run the function to remove an older version of the Az PowerShell module and its submodules.</span></span>

```powershell-interactive
Uninstall-AzModule -Name Az -Version 1.8.0
```

<span data-ttu-id="55c2b-134">À medida que o script é executado, apresenta o **Nome**, **Versão** e **Estado** de cada submódulo que está a ser desinstalado.</span><span class="sxs-lookup"><span data-stu-id="55c2b-134">As the script runs, it displays the **Name**, **Version**, and **State** of each submodule that is being uninstalled.</span></span> <span data-ttu-id="55c2b-135">Para executar o script de forma a apenas ver o que seria eliminado, sem o remover, especifique o parâmetro `-WhatIf`.</span><span class="sxs-lookup"><span data-stu-id="55c2b-135">To run the script to only see what would be deleted, without removing it, specify the `-WhatIf` parameter.</span></span>

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
> <span data-ttu-id="55c2b-136">Se não puder corresponder este script a uma dependência exata com a mesma versão para desinstalar, não irá desinstalar _nenhuma_ versão dessa dependência.</span><span class="sxs-lookup"><span data-stu-id="55c2b-136">If this script can't match an exact dependency with the same version to uninstall, it won't uninstall _any_ version of that dependency.</span></span> <span data-ttu-id="55c2b-137">Tal acontece porque podem existir outras versões do módulo de destino no seu sistema que dependem destas dependências.</span><span class="sxs-lookup"><span data-stu-id="55c2b-137">This is because there may be other versions of the target module on your system which rely on these dependencies.</span></span>

<span data-ttu-id="55c2b-138">Execute o exemplo seguinte para cada versão do módulo do Az PowerShell que queira desinstalar.</span><span class="sxs-lookup"><span data-stu-id="55c2b-138">Run the following example for every version of the Az PowerShell module that you want to uninstall.</span></span>
<span data-ttu-id="55c2b-139">Para sua comodidade, o script que se segue desinstala todas as versões do Az, **exceto** a mais recente.</span><span class="sxs-lookup"><span data-stu-id="55c2b-139">For convenience, the following script uninstalls all versions of Az **except** for the latest.</span></span>

```powershell-interactive
$Modules = Get-InstalledModule -Name Az -AllVersions |
    Sort-Object -Property Version -Descending |
        Select-Object -Skip 1
$Modules | ForEach-Object {Uninstall-AzModule -Name $_.Name -Version $_.Version}
```

## <a name="uninstall-the-azurerm-module"></a><span data-ttu-id="55c2b-140">Desinstalar o módulo do AzureRM</span><span class="sxs-lookup"><span data-stu-id="55c2b-140">Uninstall the AzureRM module</span></span>

<span data-ttu-id="55c2b-141">Se tiver o módulo do Az instalado no seu sistema e quiser desinstalar o AzureRM, existem duas opções.</span><span class="sxs-lookup"><span data-stu-id="55c2b-141">If you have the Az module installed on your system and would like to uninstall AzureRM, there are two options.</span></span> <span data-ttu-id="55c2b-142">O método utilizado depende da forma como instalou o módulo AzureRM.</span><span class="sxs-lookup"><span data-stu-id="55c2b-142">Which method you follow depends on how you installed the AzureRM module.</span></span> <span data-ttu-id="55c2b-143">Se não tiver a certeza do método de instalação original, siga os passos do MSI para primeiro desinstalar.</span><span class="sxs-lookup"><span data-stu-id="55c2b-143">If you're not sure of your original installation method, follow the MSI steps for uninstalling first.</span></span>

### <a name="option-1-uninstall-the-azurerm-powershell-module-from-msi"></a><span data-ttu-id="55c2b-144">Opção 1: Desinstalar o módulo do AzureRM PowerShell a partir do MSI</span><span class="sxs-lookup"><span data-stu-id="55c2b-144">Option 1: Uninstall the AzureRM PowerShell module from MSI</span></span>

<span data-ttu-id="55c2b-145">Se instalou o módulo do AzureRM PowerShell através do pacote de MSI, tem de fazer a desinstalação através do sistema Windows e não através do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="55c2b-145">If you installed the AzureRM PowerShell module using the MSI package, you must uninstall through the Windows system rather than PowerShell.</span></span>

|         <span data-ttu-id="55c2b-146">Plataforma</span><span class="sxs-lookup"><span data-stu-id="55c2b-146">Platform</span></span>         |                      <span data-ttu-id="55c2b-147">Instruções</span><span class="sxs-lookup"><span data-stu-id="55c2b-147">Instructions</span></span>                      |
| ------------------------ | ------------------------------------------------------ |
| <span data-ttu-id="55c2b-148">Windows 10</span><span class="sxs-lookup"><span data-stu-id="55c2b-148">Windows 10</span></span>               | <span data-ttu-id="55c2b-149">Iniciar > Definições > Aplicações</span><span class="sxs-lookup"><span data-stu-id="55c2b-149">Start > Settings > Apps</span></span>                                |
| <span data-ttu-id="55c2b-150">Windows 7</span><span class="sxs-lookup"><span data-stu-id="55c2b-150">Windows 7</span></span> </br><span data-ttu-id="55c2b-151">Windows 8</span><span class="sxs-lookup"><span data-stu-id="55c2b-151">Windows 8</span></span> | <span data-ttu-id="55c2b-152">Iniciar > Painel de Controlo > Programas > Desinstalar um programa</span><span class="sxs-lookup"><span data-stu-id="55c2b-152">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="55c2b-153">Quando estiver neste ecrã, verá **Azure PowerShell** ou **Microsoft Azure PowerShell - Month Year** na lista de programas.</span><span class="sxs-lookup"><span data-stu-id="55c2b-153">Once on this screen, you should see **Azure PowerShell** or **Microsoft Azure PowerShell - Month Year** in the program listing.</span></span> <span data-ttu-id="55c2b-154">Esta é a aplicação a desinstalar.</span><span class="sxs-lookup"><span data-stu-id="55c2b-154">This is the app to uninstall.</span></span> <span data-ttu-id="55c2b-155">Se não vir este programa na lista, instalou através de PowerShellGet e deve seguir o conjunto seguinte de instruções.</span><span class="sxs-lookup"><span data-stu-id="55c2b-155">If you don't see this program listed, then you installed through PowerShellGet, and should follow the next set of instructions.</span></span>

### <a name="option-2-uninstall-the-azurerm-powershell-module-from-powershellget"></a><span data-ttu-id="55c2b-156">Opção 2: Desinstalar o módulo do AzureRM PowerShell a partir do PowerShellGet</span><span class="sxs-lookup"><span data-stu-id="55c2b-156">Option 2: Uninstall the AzureRM PowerShell module from PowerShellGet</span></span>

<span data-ttu-id="55c2b-157">Se instalou o AzureRM com o PowerShellGet, pode remover os módulos com o cmdlet [Uninstall-AzureRM](/powershell/module/az.accounts/uninstall-azurerm), disponível como parte do módulo `Az.Accounts`.</span><span class="sxs-lookup"><span data-stu-id="55c2b-157">If you installed AzureRM with PowerShellGet, then you can remove the modules with the [Uninstall-AzureRM](/powershell/module/az.accounts/uninstall-azurerm) cmdlet, available as part of the `Az.Accounts` module.</span></span>

<span data-ttu-id="55c2b-158">Para utilizar o módulo `Az.Accounts`, precisará de ter o módulo Az instalado.</span><span class="sxs-lookup"><span data-stu-id="55c2b-158">In order to use the `Az.Accounts` module, you will need to have the Az module installed.</span></span>  <span data-ttu-id="55c2b-159">Ter o módulo AzureRM e o módulo Az instalados ao mesmo tempo não é suportado. Contudo, o módulo Az pode ser utilizado para desinstalar imediatamente o módulo AzureRM.</span><span class="sxs-lookup"><span data-stu-id="55c2b-159">Having both the AzureRM and the Az modules installed at the same time is not supported however the Az module can be used to immediately uninstall the AzureRM module.</span></span>  <span data-ttu-id="55c2b-160">Pode instalar o módulo Az e ignorar o aviso do módulo AzureRM com o seguinte comando caso não tenha o módulo Az já instalado:</span><span class="sxs-lookup"><span data-stu-id="55c2b-160">You can install the Az module and bypass the AzureRM module warning with the following command if you do not have the Az module installed already:</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

<span data-ttu-id="55c2b-161">Quando o módulo AZ estiver instalado, o comando seguinte remove _todos_ os módulos AzureRM do seu computador.</span><span class="sxs-lookup"><span data-stu-id="55c2b-161">Once the Az module is installed, the following command removes _all_ AzureRM modules from your machine.</span></span> <span data-ttu-id="55c2b-162">Requer privilégios de administrador.</span><span class="sxs-lookup"><span data-stu-id="55c2b-162">It requires administrator privileges.</span></span>

```powershell-interactive
Uninstall-AzureRm
```
