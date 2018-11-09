---
title: Instalar o Azure PowerShell no macOS ou Linux
description: Como instalar o Azure PowerShell no macOS ou Linux.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/05/2018
ms.openlocfilehash: f60ea1c608be4b1c8319d53303713ba039276abc
ms.sourcegitcommit: 06f9206e025afa7207d4657c8f57c94ddb74817a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/07/2018
ms.locfileid: "51212896"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a><span data-ttu-id="68e09-103">Instalar o Azure PowerShell no macOS ou Linux</span><span class="sxs-lookup"><span data-stu-id="68e09-103">Install Azure PowerShell on macOS or Linux</span></span>

<span data-ttu-id="68e09-104">É possível executar o Azure PowerShell no PowerShell Core v6 em plataformas não Windows.</span><span class="sxs-lookup"><span data-stu-id="68e09-104">For non-Windows platforms, it's possible to run Azure PowerShell in PowerShell Core v6.</span></span> <span data-ttu-id="68e09-105">Esta versão do PowerShell foi concebida para ser utilizada em qualquer plataforma que suporte o .NET Core.</span><span class="sxs-lookup"><span data-stu-id="68e09-105">This version of PowerShell is built for use on any platform that supports .NET Core.</span></span> <span data-ttu-id="68e09-106">Para trabalhar com estas plataformas, está disponível uma versão standard de .NET do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="68e09-106">To work with these platforms, there's a .NET Standard version of Azure PowerShell available.</span></span>

