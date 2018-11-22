---
title: Instalar o Azure PowerShell no Windows com o PowerShellGet
description: Como instalar o Azure PowerShell com o PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/15/2018
ms.openlocfilehash: a868a62bd7bb2f39775a3b7878e2c8484c50438d
ms.sourcegitcommit: 80a3da199954d0ab78765715fb49793e89a30f12
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/22/2018
ms.locfileid: "52258558"
---
# <a name="install-azure-powershell-on-windows-with-powershellget"></a><span data-ttu-id="333d9-103">Instalar o Azure PowerShell no Windows com o PowerShellGet</span><span class="sxs-lookup"><span data-stu-id="333d9-103">Install Azure PowerShell on Windows with PowerShellGet</span></span>

<span data-ttu-id="333d9-104">Este artigo explica os passos para instalar os módulos do Azure PowerShell num ambiente do Windows com o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="333d9-104">This article explains the steps to install the Azure PowerShell modules in a Windows environment using PowerShellGet.</span></span> <span data-ttu-id="333d9-105">O PowerShellGet e a gestão do módulo constituem a forma preferencial de instalar o Azure PowerShell, mas se preferir instalar com o Instalador de Plataforma Web ou o pacote MSI, veja [Outros métodos de instalação](other-install.md).</span><span class="sxs-lookup"><span data-stu-id="333d9-105">PowerShellGet and module management is the preferred way to install Azure PowerShell but if you would rather install with the Web Platform Installer or MSI package, see [Other installation methods](other-install.md).</span></span>

<span data-ttu-id="333d9-106">Para obter instruções sobre como instalar o Azure PowerShell noutras plataformas, veja [Instalar e configurar o Azure PowerShell em macOS e Linux](install-azurermps-maclinux.md).</span><span class="sxs-lookup"><span data-stu-id="333d9-106">For instructions to install Azure PowerShell on other platforms, see [Install and configure Azure PowerShell on macOS and Linux](install-azurermps-maclinux.md).</span></span>

