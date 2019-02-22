---
title: Instalar o Azure PowerShell no macOS ou Linux
description: Como instalar o Azure PowerShell no macOS ou Linux.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 936bb24eecb4077080e172bf0d29fe57ec652187
ms.sourcegitcommit: 2054a8f74cd9bf5a50ea7fdfddccaa632c842934
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "56153693"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a><span data-ttu-id="292c1-103">Instalar o Azure PowerShell no macOS ou Linux</span><span class="sxs-lookup"><span data-stu-id="292c1-103">Install Azure PowerShell on macOS or Linux</span></span>

<span data-ttu-id="292c1-104">É possível executar o Azure PowerShell no PowerShell Core v6 em plataformas não Windows.</span><span class="sxs-lookup"><span data-stu-id="292c1-104">For non-Windows platforms, it's possible to run Azure PowerShell in PowerShell Core v6.</span></span> <span data-ttu-id="292c1-105">Esta versão do PowerShell foi concebida para ser utilizada em qualquer plataforma que suporte o .NET Core.</span><span class="sxs-lookup"><span data-stu-id="292c1-105">This version of PowerShell is built for use on any platform that supports .NET Core.</span></span> <span data-ttu-id="292c1-106">Para trabalhar com estas plataformas, existe uma versão especial do Azure PowerShell disponível para o .NET Core.</span><span class="sxs-lookup"><span data-stu-id="292c1-106">To work with these platforms, there's a special .NET Core version of Azure PowerShell available.</span></span>

[!INCLUDE[az-replacing-azurerm.md](../includes/az-replacing-azurerm.md)]

## <a name="install-powershell-core"></a><span data-ttu-id="292c1-107">Instalar o PowerShell Core</span><span class="sxs-lookup"><span data-stu-id="292c1-107">Install PowerShell Core</span></span>

<span data-ttu-id="292c1-108">As instruções de instalação do PowerShell Core são diferentes para o macOS e para a maioria das distribuições do Linux.</span><span class="sxs-lookup"><span data-stu-id="292c1-108">The installation instructions for PowerShell Core are different for macOS and most Linux distributions.</span></span>
<span data-ttu-id="292c1-109">Pode encontrar instruções detalhadas nos seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="292c1-109">Detailed instructions can be found in the following articles:</span></span>