> [!NOTE]
> <span data-ttu-id="68e09-107">De momento, o Azure PowerShell para .NET Standard ainda está em fase beta.</span><span class="sxs-lookup"><span data-stu-id="68e09-107">At this time, Azure PowerShell for .NET Standard is still in beta.</span></span>
> <span data-ttu-id="68e09-108">Se se deparar com problemas ou detetar erros, registe um problema no GitHub.</span><span class="sxs-lookup"><span data-stu-id="68e09-108">If you have problems or discover bugs, please file an issue on GitHub.</span></span>
>
> * [<span data-ttu-id="68e09-109">Problemas do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="68e09-109">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core"></a><span data-ttu-id="68e09-110">Instalar o PowerShell Core</span><span class="sxs-lookup"><span data-stu-id="68e09-110">Install PowerShell Core</span></span>

<span data-ttu-id="68e09-111">As instruções de instalação do PowerShell Core são diferentes para o macOS e para a maioria das distribuições do Linux.</span><span class="sxs-lookup"><span data-stu-id="68e09-111">The installation instructions for PowerShell Core are different for macOS and most Linux distributions.</span></span>
<span data-ttu-id="68e09-112">Pode encontrar instruções detalhadas nos seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="68e09-112">Detailed instructions can be found in the following articles:</span></span>

* [<span data-ttu-id="68e09-113">Instalar o PowerShell Core no macOS</span><span class="sxs-lookup"><span data-stu-id="68e09-113">Install PowerShell Core on macOS</span></span>](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [<span data-ttu-id="68e09-114">Instalar o PowerShell Core no Linux</span><span class="sxs-lookup"><span data-stu-id="68e09-114">Install PowerShell Core on Linux</span></span>](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-standard"></a><span data-ttu-id="68e09-115">Instalar o Azure PowerShell para .NET Standard</span><span class="sxs-lookup"><span data-stu-id="68e09-115">Install Azure PowerShell for .NET Standard</span></span>

> [!IMPORTANT]
> <span data-ttu-id="68e09-116">O módulo `AzureRM`, descrito noutros artigos, não funciona com o PowerShell Core.</span><span class="sxs-lookup"><span data-stu-id="68e09-116">The `AzureRM` module detailed in other articles does not work with PowerShell Core.</span></span>
> <span data-ttu-id="68e09-117">Tem de instalar o módulo `Az` para obter a funcionalidade do Azure PowerShell no Powershell Core.</span><span class="sxs-lookup"><span data-stu-id="68e09-117">You must install the `Az` module to get Azure PowerShell functionality in PowerShell Core.</span></span>

<span data-ttu-id="68e09-118">O PowerShell Core é fornecido com o módulo do PowerShellGet já instalado.</span><span class="sxs-lookup"><span data-stu-id="68e09-118">PowerShell Core comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="68e09-119">Inicie o PowerShell com o comando:</span><span class="sxs-lookup"><span data-stu-id="68e09-119">Start PowerShell with the command:</span></span>

```bash
pwsh
```

<span data-ttu-id="68e09-120">Para instalar o Azure PowerShell, execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="68e09-120">To install Azure PowerShell, run the following command:</span></span>

```powershell-interactive
Install-Module Az
```

> [!NOTE]
> <span data-ttu-id="68e09-121">Se se deparar com um erro de permissões quando tentar instalar o módulo, poderá ter de executar o PowerShell no modo de superutilizador para o instalar.</span><span class="sxs-lookup"><span data-stu-id="68e09-121">If you encounter a permissions error when attempting to install the module, you may need to run PowerShell in superuser mode to install modules.</span></span>
>
> ```bash
> sudo pwsh
> ```

<span data-ttu-id="68e09-122">Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="68e09-122">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="68e09-123">Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:</span><span class="sxs-lookup"><span data-stu-id="68e09-123">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="68e09-124">Responda `Yes` ou `Yes to All` para continuar com a instalação.</span><span class="sxs-lookup"><span data-stu-id="68e09-124">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

## <a name="enable-aliases"></a><span data-ttu-id="68e09-125">Permitir aliases</span><span class="sxs-lookup"><span data-stu-id="68e09-125">Enable aliases</span></span>

<span data-ttu-id="68e09-126">Para compatibilidade com o módulo `AzureRM` já existente, o módulo `Az` novo tem a capacidade de criar aliases de retrocompatibilidade para os cmdlets `AzureRM`.</span><span class="sxs-lookup"><span data-stu-id="68e09-126">For compatibility with the existing `AzureRM` module, the new `Az` module has the ability to create backwards compatible aliases for the `AzureRM` cmdlets.</span></span> <span data-ttu-id="68e09-127">Antes de utilizar o módulo pela primeira vez, configure esses aliases com o comando seguinte:</span><span class="sxs-lookup"><span data-stu-id="68e09-127">Before using the module for the first time, set up these aliases with the following command:</span></span>

```powershell-interactive
# Import the module into the PowerShell session
Import-Module Az
# Enable AzureRM aliases for the user
Enable-AzureRmAlias -Scope CurrentUser
```

<span data-ttu-id="68e09-128">Isto configura os aliases para o utilizador atual apenas.</span><span class="sxs-lookup"><span data-stu-id="68e09-128">This sets up aliases for the current user only.</span></span> <span data-ttu-id="68e09-129">Veja a ajuda do cmdlet para obter outros valores que podem ser fornecidos a `-Scope`, para configurar os aliases.</span><span class="sxs-lookup"><span data-stu-id="68e09-129">Check the cmdlet help for other values that can be provided to `-Scope` to set up the aliases.</span></span>

> [!NOTE]
> <span data-ttu-id="68e09-130">Se se deparar com um erro sobre a localização de um caminho, confirme que o mesmo existe no seu sistema local.</span><span class="sxs-lookup"><span data-stu-id="68e09-130">If you encounter an error about a path location, make sure that it exists on your local system.</span></span> <span data-ttu-id="68e09-131">No âmbito `CurrentUser`, este erro pode ser resolvido mediante a execução do seguinte comando em `bash`:</span><span class="sxs-lookup"><span data-stu-id="68e09-131">For the `CurrentUser` scope, this error can be resolved by running the following command in `bash`:</span></span>
>
> ```bash
> mkdir -p $HOME/.config/powershell
> ```

## <a name="sign-in"></a><span data-ttu-id="68e09-132">Iniciar sessão</span><span class="sxs-lookup"><span data-stu-id="68e09-132">Sign in</span></span>

<span data-ttu-id="68e09-133">Para começar a utilizar o Azure PowerShell, precisa de carregar `Az` para a sua sessão do PowerShell com o cmdlet [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) e, em seguida, iniciar sessão com as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="68e09-133">To start working with Azure PowerShell, you need to load `Az` into your PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span> <span data-ttu-id="68e09-134">__Não__ precisa de privilégios elevados para importar um módulo.</span><span class="sxs-lookup"><span data-stu-id="68e09-134">Importing a module does __not__ require elevated privileges.</span></span>

```powershell-interactive
# Import the module into the PowerShell session
Import-Module Az
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="68e09-135">Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada.</span><span class="sxs-lookup"><span data-stu-id="68e09-135">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="68e09-136">A importação automática do módulo `Az` implica configurar um perfil do PowerShell, um processo sobre o qual pode obter mais informações em [Acerca de Perfis](/powershell/module/microsoft.powershell.core/about/about_profiles).</span><span class="sxs-lookup"><span data-stu-id="68e09-136">Automatically importing the `Az` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="68e09-137">No macOS e no Linux, deve trabalhar com o seu perfil através da variável de ambiente `$Profile`.</span><span class="sxs-lookup"><span data-stu-id="68e09-137">On macOS and Linux, you should work with your profile through the `$Profile` environment variable.</span></span> <span data-ttu-id="68e09-138">Para saber como manter o início de sessão do Azure entre as sessões, veja [Manter credenciais do utilizador nas sessões do PowerShell](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="68e09-138">To learn how to persist your Azure sign-in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="68e09-139">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="68e09-139">Next Steps</span></span>

<span data-ttu-id="68e09-140">Para obter mais informações sobre como utilizar o Azure PowerShell, veja o artigo [Introdução ao Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="68e09-140">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
