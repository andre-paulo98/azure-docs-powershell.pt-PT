---
title: Instalar e configurar o Azure PowerShell no macOS e Linux | Microsoft Docs
description: "Como instalar e configurar o Azure PowerShell para uma primeira utilização no macOS e Linux."
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 01/12/2018
ms.openlocfilehash: 64a86dfd4af7f3f0a91501e9a096ff190f7100cb
ms.sourcegitcommit: 20af779cd523c758d40e23d60eb989a4ef982d5c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/15/2018
---
# <a name="install-and-configure-azure-powershell-on-macos-and-linux"></a><span data-ttu-id="e60a8-103">Instalar e configurar o Azure PowerShell no macOS e Linux</span><span class="sxs-lookup"><span data-stu-id="e60a8-103">Install and configure Azure PowerShell on macOS and Linux</span></span>

<span data-ttu-id="e60a8-104">Agora, é possível instalar o PowerShell Core v6 e o Azure PowerShell em plataformas não Windows.</span><span class="sxs-lookup"><span data-stu-id="e60a8-104">It is now possible to install PowerShell Core v6 and Azure PowerShell on non-Windows platforms.</span></span>
<span data-ttu-id="e60a8-105">O processo de instalação do Azure PowerShell no macOS e Linux não difere muito do do Windows. No entanto, primeiro tem de instalar o PowerShell Core v6.</span><span class="sxs-lookup"><span data-stu-id="e60a8-105">The process of installing Azure PowerShell on macOS and Linux is not that different from Windows, however, you must first install PowerShell Core v6.</span></span>

> [!NOTE]