<span data-ttu-id="333d9-107">O modelo de implementação clássica do Azure não é suportado por esta versão do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="333d9-107">The Azure classic deployment model is not supported by this version of Azure PowerShell.</span></span> <span data-ttu-id="333d9-108">Para obter suporte para implementações clássicas, siga as instruções indicadas em [Instalar o módulo de Gestão de Serviço do Azure PowerShell](/powershell/azure/servicemanagement/install-azure-ps).</span><span class="sxs-lookup"><span data-stu-id="333d9-108">For support for classic deployments, follow the instructions in [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span>

## <a name="requirements"></a><span data-ttu-id="333d9-109">Requisitos</span><span class="sxs-lookup"><span data-stu-id="333d9-109">Requirements</span></span>

<span data-ttu-id="333d9-110">Para instalar o Azure PowerShell, precisa do PowerShellGet versão 1.1.2.0 ou superior.</span><span class="sxs-lookup"><span data-stu-id="333d9-110">To install Azure PowerShell, you need PowerShellGet version 1.1.2.0 or higher.</span></span> <span data-ttu-id="333d9-111">Para verificar se está disponível no seu sistema, execute o comando:</span><span class="sxs-lookup"><span data-stu-id="333d9-111">To check if it is available on your system, run the following command:</span></span>

```powershell-interactive
Get-Module -Name PowerShellGet -ListAvailable | Select-Object -Property Name,Version,Path
```

<span data-ttu-id="333d9-112">Deverá ver algo semelhante à saída seguinte:</span><span class="sxs-lookup"><span data-stu-id="333d9-112">You should see something similar to the following output:</span></span>

```output
Name          Version Path
----          ------- ----
Name          Version Path
----          ------- ----
PowerShellGet 1.6.0   C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.6.0\PowerShellGet.psd1
PowerShellGet 1.0.0.1 C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PowerShellGet.psd1
```

<span data-ttu-id="333d9-113">Se precisa de atualizar a sua instalação do PowerShellGet, execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="333d9-113">If you need to update your installation of PowerShellGet, run the following command:</span></span>

```powershell-interactive
Install-Module PowerShellGet -Force
```

<span data-ttu-id="333d9-114">Se não tem o PowerShellGet instalado, siga as instruções na tabela abaixo do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="333d9-114">If you don't have PowerShellGet installed, follow the instructions in the table below for your system.</span></span>

|<span data-ttu-id="333d9-115">Cenário</span><span class="sxs-lookup"><span data-stu-id="333d9-115">Scenario</span></span>|<span data-ttu-id="333d9-116">Instruções de instalação</span><span class="sxs-lookup"><span data-stu-id="333d9-116">Install instructions</span></span>|
|---|---|
|<span data-ttu-id="333d9-117">Windows 10</span><span class="sxs-lookup"><span data-stu-id="333d9-117">Windows 10</span></span><br/><span data-ttu-id="333d9-118">Windows Server 2016</span><span class="sxs-lookup"><span data-stu-id="333d9-118">Windows Server 2016</span></span>|<span data-ttu-id="333d9-119">Incorporado no Windows Management Framework (WMF) 5.0 incluído no SO</span><span class="sxs-lookup"><span data-stu-id="333d9-119">Built into Windows Management Framework (WMF) 5.0 included in the OS</span></span>|
|<span data-ttu-id="333d9-120">Atualizar para o PowerShell 5</span><span class="sxs-lookup"><span data-stu-id="333d9-120">Upgrade to PowerShell 5</span></span>| <ol><li>[<span data-ttu-id="333d9-121">Instalar a versão mais recente do WMF</span><span class="sxs-lookup"><span data-stu-id="333d9-121">Install the latest version of WMF</span></span>](https://www.microsoft.com/en-us/download/details.aspx?id=54616)</li><li><span data-ttu-id="333d9-122">Execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="333d9-122">Run the following command:</span></span><br/>```Install-Module PowerShellGet -Force```</li></ol>|
|<span data-ttu-id="333d9-123">Windows com PowerShell 3 ou PowerShell 4</span><span class="sxs-lookup"><span data-stu-id="333d9-123">Windows with PowerShell 3 or PowerShell 4</span></span>|<ol><span data-ttu-id="333d9-124"><il>[Obter os módulos PackageManagement](http://go.microsoft.com/fwlink/?LinkID=746217)</il></span><span class="sxs-lookup"><span data-stu-id="333d9-124"><il>[Get the PackageManagement modules](http://go.microsoft.com/fwlink/?LinkID=746217)</il></span></span><li><span data-ttu-id="333d9-125">Execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="333d9-125">Run the following command:</span></span><br/>```Install-Module PowerShellGet -Force```</li></ol>|

> [!NOTE]
> <span data-ttu-id="333d9-126">A utilização do PowerShellGet requer uma Política de Execução que lhe permita executar scripts.</span><span class="sxs-lookup"><span data-stu-id="333d9-126">Using PowerShellGet requires an Execution Policy that allows you to run scripts.</span></span> <span data-ttu-id="333d9-127">Para obter mais informações sobre a Política de Execução do PowerShell, veja [About Execution Policies (Sobre as Políticas de Execução)](/powershell/module/microsoft.powershell.core/about/about_execution_policies).</span><span class="sxs-lookup"><span data-stu-id="333d9-127">For more information about PowerShell's Execution Policy, see [About Execution Policies](/powershell/module/microsoft.powershell.core/about/about_execution_policies).</span></span>
>
> [!IMPORTANT]
> <span data-ttu-id="333d9-128">O módulo descrito neste documento, o AzureRM, utiliza o .NET Framework.</span><span class="sxs-lookup"><span data-stu-id="333d9-128">The module described in this document, AzureRM, uses .NET Framework.</span></span> <span data-ttu-id="333d9-129">Isto torna-o incompatível com o PowerShell 6.0, que utiliza o .NET Core.</span><span class="sxs-lookup"><span data-stu-id="333d9-129">This makes it incompatible with PowerShell 6.0, which uses .NET Core.</span></span> <span data-ttu-id="333d9-130">Se estiver a utilizar o PowerShell 6.0, siga as [instruções de instalação para macOS e Linux](install-azurermps-maclinux.md).</span><span class="sxs-lookup"><span data-stu-id="333d9-130">If you are using PowerShell 6.0, follow the [installation instructions for macOS and Linux](install-azurermps-maclinux.md).</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="333d9-131">Instalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="333d9-131">Install the Azure PowerShell module</span></span>

<span data-ttu-id="333d9-132">Precisa de privilégios elevados para instalar módulos da Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="333d9-132">You need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="333d9-133">Para instalar o Azure PowerShell, execute o seguinte comando numa sessão elevada:</span><span class="sxs-lookup"><span data-stu-id="333d9-133">To install Azure PowerShell, run the following command in an elevated session:</span></span>

```powershell-interactive
Install-Module -Name AzureRM
```

> [!NOTE]
> <span data-ttu-id="333d9-134">Se tiver uma versão mais antiga do que a 2.8.5.201 do NuGet, será pedido que transfira e instale a versão mais recente do NuGet.</span><span class="sxs-lookup"><span data-stu-id="333d9-134">If you have a version older than 2.8.5.201 of NuGet, you are prompted to download and install the latest version of NuGet.</span></span>

<span data-ttu-id="333d9-135">Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="333d9-135">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="333d9-136">Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:</span><span class="sxs-lookup"><span data-stu-id="333d9-136">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="333d9-137">Responda `Yes` ou `Yes to All` para continuar com a instalação.</span><span class="sxs-lookup"><span data-stu-id="333d9-137">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="333d9-138">O módulo `AzureRM` é um módulo de rollup para os cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="333d9-138">The `AzureRM` module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="333d9-139">A instalação do mesmo transfere todos os módulos disponíveis do Azure Resource Manager e disponibiliza os respetivos cmdlets para utilização.</span><span class="sxs-lookup"><span data-stu-id="333d9-139">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="sign-in"></a><span data-ttu-id="333d9-140">Iniciar sessão</span><span class="sxs-lookup"><span data-stu-id="333d9-140">Sign in</span></span>

<span data-ttu-id="333d9-141">Para começar a utilizar o Azure PowerShell, precisa de carregar `AzureRM` para a sua sessão atual do PowerShell com o cmdlet [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) e, em seguida, iniciar sessão com as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="333d9-141">To start working with Azure PowerShell, you need to load `AzureRM` into your current PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span>

```powershell-interactive
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="333d9-142">Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada.</span><span class="sxs-lookup"><span data-stu-id="333d9-142">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="333d9-143">A importação automática do módulo `AzureRM` implica configurar um perfil do PowerShell, um processo sobre o qual pode obter mais informações em [Acerca de Perfis](/powershell/module/microsoft.powershell.core/about/about_profiles).</span><span class="sxs-lookup"><span data-stu-id="333d9-143">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="333d9-144">Para saber como manter o início de sessão do Azure entre as sessões, veja [Manter credenciais do utilizador nas sessões do PowerShell](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="333d9-144">To learn how to persist your Azure sign in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="333d9-145">Atualizar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="333d9-145">Update the Azure PowerShell module</span></span>

<span data-ttu-id="333d9-146">Pode atualizar a sua instalação do Azure PowerShell ao executar [Update-Module](/powershell/module/powershellget/update-module).</span><span class="sxs-lookup"><span data-stu-id="333d9-146">You can update your Azure PowerShell installation by running [Update-Module](/powershell/module/powershellget/update-module).</span></span> <span data-ttu-id="333d9-147">Este comando __não__ desinstala as versões anteriores.</span><span class="sxs-lookup"><span data-stu-id="333d9-147">This command does __not__ uninstall earlier versions.</span></span>

```powershell-interactive
Update-Module -Name AzureRM
```

<span data-ttu-id="333d9-148">Se pretende remover as versões anteriores do Azure PowerShell do seu sistema, veja [Desinstalar o módulo do Azure PowerShell](uninstall-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="333d9-148">If you want to remove older versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="333d9-149">Utilizar várias versões do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="333d9-149">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="333d9-150">Pode instalar várias versões do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="333d9-150">It's possible to install multiple versions of Azure PowerShell.</span></span> <span data-ttu-id="333d9-151">Poderá precisar de mais de uma versão se trabalhar com recursos do Azure Stack no local, executar uma versão mais antiga do Windows que não pode atualizar para o PowerShell 5.0 ou utilizar o modelo de implementação clássica do Azure.</span><span class="sxs-lookup"><span data-stu-id="333d9-151">You might need more than one version if you work with on-premises Azure Stack resources, run an older version of Windows that you can't update to PowerShell 5.0, or use the Azure classic deployment model.</span></span> <span data-ttu-id="333d9-152">Para instalar uma versão anterior, apresente o argumento `-RequiredVersion` ao instalar.</span><span class="sxs-lookup"><span data-stu-id="333d9-152">To install an older version, provide the `-RequiredVersion` argument when installing.</span></span>

```powershell-interactive
# Install version 1.2.9 of Azure PowerShell
Install-Module -Name AzureRM -RequiredVersion 1.2.9
```

<span data-ttu-id="333d9-153">Ao carregar o módulo do Azure PowerShell, a versão mais recente é carregada por predefinição.</span><span class="sxs-lookup"><span data-stu-id="333d9-153">When loading the Azure PowerShell module the latest version is loaded by default.</span></span> <span data-ttu-id="333d9-154">Para carregar uma versão diferente, apresente o argumento `-RequiredVersion`.</span><span class="sxs-lookup"><span data-stu-id="333d9-154">To load a different version, provide the `-RequiredVersion` argument.</span></span>

```powershell-interactive
# Load version 1.2.9 of Azure PowerShell
Import-Module -Name AzureRM -RequiredVersion 1.2.9
```

## <a name="provide-feedback"></a><span data-ttu-id="333d9-155">Enviar comentários</span><span class="sxs-lookup"><span data-stu-id="333d9-155">Provide feedback</span></span>

<span data-ttu-id="333d9-156">Se encontrar um erro ao utilizar o Azure Powershell, [registe um erro no GitHub](https://github.com/Azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="333d9-156">If you find a bug when using Azure Powershell, please [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="333d9-157">Para enviar comentários a partir da linha de comandos, experimente o cmdlet [Send-Feedback](/powershell/module/azurerm.profile/send-feedback).</span><span class="sxs-lookup"><span data-stu-id="333d9-157">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="333d9-158">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="333d9-158">Next Steps</span></span>

<span data-ttu-id="333d9-159">Para começar a utilizar o Azure PowerShell, veja [Introdução ao Azure PowerShell](get-started-azureps.md) para saber mais sobre o módulo e os respetivos recursos.</span><span class="sxs-lookup"><span data-stu-id="333d9-159">To get started using Azure PowerShell, see [Get Started with Azure PowerShell](get-started-azureps.md) to learn more about the module and its features.</span></span>