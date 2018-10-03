---
title: Instalar o Azure PowerShell no macOS ou Linux
description: Como instalar o Azure PowerShell no macOS ou Linux.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/24/2018
ms.openlocfilehash: 05e86d96b345455f3d3bb3fe6dedf933fff6187c
ms.sourcegitcommit: 19dffee617477001f98d43e39a50ce1fad087b74
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2018
ms.locfileid: "47179246"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a><span data-ttu-id="8506b-103">Instalar o Azure PowerShell no macOS ou Linux</span><span class="sxs-lookup"><span data-stu-id="8506b-103">Install Azure PowerShell on macOS or Linux</span></span>

<span data-ttu-id="8506b-104">É possível executar o Azure PowerShell no PowerShell Core v6 em plataformas não Windows.</span><span class="sxs-lookup"><span data-stu-id="8506b-104">For non-Windows platforms, it's possible to run Azure PowerShell in PowerShell Core v6.</span></span> <span data-ttu-id="8506b-105">Esta versão do PowerShell foi concebida para ser utilizada em qualquer plataforma que suporte o .NET Core.</span><span class="sxs-lookup"><span data-stu-id="8506b-105">This version of PowerShell is built for use on any platform that supports .NET Core.</span></span> <span data-ttu-id="8506b-106">Para trabalhar com estas plataformas, está disponível uma versão standard de .NET do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8506b-106">To work with these platforms, there's a .NET Standard version of Azure PowerShell available.</span></span>