> <span data-ttu-id="e60a8-106">Atualmente, tanto o PowerShell Core v6 como o Azure PowerShell para .NET Core ainda se encontram em fase beta.</span><span class="sxs-lookup"><span data-stu-id="e60a8-106">At this time, both PowerShell Core v6 and Azure PowerShell for .NET Core are still in beta.</span></span>
> <span data-ttu-id="e60a8-107">O suporte para estes produtos é limitado.</span><span class="sxs-lookup"><span data-stu-id="e60a8-107">Support for these products is limited.</span></span> <span data-ttu-id="e60a8-108">Se tiver problemas ou detetar erros, envie um relatório para Problemas no GitHub.</span><span class="sxs-lookup"><span data-stu-id="e60a8-108">If you have problems or discover bugs, please file Issues in GitHub.</span></span>
>
> * [<span data-ttu-id="e60a8-109">Problemas do PowerShell Core v6</span><span class="sxs-lookup"><span data-stu-id="e60a8-109">Issues for PowerShell Core v6</span></span>](https://github.com/PowerShell/PowerShell/issues)
> * [<span data-ttu-id="e60a8-110">Problemas do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="e60a8-110">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="step-1-install-powershell-core-v6"></a><span data-ttu-id="e60a8-111">Passo 1: Instalar o PowerShell Core v6</span><span class="sxs-lookup"><span data-stu-id="e60a8-111">Step 1: Install PowerShell Core v6</span></span>

<span data-ttu-id="e60a8-112">O processo de instalação do PowerShell Core v6 varia consoante o sistema operativo de destino.</span><span class="sxs-lookup"><span data-stu-id="e60a8-112">The process of installing PowerShell Core v6 on varies depending on the target operating system.</span></span>
<span data-ttu-id="e60a8-113">Embora seja possível instalar o PowerShell Core v6 no Windows, este artigo incide sobre o macOS e Linux.</span><span class="sxs-lookup"><span data-stu-id="e60a8-113">While it is possible to install PowerShell Core v6 on Windows, this article focuses on macOS and Linux.</span></span> <span data-ttu-id="e60a8-114">Se quiser utilizar o Azure PowerShell no Windows, veja o artigo [instalar](./install-azurerm-ps.md) para o Windows.</span><span class="sxs-lookup"><span data-stu-id="e60a8-114">If you want to use Azure PowerShell on Windows, see the [install](./install-azurerm-ps.md) article for Windows.</span></span>

<span data-ttu-id="e60a8-115">A instalação do **PowerShell Core v6** no Linux ou macOS varia consoante a distribuição do Linux e a versão do SO.</span><span class="sxs-lookup"><span data-stu-id="e60a8-115">Installing **PowerShell Core v6** on Linux or macOS varies depending on the Linux distribution and OS version.</span></span>
<span data-ttu-id="e60a8-116">Pode encontrar instruções detalhadas no seguinte artigo:</span><span class="sxs-lookup"><span data-stu-id="e60a8-116">Detailed instructions can be found in the following article:</span></span>

- [<span data-ttu-id="e60a8-117">Instalar o PowerShell Core no macOS e no Linux</span><span class="sxs-lookup"><span data-stu-id="e60a8-117">Installing PowerShell Core on macOS and Linux</span></span>](/powershell/scripting/setup/installing-powershell-core-on-macos-and-linux)

## <a name="step-2-install-azure-powershell-for-net-core"></a><span data-ttu-id="e60a8-118">Passo 2: Instalar o Azure PowerShell para .NET Core</span><span class="sxs-lookup"><span data-stu-id="e60a8-118">Step 2: Install Azure PowerShell for .NET Core</span></span>

<span data-ttu-id="e60a8-119">O PowerShell Core v6 é fornecido com o módulo PowerShellGet já instalado.</span><span class="sxs-lookup"><span data-stu-id="e60a8-119">PowerShell Core v6 comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="e60a8-120">o que facilita a instalação de qualquer módulo que seja publicado na Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e60a8-120">This makes it easy to install any module that is published to the PowerShell Gallery.</span></span> <span data-ttu-id="e60a8-121">Para instalar o Azure PowerShell, abra uma nova sessão do PowerShell e execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="e60a8-121">To install Azure PowerShell, open a new PowerShell session and run the following command:</span></span>

```powershell
Install-Module AzureRM.NetCore
```

## <a name="step-3-load-the-azurermnetcore-module"></a><span data-ttu-id="e60a8-122">Passo 3: Carregar o módulo AzureRM.Netcore</span><span class="sxs-lookup"><span data-stu-id="e60a8-122">Step 3: Load the AzureRM.Netcore module</span></span>

<span data-ttu-id="e60a8-123">Uma vez que o módulo seja instalado, terá de carregar o módulo para a sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e60a8-123">Once the module is installed, you need to load the module into your PowerShell session.</span></span> <span data-ttu-id="e60a8-124">Os módulos são carregados com o cmdlet `Import-Module`, da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="e60a8-124">Modules are loaded using the `Import-Module` cmdlet, as follows:</span></span>

```powershell
Import-Module AzureRM.Netcore
Import-Module AzureRM.Profile.Netcore
```

<span data-ttu-id="e60a8-125">Quando a importação terminar, pode testar o módulo que acabou de instalar ao tentar iniciar sessão no Azure através do seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="e60a8-125">After the import completes, you can test your newly installed and module by attempting to sign into Azure using the following command:</span></span>

```powershell
Login-AzureRMAccount
```

<span data-ttu-id="e60a8-126">O comando acima deve pedir-lhe para aceder a `https://aka.ms/devicelogin` e introduzir o código fornecido.</span><span class="sxs-lookup"><span data-stu-id="e60a8-126">The above command should prompt you to go to `https://aka.ms/devicelogin` and enter the provided code.</span></span>

## <a name="available-cmdlets"></a><span data-ttu-id="e60a8-127">Cmdlets disponíveis</span><span class="sxs-lookup"><span data-stu-id="e60a8-127">Available cmdlets</span></span>

<span data-ttu-id="e60a8-128">Os módulos do Azure PowerShell para .NET Standard ainda estão em desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="e60a8-128">The Azure PowerShell modules for .NET Standard are still in development.</span></span> <span data-ttu-id="e60a8-129">Estes módulos não fornecem o conjunto completo de cmdlets que estão disponíveis para a versão do Windows dos módulos.</span><span class="sxs-lookup"><span data-stu-id="e60a8-129">These modules do not provide the full set of cmdlets that are available for the Windows version of the modules.</span></span> <span data-ttu-id="e60a8-130">As seguintes funções estão implementadas nos módulos AzureRM.Netcore:</span><span class="sxs-lookup"><span data-stu-id="e60a8-130">The following functions are implemented in AzureRM.Netcore modules:</span></span>

* <span data-ttu-id="e60a8-131">Gestão de contas</span><span class="sxs-lookup"><span data-stu-id="e60a8-131">Account management</span></span>
  - <span data-ttu-id="e60a8-132">Inicie sessão com a conta Microsoft, a conta Organizacional ou o Principal de Serviço através do Microsoft Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="e60a8-132">Login with Microsoft account, Organizational account, or Service Principal through Microsoft Azure Active Directory</span></span>
  - <span data-ttu-id="e60a8-133">Guarde as Credenciais no disco com o AzureRmContext guardar e carregue as credenciais guardadas com o Import-AzureRmContext</span><span class="sxs-lookup"><span data-stu-id="e60a8-133">Save Credentials to disk with Save-AzureRmContext and load saved credentials using Import-AzureRmContext</span></span>
* <span data-ttu-id="e60a8-134">Ambiente</span><span class="sxs-lookup"><span data-stu-id="e60a8-134">Environment</span></span>
  - <span data-ttu-id="e60a8-135">Obtenha os diferentes ambientes do Microsoft Azure prontos a utilizar</span><span class="sxs-lookup"><span data-stu-id="e60a8-135">Get the different out-of-box Microsoft Azure environments</span></span>
  - <span data-ttu-id="e60a8-136">Adicione/Defina/Remova ambientes personalizados (por exemplo, os ambientes do Azure Stack ou do Windows Azure Pack)</span><span class="sxs-lookup"><span data-stu-id="e60a8-136">Add/Set/Remove customized environments (like your Azure Stack or Windows Azure Pack environments)</span></span>
* <span data-ttu-id="e60a8-137">Cmdlets do plano de gestão para os serviços do Azure através das interfaces do Resource Manager e da Gestão do Serviço.</span><span class="sxs-lookup"><span data-stu-id="e60a8-137">Management plane cmdlets for Azure services using Resource Manager and Service Management interfaces.</span></span>
  - <span data-ttu-id="e60a8-138">Máquina Virtual</span><span class="sxs-lookup"><span data-stu-id="e60a8-138">Virtual Machine</span></span>
  - <span data-ttu-id="e60a8-139">Serviço de Aplicações (Sites)</span><span class="sxs-lookup"><span data-stu-id="e60a8-139">App Service (Websites)</span></span>
  - <span data-ttu-id="e60a8-140">SQL Database</span><span class="sxs-lookup"><span data-stu-id="e60a8-140">SQL Database</span></span>
  - <span data-ttu-id="e60a8-141">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e60a8-141">Storage</span></span>
  - <span data-ttu-id="e60a8-142">Rede</span><span class="sxs-lookup"><span data-stu-id="e60a8-142">Network</span></span>

## <a name="next-steps"></a><span data-ttu-id="e60a8-143">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="e60a8-143">Next Steps</span></span>

<span data-ttu-id="e60a8-144">Para obter mais informações sobre como utilizar o Azure PowerShell, veja o artigo [Introdução ao Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="e60a8-144">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
