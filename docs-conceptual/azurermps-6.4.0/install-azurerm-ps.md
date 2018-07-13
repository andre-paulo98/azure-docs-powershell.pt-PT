---
title: Instalar o Azure PowerShell no Windows com o PowerShellGet
description: Como instalar o Azure PowerShell com o PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/15/2018
ms.openlocfilehash: 0d8019a7acaf2ba3baaa0772a76285ec497c991c
ms.sourcegitcommit: de0e60800df1add9f3400166faacca202ef567d9
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/03/2018
ms.locfileid: "37406564"
---
# <a name="install-azure-powershell-on-windows-with-powershellget"></a><span data-ttu-id="5ce3f-103">Instalar o Azure PowerShell no Windows com o PowerShellGet</span><span class="sxs-lookup"><span data-stu-id="5ce3f-103">Install Azure PowerShell on Windows with PowerShellGet</span></span>

<span data-ttu-id="5ce3f-104">Este artigo explica os passos para instalar os módulos do Azure PowerShell num ambiente do Windows com o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="5ce3f-104">This article explains the steps to install the Azure PowerShell modules in a Windows environment using PowerShellGet.</span></span> <span data-ttu-id="5ce3f-105">O PowerShellGet e a gestão do módulo constituem a forma preferencial de instalar o Azure PowerShell, mas se preferir instalar com o Instalador de Plataforma Web ou o pacote MSI, veja [Outros métodos de instalação](other-install.md).</span><span class="sxs-lookup"><span data-stu-id="5ce3f-105">PowerShellGet and module management is the preferred way to install Azure PowerShell but if you would rather install with the Web Platform Installer or MSI package, see [Other installation methods](other-install.md).</span></span>

<span data-ttu-id="5ce3f-106">Para obter instruções sobre como instalar o Azure PowerShell noutras plataformas, veja [Instalar e configurar o Azure PowerShell em macOS e Linux](install-azurermps-maclinux.md).</span><span class="sxs-lookup"><span data-stu-id="5ce3f-106">For instructions to install Azure PowerShell on other platforms, see [Install and configure Azure PowerShell on macOS and Linux](install-azurermps-maclinux.md).</span></span>

<span data-ttu-id="5ce3f-107">O modelo de implementação clássica do Azure não é suportado por esta versão do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5ce3f-107">The Azure classic deployment model is not supported by this version of Azure PowerShell.</span></span> <span data-ttu-id="5ce3f-108">Para obter suporte para implementações clássicas, siga as instruções indicadas em [Instalar o módulo de Gestão de Serviço do Azure PowerShell](/powershell/azure/servicemanagement/install-azure-ps).</span><span class="sxs-lookup"><span data-stu-id="5ce3f-108">For support for classic deployments, follow the instructions in [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span>

## <a name="requirements"></a><span data-ttu-id="5ce3f-109">Requisitos</span><span class="sxs-lookup"><span data-stu-id="5ce3f-109">Requirements</span></span>

<span data-ttu-id="5ce3f-110">A partir da versão 6.0, o Azure PowerShell exige a versão 5.0 ou superior do PowerShell em execução no Windows.</span><span class="sxs-lookup"><span data-stu-id="5ce3f-110">Starting with version 6.0, Azure PowerShell requires version 5.0 or higher of PowerShell running on Windows.</span></span> <span data-ttu-id="5ce3f-111">Para verificar a versão do PowerShell em execução na sua máquina, execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="5ce3f-111">To check the version of PowerShell running on your machine, run the following command:</span></span>

```powershell
$PSVersionTable.PSVersion
```

