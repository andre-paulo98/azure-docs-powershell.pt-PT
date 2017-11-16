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
ms.date: 09/06/2017
ms.openlocfilehash: 94b39c18acaca7a4b17b5207feed025442665acc
ms.sourcegitcommit: 358d260a867c6ee2e8700b91f776ba4f1b0e24a5
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/11/2017
---
# <a name="install-and-configure-azure-powershell-on-macos-and-linux"></a><span data-ttu-id="129d5-103">Instalar e configurar o Azure PowerShell no macOS e Linux</span><span class="sxs-lookup"><span data-stu-id="129d5-103">Install and configure Azure PowerShell on macOS and Linux</span></span>

<span data-ttu-id="129d5-104">Agora, é possível instalar o PowerShell 6 (beta) e o Azure PowerShell em plataformas não Windows.</span><span class="sxs-lookup"><span data-stu-id="129d5-104">It is now possible to install PowerShell 6 (beta) and Azure PowerShell on non-Windows platforms.</span></span>
<span data-ttu-id="129d5-105">O processo de instalação do Azure PowerShell no macOS e Linux não difere muito do do Windows. No entanto, primeiro, tem de instalar o PowerShell 6 (beta).</span><span class="sxs-lookup"><span data-stu-id="129d5-105">The process of installing Azure PowerShell on macOS and Linux is not that different from Windows, however, you must first install PowerShell 6 (beta).</span></span>

> [!NOTE]

