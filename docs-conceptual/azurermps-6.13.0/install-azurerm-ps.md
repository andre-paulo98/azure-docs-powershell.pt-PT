---
title: Instalar o Azure PowerShell no Windows com o PowerShellGet
description: Como instalar o Azure PowerShell com o PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/16/2018
ms.openlocfilehash: 616a9e14c3944e3151676d89b8a22e35d8f9d406
ms.sourcegitcommit: 558436c824d9b59731aa9b963cdc8df4dea932e7
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/29/2018
ms.locfileid: "52586433"
---
# <a name="install-azure-powershell-on-windows-with-powershellget"></a><span data-ttu-id="47dee-103">Instalar o Azure PowerShell no Windows com o PowerShellGet</span><span class="sxs-lookup"><span data-stu-id="47dee-103">Install Azure PowerShell on Windows with PowerShellGet</span></span>

<span data-ttu-id="47dee-104">Este artigo explica os passos para instalar os módulos do Azure PowerShell num ambiente do Windows com o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="47dee-104">This article explains the steps to install the Azure PowerShell modules in a Windows environment using PowerShellGet.</span></span> <span data-ttu-id="47dee-105">O PowerShellGet e a gestão do módulo constituem a forma preferencial de instalar o Azure PowerShell, mas se preferir instalar com o Instalador de Plataforma Web ou o pacote MSI, veja [Outros métodos de instalação](other-install.md).</span><span class="sxs-lookup"><span data-stu-id="47dee-105">PowerShellGet and module management is the preferred way to install Azure PowerShell but if you would rather install with the Web Platform Installer or MSI package, see [Other installation methods](other-install.md).</span></span>

<span data-ttu-id="47dee-106">Para obter instruções sobre como instalar o Azure PowerShell noutras plataformas, veja [Instalar e configurar o Azure PowerShell em macOS e Linux](install-azurermps-maclinux.md).</span><span class="sxs-lookup"><span data-stu-id="47dee-106">For instructions to install Azure PowerShell on other platforms, see [Install and configure Azure PowerShell on macOS and Linux](install-azurermps-maclinux.md).</span></span>