<span data-ttu-id="5ce3f-112">Se tem uma versão desatualizada, veja [Atualizar o Windows PowerShell existente](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="5ce3f-112">If you have an outdated version, see [Upgrading existing Windows PowerShell](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell).</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="5ce3f-113">Instalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="5ce3f-113">Install the Azure PowerShell module</span></span>

<span data-ttu-id="5ce3f-114">Precisa de privilégios elevados para instalar módulos da Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5ce3f-114">You need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="5ce3f-115">Para instalar o Azure PowerShell, execute o seguinte comando numa sessão elevada:</span><span class="sxs-lookup"><span data-stu-id="5ce3f-115">To install Azure PowerShell, run the following command in an elevated session:</span></span>

```powershell
Install-Module -Name AzureRM
```

> [!NOTE]
> <span data-ttu-id="5ce3f-116">Se tiver uma versão mais antiga do que a 2.8.5.201 do NuGet, será pedido que transfira e instale a versão mais recente do NuGet.</span><span class="sxs-lookup"><span data-stu-id="5ce3f-116">If you have a version older than 2.8.5.201 of NuGet, you are prompted to download and install the latest version of NuGet.</span></span>

<span data-ttu-id="5ce3f-117">Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="5ce3f-117">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="5ce3f-118">Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:</span><span class="sxs-lookup"><span data-stu-id="5ce3f-118">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="5ce3f-119">Responda `Yes` ou `Yes to All` para continuar com a instalação.</span><span class="sxs-lookup"><span data-stu-id="5ce3f-119">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="5ce3f-120">O módulo `AzureRM` é um módulo de rollup para os cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5ce3f-120">The `AzureRM` module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="5ce3f-121">A instalação do mesmo transfere todos os módulos disponíveis do Azure Resource Manager e disponibiliza os respetivos cmdlets para utilização.</span><span class="sxs-lookup"><span data-stu-id="5ce3f-121">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="sign-in"></a><span data-ttu-id="5ce3f-122">Iniciar sessão</span><span class="sxs-lookup"><span data-stu-id="5ce3f-122">Sign in</span></span>

<span data-ttu-id="5ce3f-123">Para começar a utilizar o Azure PowerShell, precisa de carregar `AzureRM` para a sua sessão atual do PowerShell com o cmdlet [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) e, em seguida, iniciar sessão com as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="5ce3f-123">To start working with Azure PowerShell, you need to load `AzureRM` into your current PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span>

```powershell
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="5ce3f-124">Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada.</span><span class="sxs-lookup"><span data-stu-id="5ce3f-124">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="5ce3f-125">A importação automática do módulo `AzureRM` implica configurar um perfil do PowerShell, um processo sobre o qual pode obter mais informações em [Acerca de Perfis](/powershell/module/microsoft.powershell.core/about/about_profiles).</span><span class="sxs-lookup"><span data-stu-id="5ce3f-125">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="5ce3f-126">Para saber como manter o início de sessão do Azure entre as sessões, veja [Manter credenciais do utilizador nas sessões do PowerShell](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="5ce3f-126">To learn how to persist your Azure sign in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="5ce3f-127">Atualizar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="5ce3f-127">Update the Azure PowerShell module</span></span>

<span data-ttu-id="5ce3f-128">Pode atualizar a sua instalação do Azure PowerShell ao executar [Update-Module](/powershell/module/powershellget/update-module).</span><span class="sxs-lookup"><span data-stu-id="5ce3f-128">You can update your Azure PowerShell installation by running [Update-Module](/powershell/module/powershellget/update-module).</span></span> <span data-ttu-id="5ce3f-129">Este comando __não__ desinstala as versões anteriores.</span><span class="sxs-lookup"><span data-stu-id="5ce3f-129">This command does __not__ uninstall earlier versions.</span></span>

```powershell
Update-Module -Name AzureRM
```

<span data-ttu-id="5ce3f-130">Se pretende remover as versões anteriores do Azure PowerShell do seu sistema, veja [Desinstalar o módulo do Azure PowerShell](uninstall-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="5ce3f-130">If you want to remove older versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="5ce3f-131">Utilizar várias versões do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="5ce3f-131">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="5ce3f-132">Pode instalar várias versões do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5ce3f-132">It's possible to install multiple versions of Azure PowerShell.</span></span> <span data-ttu-id="5ce3f-133">Poderá precisar de mais de uma versão se trabalhar com recursos do Azure Stack no local, executar uma versão mais antiga do Windows que não pode atualizar para o PowerShell 5.0 ou utilizar o modelo de implementação clássica do Azure.</span><span class="sxs-lookup"><span data-stu-id="5ce3f-133">You might need more than one version if you work with on-premises Azure Stack resources, run an older version of Windows that you can't update to PowerShell 5.0, or use the Azure classic deployment model.</span></span> <span data-ttu-id="5ce3f-134">Para instalar uma versão anterior, apresente o argumento `-RequiredVersion` ao instalar.</span><span class="sxs-lookup"><span data-stu-id="5ce3f-134">To install an older version, provide the `-RequiredVersion` argument when installing.</span></span>

```powershell
# Install version 1.2.9 of Azure PowerShell
Install-Module -Name AzureRM -RequiredVersion 1.2.9
```

<span data-ttu-id="5ce3f-135">Ao carregar o módulo do Azure PowerShell, a versão mais recente é carregada por predefinição.</span><span class="sxs-lookup"><span data-stu-id="5ce3f-135">When loading the Azure PowerShell module the latest version is loaded by default.</span></span> <span data-ttu-id="5ce3f-136">Para carregar uma versão diferente, apresente o argumento `-RequiredVersion`.</span><span class="sxs-lookup"><span data-stu-id="5ce3f-136">To load a different version, provide the `-RequiredVersion` argument.</span></span>

```powershell
# Load version 1.2.9 of Azure PowerShell
Import-Module -Name AzureRM -RequiredVersion 1.2.9
```

## <a name="provide-feedback"></a><span data-ttu-id="5ce3f-137">Enviar comentários</span><span class="sxs-lookup"><span data-stu-id="5ce3f-137">Provide feedback</span></span>

<span data-ttu-id="5ce3f-138">Se encontrar um erro ao utilizar o Azure Powershell, [registe um erro no GitHub](https://github.com/Azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="5ce3f-138">If you find a bug when using Azure Powershell, please [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="5ce3f-139">Para enviar comentários a partir da linha de comandos, experimente o cmdlet [Send-Feedback](/powershell/module/azurerm.profile/send-feedback).</span><span class="sxs-lookup"><span data-stu-id="5ce3f-139">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5ce3f-140">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="5ce3f-140">Next Steps</span></span>

<span data-ttu-id="5ce3f-141">Para começar a utilizar o Azure PowerShell, veja [Introdução ao Azure PowerShell](get-started-azureps.md) para saber mais sobre o módulo e os respetivos recursos.</span><span class="sxs-lookup"><span data-stu-id="5ce3f-141">To get started using Azure PowerShell, see [Get Started with Azure PowerShell](get-started-azureps.md) to learn more about the module and its features.</span></span>