> [!NOTE]
> <span data-ttu-id="8506b-107">Atualmente, tanto o PowerShell Core v6, como o Azure PowerShell para .NET Standard, ainda se encontram em fase beta.</span><span class="sxs-lookup"><span data-stu-id="8506b-107">At this time, both PowerShell Core v6 and Azure PowerShell for .NET Standard are still in beta.</span></span>
> <span data-ttu-id="8506b-108">O suporte para estes produtos é limitado.</span><span class="sxs-lookup"><span data-stu-id="8506b-108">Support for these products is limited.</span></span> <span data-ttu-id="8506b-109">Se se deparar com problemas ou detetar erros, registe um problema no GitHub.</span><span class="sxs-lookup"><span data-stu-id="8506b-109">If you have problems or discover bugs, please file an issue on GitHub.</span></span>
>
> * [<span data-ttu-id="8506b-110">Problemas do PowerShell Core v6</span><span class="sxs-lookup"><span data-stu-id="8506b-110">Issues for PowerShell Core v6</span></span>](https://github.com/PowerShell/PowerShell/issues)
> * [<span data-ttu-id="8506b-111">Problemas do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="8506b-111">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core"></a><span data-ttu-id="8506b-112">Instalar o PowerShell Core</span><span class="sxs-lookup"><span data-stu-id="8506b-112">Install PowerShell Core</span></span>

<span data-ttu-id="8506b-113">As instruções de instalação do PowerShell Core são diferentes para o macOS e para a maioria das distribuições do Linux.</span><span class="sxs-lookup"><span data-stu-id="8506b-113">The installation instructions for PowerShell Core are different for macOS and most Linux distributions.</span></span>
<span data-ttu-id="8506b-114">Pode encontrar instruções detalhadas nos seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="8506b-114">Detailed instructions can be found in the following articles:</span></span>

* [<span data-ttu-id="8506b-115">Instalar o PowerShell Core no macOS</span><span class="sxs-lookup"><span data-stu-id="8506b-115">Install PowerShell Core on macOS</span></span>](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [<span data-ttu-id="8506b-116">Instalar o PowerShell Core no Linux</span><span class="sxs-lookup"><span data-stu-id="8506b-116">Install PowerShell Core on Linux</span></span>](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-standard"></a><span data-ttu-id="8506b-117">Instalar o Azure PowerShell para .NET Standard</span><span class="sxs-lookup"><span data-stu-id="8506b-117">Install Azure PowerShell for .NET Standard</span></span>

> [!IMPORTANT]
> <span data-ttu-id="8506b-118">O módulo `AzureRM`, descrito noutros artigos, não funciona com o PowerShell Core.</span><span class="sxs-lookup"><span data-stu-id="8506b-118">The `AzureRM` module detailed in other articles does not work with PowerShell Core.</span></span>
> <span data-ttu-id="8506b-119">Tem de instalar o módulo `Az` para obter a funcionalidade do Azure PowerShell no Powershell Core.</span><span class="sxs-lookup"><span data-stu-id="8506b-119">You must install the `Az` module to get Azure PowerShell functionality in PowerShell Core.</span></span>

<span data-ttu-id="8506b-120">O PowerShell Core é fornecido com o módulo do PowerShellGet já instalado.</span><span class="sxs-lookup"><span data-stu-id="8506b-120">PowerShell Core comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="8506b-121">Inicie o PowerShell com o comando:</span><span class="sxs-lookup"><span data-stu-id="8506b-121">Start PowerShell with the command:</span></span>

```bash
pwsh
```

<span data-ttu-id="8506b-122">Para instalar o Azure PowerShell, execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="8506b-122">To install Azure PowerShell, run the following command:</span></span>

```powershell
Install-Module Az
```

> [!NOTE]
> <span data-ttu-id="8506b-123">Se se deparar com um erro de permissões quando tentar instalar o módulo, poderá ter de executar o PowerShell no modo de superutilizador para o instalar.</span><span class="sxs-lookup"><span data-stu-id="8506b-123">If you encounter a permissions error when attempting to install the module, you may need to run PowerShell in superuser mode to install modules.</span></span>
>
> ```bash
> sudo pwsh
> ```

<span data-ttu-id="8506b-124">Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="8506b-124">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="8506b-125">Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:</span><span class="sxs-lookup"><span data-stu-id="8506b-125">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="8506b-126">Responda `Yes` ou `Yes to All` para continuar com a instalação.</span><span class="sxs-lookup"><span data-stu-id="8506b-126">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

## <a name="enable-aliases"></a><span data-ttu-id="8506b-127">Permitir aliases</span><span class="sxs-lookup"><span data-stu-id="8506b-127">Enable aliases</span></span>

<span data-ttu-id="8506b-128">Para compatibilidade com o módulo `AzureRM` já existente, o módulo `Az` novo tem a capacidade de criar aliases de retrocompatibilidade para os cmdlets `AzureRM`.</span><span class="sxs-lookup"><span data-stu-id="8506b-128">For compatibility with the existing `AzureRM` module, the new `Az` module has the ability to create backwards compatible aliases for the `AzureRM` cmdlets.</span></span> <span data-ttu-id="8506b-129">Antes de utilizar o módulo pela primeira vez, configure esses aliases com o comando seguinte:</span><span class="sxs-lookup"><span data-stu-id="8506b-129">Before using the module for the first time, set up these aliases with the following command:</span></span>

```powershell
# Import the module into the PowerShell session
Import-Module Az
# Enable AzureRM aliases for the user
Enable-AzureRmAlias -Scope CurrentUser
```

<span data-ttu-id="8506b-130">Isto configura os aliases para o utilizador atual apenas.</span><span class="sxs-lookup"><span data-stu-id="8506b-130">This sets up aliases for the current user only.</span></span> <span data-ttu-id="8506b-131">Veja a ajuda do cmdlet para obter outros valores que podem ser fornecidos a `-Scope`, para configurar os aliases.</span><span class="sxs-lookup"><span data-stu-id="8506b-131">Check the cmdlet help for other values that can be provided to `-Scope` to set up the aliases.</span></span>

> [!NOTE]
> <span data-ttu-id="8506b-132">Se se deparar com um erro sobre a localização de um caminho, confirme que o mesmo existe no seu sistema local.</span><span class="sxs-lookup"><span data-stu-id="8506b-132">If you encounter an error about a path location, make sure that it exists on your local system.</span></span> <span data-ttu-id="8506b-133">No âmbito `CurrentUser`, este erro pode ser resolvido mediante a execução do seguinte comando em `bash`:</span><span class="sxs-lookup"><span data-stu-id="8506b-133">For the `CurrentUser` scope, this error can be resolved by running the following command in `bash`:</span></span>
>
> ```bash
> mkdir -p $HOME/.config/powershell
> ```

## <a name="sign-in"></a><span data-ttu-id="8506b-134">Iniciar sessão</span><span class="sxs-lookup"><span data-stu-id="8506b-134">Sign in</span></span>

<span data-ttu-id="8506b-135">Para começar a utilizar o Azure PowerShell, precisa de carregar `Az` para a sua sessão do PowerShell com o cmdlet [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) e, em seguida, iniciar sessão com as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="8506b-135">To start working with Azure PowerShell, you need to load `Az` into your PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span> <span data-ttu-id="8506b-136">__Não__ precisa de privilégios elevados para importar um módulo.</span><span class="sxs-lookup"><span data-stu-id="8506b-136">Importing a module does __not__ require elevated privileges.</span></span>

```powershell
# Import the module into the PowerShell session
Import-Module Az
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="8506b-137">Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada.</span><span class="sxs-lookup"><span data-stu-id="8506b-137">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="8506b-138">A importação automática do módulo `Az` implica configurar um perfil do PowerShell, um processo sobre o qual pode obter mais informações em [Acerca de Perfis](/powershell/module/microsoft.powershell.core/about/about_profiles).</span><span class="sxs-lookup"><span data-stu-id="8506b-138">Automatically importing the `Az` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="8506b-139">No macOS e no Linux, deve trabalhar com o seu perfil através da variável de ambiente `$Profile`.</span><span class="sxs-lookup"><span data-stu-id="8506b-139">On macOS and Linux, you should work with your profile through the `$Profile` environment variable.</span></span> <span data-ttu-id="8506b-140">Para saber como manter o início de sessão do Azure entre as sessões, veja [Manter credenciais do utilizador nas sessões do PowerShell](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="8506b-140">To learn how to persist your Azure sign-in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="8506b-141">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="8506b-141">Next Steps</span></span>

<span data-ttu-id="8506b-142">Para obter mais informações sobre como utilizar o Azure PowerShell, veja o artigo [Introdução ao Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="8506b-142">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
