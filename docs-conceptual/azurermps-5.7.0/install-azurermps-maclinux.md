---
title: Instalar o Azure PowerShell no macOS ou Linux
description: Como instalar o Azure PowerShell no macOS ou Linux.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 47611281f67d68c9fc2686e0c6156b060a225158
ms.sourcegitcommit: 80a3da199954d0ab78765715fb49793e89a30f12
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/22/2018
ms.locfileid: "52257759"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a><span data-ttu-id="43183-103">Instalar o Azure PowerShell no macOS ou Linux</span><span class="sxs-lookup"><span data-stu-id="43183-103">Install Azure PowerShell on macOS or Linux</span></span>

<span data-ttu-id="43183-104">É possível executar o Azure PowerShell no PowerShell Core v6 em plataformas não Windows.</span><span class="sxs-lookup"><span data-stu-id="43183-104">For non-Windows platforms, it's possible to run Azure PowerShell in PowerShell Core v6.</span></span> <span data-ttu-id="43183-105">Esta versão do PowerShell foi concebida para ser utilizada em qualquer plataforma que suporte o .NET Core.</span><span class="sxs-lookup"><span data-stu-id="43183-105">This version of PowerShell is built for use on any platform that supports .NET Core.</span></span> <span data-ttu-id="43183-106">Para trabalhar com estas plataformas, existe uma versão especial do Azure PowerShell disponível para o .NET Core.</span><span class="sxs-lookup"><span data-stu-id="43183-106">To work with these platforms, there's a special .NET Core version of Azure PowerShell available.</span></span>