<span data-ttu-id="47dee-107">O modelo de implementação clássica do Azure não é suportado por esta versão do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="47dee-107">The Azure classic deployment model is not supported by this version of Azure PowerShell.</span></span> <span data-ttu-id="47dee-108">Para obter suporte para implementações clássicas, siga as instruções indicadas em [Instalar o módulo de Gestão de Serviço do Azure PowerShell](/powershell/azure/servicemanagement/install-azure-ps).</span><span class="sxs-lookup"><span data-stu-id="47dee-108">For support for classic deployments, follow the instructions in [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span>

[!INCLUDE[az-replacing-azurerm](../includes/az-replacing-azurerm.md)]

## <a name="requirements"></a><span data-ttu-id="47dee-109">Requisitos</span><span class="sxs-lookup"><span data-stu-id="47dee-109">Requirements</span></span>

<span data-ttu-id="47dee-110">A partir do Azure PowerShell versão 6.0, o Azure PowerShell requer a versão 5.0 do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="47dee-110">Starting with Azure PowerShell version 6.0, Azure PowerShell requires PowerShell version 5.0.</span></span> <span data-ttu-id="47dee-111">Para verificar a versão do PowerShell em execução na sua máquina, execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="47dee-111">To check the version of PowerShell running on your machine, run the following command:</span></span>

```powershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="47dee-112">Se tem uma versão desatualizada, veja [Atualizar o Windows PowerShell existente](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="47dee-112">If you have an outdated version, see [Upgrading existing Windows PowerShell](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="47dee-113">O módulo descrito neste documento, o AzureRM, utiliza o .NET Framework.</span><span class="sxs-lookup"><span data-stu-id="47dee-113">The module described in this document, AzureRM, uses .NET Framework.</span></span> <span data-ttu-id="47dee-114">Isto torna-o incompatível com o PowerShell 6.0, que utiliza o .NET Core.</span><span class="sxs-lookup"><span data-stu-id="47dee-114">This makes it incompatible with PowerShell 6.0, which uses .NET Core.</span></span> <span data-ttu-id="47dee-115">Se estiver a utilizar o PowerShell 6.0, siga as [instruções de instalação para macOS e Linux](install-azurermps-maclinux.md).</span><span class="sxs-lookup"><span data-stu-id="47dee-115">If you are using PowerShell 6.0, follow the [installation instructions for macOS and Linux](install-azurermps-maclinux.md).</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="47dee-116">Instalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="47dee-116">Install the Azure PowerShell module</span></span>

<span data-ttu-id="47dee-117">Precisa de privilégios elevados para instalar módulos da Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="47dee-117">You need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="47dee-118">Para instalar o Azure PowerShell, execute o seguinte comando numa sessão elevada:</span><span class="sxs-lookup"><span data-stu-id="47dee-118">To install Azure PowerShell, run the following command in an elevated session:</span></span>

```powershell-interactive
Install-Module -Name AzureRM -AllowClobber
```

> [!NOTE]
> <span data-ttu-id="47dee-119">Se tiver uma versão mais antiga do que a 2.8.5.201 do NuGet, será pedido que transfira e instale a versão mais recente do NuGet.</span><span class="sxs-lookup"><span data-stu-id="47dee-119">If you have a version older than 2.8.5.201 of NuGet, you are prompted to download and install the latest version of NuGet.</span></span>

<span data-ttu-id="47dee-120">Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="47dee-120">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="47dee-121">Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:</span><span class="sxs-lookup"><span data-stu-id="47dee-121">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="47dee-122">Responda `Yes` ou `Yes to All` para continuar com a instalação.</span><span class="sxs-lookup"><span data-stu-id="47dee-122">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="47dee-123">O módulo `AzureRM` é um módulo de rollup para os cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="47dee-123">The `AzureRM` module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="47dee-124">A instalação do mesmo transfere todos os módulos disponíveis do Azure Resource Manager e disponibiliza os respetivos cmdlets para utilização.</span><span class="sxs-lookup"><span data-stu-id="47dee-124">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="sign-in"></a><span data-ttu-id="47dee-125">Iniciar sessão</span><span class="sxs-lookup"><span data-stu-id="47dee-125">Sign in</span></span>

<span data-ttu-id="47dee-126">Para começar a trabalhar com o Azure PowerShell, inicie sessão com as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="47dee-126">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

> [!NOTE]
>
> <span data-ttu-id="47dee-127">Se tiver desativado o carregamento automático do módulo, tem de importar o módulo manualmente com `Import-Module AzureRM`.</span><span class="sxs-lookup"><span data-stu-id="47dee-127">If you've disabled module autoloading, you need to manually import the module with `Import-Module AzureRM`.</span></span> <span data-ttu-id="47dee-128">Devido à forma como o módulo está estruturado, esta operação pode demorar alguns segundos.</span><span class="sxs-lookup"><span data-stu-id="47dee-128">Because of the way the module is structured, this can take a few seconds.</span></span>


<span data-ttu-id="47dee-129">Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada.</span><span class="sxs-lookup"><span data-stu-id="47dee-129">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="47dee-130">Para saber como manter o início de sessão do Azure nas sessões do PowerShell, veja [Manter as credenciais do utilizador nas sessões do PowerShell](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="47dee-130">To learn how to persist your Azure sign-in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="47dee-131">Atualizar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="47dee-131">Update the Azure PowerShell module</span></span>

<span data-ttu-id="47dee-132">Pode atualizar a sua instalação do Azure PowerShell ao executar [Update-Module](/powershell/module/powershellget/update-module).</span><span class="sxs-lookup"><span data-stu-id="47dee-132">You can update your Azure PowerShell installation by running [Update-Module](/powershell/module/powershellget/update-module).</span></span> <span data-ttu-id="47dee-133">Este comando __não__ desinstala as versões anteriores.</span><span class="sxs-lookup"><span data-stu-id="47dee-133">This command does __not__ uninstall earlier versions.</span></span>

```powershell-interactive
Update-Module -Name AzureRM
```

<span data-ttu-id="47dee-134">Se pretende remover as versões anteriores do Azure PowerShell do seu sistema, veja [Desinstalar o módulo do Azure PowerShell](uninstall-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="47dee-134">If you want to remove older versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="47dee-135">Utilizar várias versões do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="47dee-135">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="47dee-136">Pode instalar mais de uma versão do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="47dee-136">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="47dee-137">Para verificar se tem várias versões do Azure PowerShell instaladas, utilize o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="47dee-137">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-Module -Name AzureRM -List | select Name,Version
```

<span data-ttu-id="47dee-138">Para remover uma versão do Azure PowerShell, veja [Desinstalar o módulo do Azure PowerShell](uninstall-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="47dee-138">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

<span data-ttu-id="47dee-139">Poderá precisar de mais de uma versão se trabalhar com recursos do Azure Stack no local, executar uma versão mais antiga do Windows ou utilizar o modelo de implementação clássica do Azure.</span><span class="sxs-lookup"><span data-stu-id="47dee-139">You might need more than one version if you work with on-premises Azure Stack resources, run an older version of Windows, or use the Azure classic deployment model.</span></span> <span data-ttu-id="47dee-140">Para instalar uma versão anterior, apresente o argumento `-RequiredVersion` ao instalar.</span><span class="sxs-lookup"><span data-stu-id="47dee-140">To install an older version, provide the `-RequiredVersion` argument when installing.</span></span>

```powershell-interactive
# Install version 2.3.0 of Azure PowerShell
Install-Module -Name AzureRM -RequiredVersion 2.3.0
```

<span data-ttu-id="47dee-141">Ao carregar o módulo do Azure PowerShell, a versão mais recente é carregada por predefinição.</span><span class="sxs-lookup"><span data-stu-id="47dee-141">When loading the Azure PowerShell module the latest version is loaded by default.</span></span> <span data-ttu-id="47dee-142">Para carregar uma versão diferente, apresente o argumento `-RequiredVersion`.</span><span class="sxs-lookup"><span data-stu-id="47dee-142">To load a different version, provide the `-RequiredVersion` argument.</span></span>

```powershell-interactive
# Load version 2.3.0 of Azure PowerShell
Import-Module -Name AzureRM -RequiredVersion 2.3.0
```

## <a name="provide-feedback"></a><span data-ttu-id="47dee-143">Enviar comentários</span><span class="sxs-lookup"><span data-stu-id="47dee-143">Provide feedback</span></span>

<span data-ttu-id="47dee-144">Se encontrar um erro ao utilizar o Azure Powershell, [registe um erro no GitHub](https://github.com/Azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="47dee-144">If you find a bug when using Azure Powershell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="47dee-145">Para enviar comentários a partir da linha de comandos, experimente o cmdlet [Send-Feedback](/powershell/module/azurerm.profile/send-feedback).</span><span class="sxs-lookup"><span data-stu-id="47dee-145">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="47dee-146">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="47dee-146">Next Steps</span></span>

<span data-ttu-id="47dee-147">Para começar a utilizar o Azure PowerShell, veja [Introdução ao Azure PowerShell](get-started-azureps.md) para saber mais sobre o módulo e os respetivos recursos.</span><span class="sxs-lookup"><span data-stu-id="47dee-147">To get started using Azure PowerShell, see [Get Started with Azure PowerShell](get-started-azureps.md) to learn more about the module and its features.</span></span>