> <span data-ttu-id="129d5-106">Atualmente, tanto o PowerShell 6 (beta) como o Azure PowerShell para .NET Core ainda se encontram em fase beta.</span><span class="sxs-lookup"><span data-stu-id="129d5-106">At this time, both PowerShell 6 (beta) and Azure PowerShell for .NET Core are still in beta.</span></span>
> <span data-ttu-id="129d5-107">O suporte para estes produtos é limitado.</span><span class="sxs-lookup"><span data-stu-id="129d5-107">Support for these products is limited.</span></span> <span data-ttu-id="129d5-108">Se tiver problemas ou detetar erros, envie um relatório para Problemas no GitHub.</span><span class="sxs-lookup"><span data-stu-id="129d5-108">If you have problems or discover bugs, please file Issues in GitHub.</span></span>
>
> * [<span data-ttu-id="129d5-109">Problemas do PowerShell 6 (beta)</span><span class="sxs-lookup"><span data-stu-id="129d5-109">Issues for PowerShell 6 (beta)</span></span>](https://github.com/PowerShell/PowerShell/issues)
> * [<span data-ttu-id="129d5-110">Problemas do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="129d5-110">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="step-1-install-powershell-6-beta"></a><span data-ttu-id="129d5-111">Passo 1: Instalar o PowerShell 6 (beta)</span><span class="sxs-lookup"><span data-stu-id="129d5-111">Step 1: Install PowerShell 6 (beta)</span></span>

<span data-ttu-id="129d5-112">O processo de instalação do PowerShell 6 (beta) varia consoante o sistema operativo de destino.</span><span class="sxs-lookup"><span data-stu-id="129d5-112">The process of installing PowerShell 6 (beta) on varies depending on the target operating system.</span></span>
<span data-ttu-id="129d5-113">Embora seja possível instalar o PowerShell 6 (beta) no Windows, este artigo incide sobre o macOS e Linux.</span><span class="sxs-lookup"><span data-stu-id="129d5-113">While it is possible to install PowerShell 6 (beta) on Windows, this article focuses on macOS and Linux.</span></span> <span data-ttu-id="129d5-114">Se quiser utilizar o Azure PowerShell no Windows, veja o artigo [instalar](./install-azurerm-ps.md) para o Windows.</span><span class="sxs-lookup"><span data-stu-id="129d5-114">If you want to use Azure PowerShell on Windows, see the [install](./install-azurerm-ps.md) article for Windows.</span></span>

<span data-ttu-id="129d5-115">Para instalar o **PowerShell 6** (beta) no Linux ou macOS, tem de:</span><span class="sxs-lookup"><span data-stu-id="129d5-115">To install **PowerShell 6** (beta) on Linux or macOS, you need to:</span></span>

1. <span data-ttu-id="129d5-116">Obter o PowerShell para o SO e versão específicos a partir do [GitHub](https://github.com/powershell/powershell#get-powershell)</span><span class="sxs-lookup"><span data-stu-id="129d5-116">Get PowerShell for the specific OS and version, from [GitHub](https://github.com/powershell/powershell#get-powershell)</span></span>
2. <span data-ttu-id="129d5-117">Seguir as instruções de instalação</span><span class="sxs-lookup"><span data-stu-id="129d5-117">Follow the installation instructions</span></span>
   - [<span data-ttu-id="129d5-118">Linux</span><span class="sxs-lookup"><span data-stu-id="129d5-118">Linux</span></span>](https://github.com/PowerShell/PowerShell/blob/master/docs/installation/linux.md)
   - [<span data-ttu-id="129d5-119">macOS</span><span class="sxs-lookup"><span data-stu-id="129d5-119">macOS</span></span>](https://github.com/PowerShell/PowerShell/blob/master/docs/installation/linux.md#macos-1012)

## <a name="step-2-install-azure-powershell-for-net-core"></a><span data-ttu-id="129d5-120">Passo 2: Instalar o Azure PowerShell para .NET Core</span><span class="sxs-lookup"><span data-stu-id="129d5-120">Step 2: Install Azure PowerShell for .NET Core</span></span>

<span data-ttu-id="129d5-121">O PowerShell 6 (beta) vem com o módulo PowerShellGet já instalado,</span><span class="sxs-lookup"><span data-stu-id="129d5-121">PowerShell 6 (beta) comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="129d5-122">o que facilita a instalação de qualquer módulo que seja publicado na Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="129d5-122">This makes it easy to install any module that is published to the PowerShell Gallery.</span></span> <span data-ttu-id="129d5-123">Para instalar o Azure PowerShell, abra uma nova sessão do PowerShell e execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="129d5-123">To install Azure PowerShell, open a new PowerShell session and run the following command:</span></span>

```powershell
Install-Module AzureRM.NetCore
```

## <a name="step-3-load-the-azurermnetcore-module"></a><span data-ttu-id="129d5-124">Passo 3: Carregar o módulo AzureRM.Netcore</span><span class="sxs-lookup"><span data-stu-id="129d5-124">Step 3: Load the AzureRM.Netcore module</span></span>

<span data-ttu-id="129d5-125">Uma vez que o módulo seja instalado, terá de carregar o módulo para a sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="129d5-125">Once the module is installed, you need to load the module into your PowerShell session.</span></span> <span data-ttu-id="129d5-126">Os módulos são carregados com o cmdlet `Import-Module`, da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="129d5-126">Modules are loaded using the `Import-Module` cmdlet, as follows:</span></span>

```powershell
Import-Module AzureRM.Netcore
```

<span data-ttu-id="129d5-127">Quando a importação terminar, pode testar o módulo que acabou de instalar ao tentar iniciar sessão no Azure através do seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="129d5-127">After the import completes, you can test your newly installed and module by attempting to sign into Azure using the following command:</span></span>

```powershell
Login-AzureRMAccount
```

<span data-ttu-id="129d5-128">O comando acima deve pedir-lhe para aceder a `https://aka.ms/devicelogin` e introduzir o código fornecido.</span><span class="sxs-lookup"><span data-stu-id="129d5-128">The above command should prompt you to go to `https://aka.ms/devicelogin` and enter the provided code.</span></span>

## <a name="available-cmdlets"></a><span data-ttu-id="129d5-129">Cmdlets disponíveis</span><span class="sxs-lookup"><span data-stu-id="129d5-129">Available cmdlets</span></span>

<span data-ttu-id="129d5-130">Os módulos do Azure PowerShell para .NET Standard ainda estão em desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="129d5-130">The Azure PowerShell modules for .NET Standard are still in development.</span></span> <span data-ttu-id="129d5-131">Estes módulos não fornecem o conjunto completo de cmdlets que estão disponíveis para a versão do Windows dos módulos.</span><span class="sxs-lookup"><span data-stu-id="129d5-131">These modules do not provide the full set of cmdlets that are available for the Windows version of the modules.</span></span> <span data-ttu-id="129d5-132">As seguintes funções estão implementadas nos módulos AzureRM.Netcore:</span><span class="sxs-lookup"><span data-stu-id="129d5-132">The following functions are implemented in AzureRM.Netcore modules:</span></span>

* <span data-ttu-id="129d5-133">Gestão de contas</span><span class="sxs-lookup"><span data-stu-id="129d5-133">Account management</span></span>
  - <span data-ttu-id="129d5-134">Inicie sessão com a conta Microsoft, a conta Organizacional ou o Principal de Serviço através do Microsoft Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="129d5-134">Login with Microsoft account, Organizational account, or Service Principal through Microsoft Azure Active Directory</span></span>
  - <span data-ttu-id="129d5-135">Guarde as Credenciais no disco com o AzureRmContext guardar e carregue as credenciais guardadas com o Import-AzureRmContext</span><span class="sxs-lookup"><span data-stu-id="129d5-135">Save Credentials to disk with Save-AzureRmContext and load saved credentials using Import-AzureRmContext</span></span>
* <span data-ttu-id="129d5-136">Ambiente</span><span class="sxs-lookup"><span data-stu-id="129d5-136">Environment</span></span>
  - <span data-ttu-id="129d5-137">Obtenha os diferentes ambientes do Microsoft Azure prontos a utilizar</span><span class="sxs-lookup"><span data-stu-id="129d5-137">Get the different out-of-box Microsoft Azure environments</span></span>
  - <span data-ttu-id="129d5-138">Adicione/Defina/Remova ambientes personalizados (por exemplo, os ambientes do Azure Stack ou do Windows Azure Pack)</span><span class="sxs-lookup"><span data-stu-id="129d5-138">Add/Set/Remove customized environments (like your Azure Stack or Windows Azure Pack environments)</span></span>
* <span data-ttu-id="129d5-139">Cmdlets do plano de gestão para os serviços do Azure através das interfaces do Resource Manager e da Gestão do Serviço.</span><span class="sxs-lookup"><span data-stu-id="129d5-139">Management plane cmdlets for Azure services using Resource Manager and Service Management interfaces.</span></span>
  - <span data-ttu-id="129d5-140">Máquina Virtual</span><span class="sxs-lookup"><span data-stu-id="129d5-140">Virtual Machine</span></span>
  - <span data-ttu-id="129d5-141">Serviço de Aplicações (Sites)</span><span class="sxs-lookup"><span data-stu-id="129d5-141">App Service (Websites)</span></span>
  - <span data-ttu-id="129d5-142">Base de Dados SQL</span><span class="sxs-lookup"><span data-stu-id="129d5-142">SQL Database</span></span>
  - <span data-ttu-id="129d5-143">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="129d5-143">Storage</span></span>
  - <span data-ttu-id="129d5-144">Rede</span><span class="sxs-lookup"><span data-stu-id="129d5-144">Network</span></span>

## <a name="next-steps"></a><span data-ttu-id="129d5-145">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="129d5-145">Next Steps</span></span>

<span data-ttu-id="129d5-146">Para obter mais informações sobre como utilizar o Azure PowerShell, veja o artigo [Introdução ao Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="129d5-146">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