* [<span data-ttu-id="292c1-110">Instalar o PowerShell Core no macOS</span><span class="sxs-lookup"><span data-stu-id="292c1-110">Install PowerShell Core on macOS</span></span>](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [<span data-ttu-id="292c1-111">Instalar o PowerShell Core no Linux</span><span class="sxs-lookup"><span data-stu-id="292c1-111">Install PowerShell Core on Linux</span></span>](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a><span data-ttu-id="292c1-112">Instalar o Azure PowerShell para o .NET Core</span><span class="sxs-lookup"><span data-stu-id="292c1-112">Install Azure PowerShell for .NET Core</span></span>

<span data-ttu-id="292c1-113">O PowerShell Core é fornecido com o módulo do PowerShellGet já instalado.</span><span class="sxs-lookup"><span data-stu-id="292c1-113">PowerShell Core comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="292c1-114">A instalação de módulos no PowerShell exige privilégios elevados, pelo que irá precisar de iniciar a sua sessão como um superutilizador:</span><span class="sxs-lookup"><span data-stu-id="292c1-114">Installation of modules in PowerShell requires elevated privileges, so you'll need to start your session as superuser:</span></span>

```bash
sudo pwsh
```

<span data-ttu-id="292c1-115">Para instalar o Azure PowerShell, execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="292c1-115">To install Azure PowerShell, run the following command:</span></span>

```powershell-interactive
Install-Module AzureRM.NetCore
```

> [!IMPORTANT]
> <span data-ttu-id="292c1-116">O módulo `AzureRM` descrito noutros artigos não é criado para o .NET Core e não irá funcionar com o PowerShell Core.</span><span class="sxs-lookup"><span data-stu-id="292c1-116">The `AzureRM` module detailed in other articles is not built for .NET Core and will not work with PowerShell Core.</span></span> <span data-ttu-id="292c1-117">Tanto `AzureRM` como `AzureRM.NetCore` utilizam os mesmos nomes de cmdlet, pelo que a única diferença é o nome do módulo de rollup e a versão de .NET para a qual são criados.</span><span class="sxs-lookup"><span data-stu-id="292c1-117">Both `AzureRM` and `AzureRM.NetCore` use the same cmdlet names, so the only difference is the name of the rollup module and which .NET version they are built against.</span></span>

<span data-ttu-id="292c1-118">Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="292c1-118">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="292c1-119">Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:</span><span class="sxs-lookup"><span data-stu-id="292c1-119">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="292c1-120">Responda `Yes` ou `Yes to All` para continuar com a instalação.</span><span class="sxs-lookup"><span data-stu-id="292c1-120">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

## <a name="sign-in"></a><span data-ttu-id="292c1-121">Iniciar sessão</span><span class="sxs-lookup"><span data-stu-id="292c1-121">Sign in</span></span>

<span data-ttu-id="292c1-122">Para começar a utilizar o Azure PowerShell, precisa de carregar `AzureRM.Netcore` para a sua sessão do PowerShell com o cmdlet [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) e, em seguida, iniciar sessão com as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="292c1-122">To start working with Azure PowerShell, you need to load `AzureRM.Netcore` into your PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span> <span data-ttu-id="292c1-123">__Não__ precisa de privilégios elevados para importar um módulo.</span><span class="sxs-lookup"><span data-stu-id="292c1-123">Importing a module does __not__ require elevated privileges.</span></span>

```powershell-interactive
# Import the module into the PowerShell session
Import-Module AzureRM.Netcore
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="292c1-124">Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada.</span><span class="sxs-lookup"><span data-stu-id="292c1-124">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="292c1-125">A importação automática do módulo `AzureRM` implica configurar um perfil do PowerShell, um processo sobre o qual pode obter mais informações em [Acerca de Perfis](/powershell/module/microsoft.powershell.core/about/about_profiles).</span><span class="sxs-lookup"><span data-stu-id="292c1-125">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="292c1-126">No macOS e no Linux, deve trabalhar com o seu perfil através da variável de ambiente `$Profile`.</span><span class="sxs-lookup"><span data-stu-id="292c1-126">On macOS and Linux, you should work with your profile through the `$Profile` environment variable.</span></span> <span data-ttu-id="292c1-127">Para saber como manter o início de sessão do Azure entre as sessões, veja [Manter credenciais do utilizador nas sessões do PowerShell](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="292c1-127">To learn how to persist your Azure sign in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="available-cmdlets"></a><span data-ttu-id="292c1-128">Cmdlets disponíveis</span><span class="sxs-lookup"><span data-stu-id="292c1-128">Available cmdlets</span></span>

<span data-ttu-id="292c1-129">Os módulos do Azure PowerShell para o .NET Core ainda estão em desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="292c1-129">The Azure PowerShell modules for .NET Core are still in development.</span></span> <span data-ttu-id="292c1-130">Estes módulos não fornecem o conjunto completo de cmdlets que estão disponíveis para a versão do Windows dos módulos.</span><span class="sxs-lookup"><span data-stu-id="292c1-130">These modules do not provide the full set of cmdlets that are available for the Windows version of the modules.</span></span> <span data-ttu-id="292c1-131">As seguintes funções estão implementadas nos módulos AzureRM.Netcore:</span><span class="sxs-lookup"><span data-stu-id="292c1-131">The following functions are implemented in AzureRM.Netcore modules:</span></span>

* <span data-ttu-id="292c1-132">Gestão de contas</span><span class="sxs-lookup"><span data-stu-id="292c1-132">Account management</span></span>
  * <span data-ttu-id="292c1-133">Inicie sessão com a Conta Microsoft, a Conta escolar ou profissional, ou o Principal de Serviço através do Microsoft Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="292c1-133">Sign in with Microsoft account, Organizational account, or Service Principal through Microsoft Azure Active Directory</span></span>
  * <span data-ttu-id="292c1-134">Guarde as Credenciais no disco com o AzureRmContext guardar e carregue as credenciais guardadas com o Import-AzureRmContext</span><span class="sxs-lookup"><span data-stu-id="292c1-134">Save Credentials to disk with Save-AzureRmContext and load saved credentials using Import-AzureRmContext</span></span>
* <span data-ttu-id="292c1-135">Ambiente</span><span class="sxs-lookup"><span data-stu-id="292c1-135">Environment</span></span>
  * <span data-ttu-id="292c1-136">Obtenha os diferentes ambientes do Microsoft Azure prontos a utilizar</span><span class="sxs-lookup"><span data-stu-id="292c1-136">Get the different out-of-box Microsoft Azure environments</span></span>
  * <span data-ttu-id="292c1-137">Adicione/Defina/Remova ambientes personalizados (por exemplo, os ambientes do Azure Stack ou do Windows Azure Pack)</span><span class="sxs-lookup"><span data-stu-id="292c1-137">Add/Set/Remove customized environments (like your Azure Stack or Windows Azure Pack environments)</span></span>
* <span data-ttu-id="292c1-138">Cmdlets do plano de gestão para os serviços do Azure através das interfaces do Resource Manager e da Gestão do Serviço.</span><span class="sxs-lookup"><span data-stu-id="292c1-138">Management plane cmdlets for Azure services using Resource Manager and Service Management interfaces.</span></span>
  * <span data-ttu-id="292c1-139">Máquina Virtual</span><span class="sxs-lookup"><span data-stu-id="292c1-139">Virtual Machine</span></span>
  * <span data-ttu-id="292c1-140">Serviço de Aplicações (Sites)</span><span class="sxs-lookup"><span data-stu-id="292c1-140">App Service (Websites)</span></span>
  * <span data-ttu-id="292c1-141">SQL Database</span><span class="sxs-lookup"><span data-stu-id="292c1-141">SQL Database</span></span>
  * <span data-ttu-id="292c1-142">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="292c1-142">Storage</span></span>
  * <span data-ttu-id="292c1-143">Rede</span><span class="sxs-lookup"><span data-stu-id="292c1-143">Network</span></span>

## <a name="next-steps"></a><span data-ttu-id="292c1-144">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="292c1-144">Next Steps</span></span>

<span data-ttu-id="292c1-145">Para obter mais informações sobre como utilizar o Azure PowerShell, veja o artigo [Introdução ao Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="292c1-145">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