> [!NOTE]
> <span data-ttu-id="43183-107">Atualmente, tanto o PowerShell Core v6 como o Azure PowerShell para .NET Core ainda se encontram em fase beta.</span><span class="sxs-lookup"><span data-stu-id="43183-107">At this time, both PowerShell Core v6 and Azure PowerShell for .NET Core are still in beta.</span></span>
> <span data-ttu-id="43183-108">O suporte para estes produtos é limitado.</span><span class="sxs-lookup"><span data-stu-id="43183-108">Support for these products is limited.</span></span> <span data-ttu-id="43183-109">Se se deparar com problemas ou detetar erros, registe um problema no GitHub.</span><span class="sxs-lookup"><span data-stu-id="43183-109">If you have problems or discover bugs, please file an issue on GitHub.</span></span>
>
> * [<span data-ttu-id="43183-110">Problemas do PowerShell Core v6</span><span class="sxs-lookup"><span data-stu-id="43183-110">Issues for PowerShell Core v6</span></span>](https://github.com/PowerShell/PowerShell/issues)
> * [<span data-ttu-id="43183-111">Problemas do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="43183-111">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core"></a><span data-ttu-id="43183-112">Instalar o PowerShell Core</span><span class="sxs-lookup"><span data-stu-id="43183-112">Install PowerShell Core</span></span>

<span data-ttu-id="43183-113">As instruções de instalação do PowerShell Core são diferentes para o macOS e para a maioria das distribuições do Linux.</span><span class="sxs-lookup"><span data-stu-id="43183-113">The installation instructions for PowerShell Core are different for macOS and most Linux distributions.</span></span>
<span data-ttu-id="43183-114">Pode encontrar instruções detalhadas nos seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="43183-114">Detailed instructions can be found in the following articles:</span></span>

* [<span data-ttu-id="43183-115">Instalar o PowerShell Core no macOS</span><span class="sxs-lookup"><span data-stu-id="43183-115">Install PowerShell Core on macOS</span></span>](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [<span data-ttu-id="43183-116">Instalar o PowerShell Core no Linux</span><span class="sxs-lookup"><span data-stu-id="43183-116">Install PowerShell Core on Linux</span></span>](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a><span data-ttu-id="43183-117">Instalar o Azure PowerShell para o .NET Core</span><span class="sxs-lookup"><span data-stu-id="43183-117">Install Azure PowerShell for .NET Core</span></span>

<span data-ttu-id="43183-118">O PowerShell Core é fornecido com o módulo do PowerShellGet já instalado.</span><span class="sxs-lookup"><span data-stu-id="43183-118">PowerShell Core comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="43183-119">A instalação de módulos no PowerShell exige privilégios elevados, pelo que irá precisar de iniciar a sua sessão como um superutilizador:</span><span class="sxs-lookup"><span data-stu-id="43183-119">Installation of modules in PowerShell requires elevated privileges, so you'll need to start your session as superuser:</span></span>

```bash
sudo pwsh
```

<span data-ttu-id="43183-120">Para instalar o Azure PowerShell, execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="43183-120">To install Azure PowerShell, run the following command:</span></span>

```powershell-interactive
Install-Module AzureRM.NetCore
```

> [!IMPORTANT]
> <span data-ttu-id="43183-121">O módulo `AzureRM` descrito noutros artigos não é criado para o .NET Core e não irá funcionar com o PowerShell Core.</span><span class="sxs-lookup"><span data-stu-id="43183-121">The `AzureRM` module detailed in other articles is not built for .NET Core and will not work with PowerShell Core.</span></span> <span data-ttu-id="43183-122">Tanto `AzureRM` como `AzureRM.NetCore` utilizam os mesmos nomes de cmdlet, pelo que a única diferença é o nome do módulo de rollup e a versão de .NET para a qual são criados.</span><span class="sxs-lookup"><span data-stu-id="43183-122">Both `AzureRM` and `AzureRM.NetCore` use the same cmdlet names, so the only difference is the name of the rollup module and which .NET version they are built against.</span></span>

<span data-ttu-id="43183-123">Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="43183-123">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="43183-124">Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:</span><span class="sxs-lookup"><span data-stu-id="43183-124">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="43183-125">Responda `Yes` ou `Yes to All` para continuar com a instalação.</span><span class="sxs-lookup"><span data-stu-id="43183-125">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

## <a name="sign-in"></a><span data-ttu-id="43183-126">Iniciar sessão</span><span class="sxs-lookup"><span data-stu-id="43183-126">Sign in</span></span>

<span data-ttu-id="43183-127">Para começar a utilizar o Azure PowerShell, precisa de carregar `AzureRM.Netcore` para a sua sessão do PowerShell com o cmdlet [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) e, em seguida, iniciar sessão com as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="43183-127">To start working with Azure PowerShell, you need to load `AzureRM.Netcore` into your PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span> <span data-ttu-id="43183-128">__Não__ precisa de privilégios elevados para importar um módulo.</span><span class="sxs-lookup"><span data-stu-id="43183-128">Importing a module does __not__ require elevated privileges.</span></span>

```powershell-interactive
# Import the module into the PowerShell session
Import-Module AzureRM.Netcore
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="43183-129">Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada.</span><span class="sxs-lookup"><span data-stu-id="43183-129">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="43183-130">A importação automática do módulo `AzureRM` implica configurar um perfil do PowerShell, um processo sobre o qual pode obter mais informações em [Acerca de Perfis](/powershell/module/microsoft.powershell.core/about/about_profiles).</span><span class="sxs-lookup"><span data-stu-id="43183-130">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="43183-131">No macOS e no Linux, deve trabalhar com o seu perfil através da variável de ambiente `$Profile`.</span><span class="sxs-lookup"><span data-stu-id="43183-131">On macOS and Linux, you should work with your profile through the `$Profile` environment variable.</span></span> <span data-ttu-id="43183-132">Para saber como manter o início de sessão do Azure entre as sessões, veja [Manter credenciais do utilizador nas sessões do PowerShell](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="43183-132">To learn how to persist your Azure sign in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="available-cmdlets"></a><span data-ttu-id="43183-133">Cmdlets disponíveis</span><span class="sxs-lookup"><span data-stu-id="43183-133">Available cmdlets</span></span>

<span data-ttu-id="43183-134">Os módulos do Azure PowerShell para o .NET Core ainda estão em desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="43183-134">The Azure PowerShell modules for .NET Core are still in development.</span></span> <span data-ttu-id="43183-135">Estes módulos não fornecem o conjunto completo de cmdlets que estão disponíveis para a versão do Windows dos módulos.</span><span class="sxs-lookup"><span data-stu-id="43183-135">These modules do not provide the full set of cmdlets that are available for the Windows version of the modules.</span></span> <span data-ttu-id="43183-136">As seguintes funções estão implementadas nos módulos AzureRM.Netcore:</span><span class="sxs-lookup"><span data-stu-id="43183-136">The following functions are implemented in AzureRM.Netcore modules:</span></span>

* <span data-ttu-id="43183-137">Gestão de contas</span><span class="sxs-lookup"><span data-stu-id="43183-137">Account management</span></span>
  * <span data-ttu-id="43183-138">Inicie sessão com a Conta Microsoft, a Conta escolar ou profissional, ou o Principal de Serviço através do Microsoft Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="43183-138">Sign in with Microsoft account, Organizational account, or Service Principal through Microsoft Azure Active Directory</span></span>
  * <span data-ttu-id="43183-139">Guarde as Credenciais no disco com o AzureRmContext guardar e carregue as credenciais guardadas com o Import-AzureRmContext</span><span class="sxs-lookup"><span data-stu-id="43183-139">Save Credentials to disk with Save-AzureRmContext and load saved credentials using Import-AzureRmContext</span></span>
* <span data-ttu-id="43183-140">Ambiente</span><span class="sxs-lookup"><span data-stu-id="43183-140">Environment</span></span>
  * <span data-ttu-id="43183-141">Obtenha os diferentes ambientes do Microsoft Azure prontos a utilizar</span><span class="sxs-lookup"><span data-stu-id="43183-141">Get the different out-of-box Microsoft Azure environments</span></span>
  * <span data-ttu-id="43183-142">Adicione/Defina/Remova ambientes personalizados (por exemplo, os ambientes do Azure Stack ou do Windows Azure Pack)</span><span class="sxs-lookup"><span data-stu-id="43183-142">Add/Set/Remove customized environments (like your Azure Stack or Windows Azure Pack environments)</span></span>
* <span data-ttu-id="43183-143">Cmdlets do plano de gestão para os serviços do Azure através das interfaces do Resource Manager e da Gestão do Serviço.</span><span class="sxs-lookup"><span data-stu-id="43183-143">Management plane cmdlets for Azure services using Resource Manager and Service Management interfaces.</span></span>
  * <span data-ttu-id="43183-144">Máquina Virtual</span><span class="sxs-lookup"><span data-stu-id="43183-144">Virtual Machine</span></span>
  * <span data-ttu-id="43183-145">Serviço de Aplicações (Sites)</span><span class="sxs-lookup"><span data-stu-id="43183-145">App Service (Websites)</span></span>
  * <span data-ttu-id="43183-146">SQL Database</span><span class="sxs-lookup"><span data-stu-id="43183-146">SQL Database</span></span>
  * <span data-ttu-id="43183-147">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="43183-147">Storage</span></span>
  * <span data-ttu-id="43183-148">Rede</span><span class="sxs-lookup"><span data-stu-id="43183-148">Network</span></span>

## <a name="next-steps"></a><span data-ttu-id="43183-149">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="43183-149">Next Steps</span></span>

<span data-ttu-id="43183-150">Para obter mais informações sobre como utilizar o Azure PowerShell, veja o artigo [Introdução ao Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="43183-150">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
