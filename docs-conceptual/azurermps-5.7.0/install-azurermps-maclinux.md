---
title: Instalar o Azure PowerShell no macOS ou Linux
description: Como instalar o Azure PowerShell no macOS ou Linux.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 17912c155255b6fdfd3cfb9242163b67d405dc03
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323259"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a><span data-ttu-id="e72ad-103">Instalar o Azure PowerShell no macOS ou Linux</span><span class="sxs-lookup"><span data-stu-id="e72ad-103">Install Azure PowerShell on macOS or Linux</span></span>

<span data-ttu-id="e72ad-104">Em plataformas não Windows, é possível executar o Azure PowerShell por cima do PowerShell Core v6.</span><span class="sxs-lookup"><span data-stu-id="e72ad-104">For non-Windows platforms, it's possible to run Azure PowerShell on top of PowerShell Core v6.</span></span> <span data-ttu-id="e72ad-105">Em vez do Azure PowerShell padrão baseado no .NET Framework para Windows, este produto foi concebido para o .NET Core e pode ser executado em qualquer plataforma que suporte o .Net Core runtime.</span><span class="sxs-lookup"><span data-stu-id="e72ad-105">Rather than the standard Azure PowerShell built on .NET Framework for Windows, this product is built for .NET Core and can run on any platform which supports the .Net Core runtime.</span></span>

> [!NOTE]
> <span data-ttu-id="e72ad-106">Atualmente, tanto o PowerShell Core v6 como o Azure PowerShell para .NET Core ainda se encontram em fase beta.</span><span class="sxs-lookup"><span data-stu-id="e72ad-106">At this time, both PowerShell Core v6 and Azure PowerShell for .NET Core are still in beta.</span></span>
> <span data-ttu-id="e72ad-107">O suporte para estes produtos é limitado.</span><span class="sxs-lookup"><span data-stu-id="e72ad-107">Support for these products is limited.</span></span> <span data-ttu-id="e72ad-108">Se se deparar com problemas ou detetar erros, registe um problema no GitHub.</span><span class="sxs-lookup"><span data-stu-id="e72ad-108">If you have problems or discover bugs, please file an issue on GitHub.</span></span>
>
> * [<span data-ttu-id="e72ad-109">Problemas do PowerShell Core v6</span><span class="sxs-lookup"><span data-stu-id="e72ad-109">Issues for PowerShell Core v6</span></span>](https://github.com/PowerShell/PowerShell/issues)
> * [<span data-ttu-id="e72ad-110">Problemas do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="e72ad-110">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core-v6"></a><span data-ttu-id="e72ad-111">Instalar o PowerShell Core v6</span><span class="sxs-lookup"><span data-stu-id="e72ad-111">Install PowerShell Core v6</span></span>

<span data-ttu-id="e72ad-112">A instalação do PowerShell Core v6 no Linux ou macOS varia consoante a distribuição do Linux e a versão do SO.</span><span class="sxs-lookup"><span data-stu-id="e72ad-112">Installing PowerShell Core v6 on Linux or macOS varies depending on the Linux distribution and OS version.</span></span>
<span data-ttu-id="e72ad-113">Pode encontrar instruções detalhadas nos seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="e72ad-113">Detailed instructions can be found in the following articles:</span></span>

- [<span data-ttu-id="e72ad-114">Instalar o PowerShell Core no macOS</span><span class="sxs-lookup"><span data-stu-id="e72ad-114">Install PowerShell Core on macOS</span></span>](/powershell/scripting/setup/installing-powershell-core-on-macos)
- [<span data-ttu-id="e72ad-115">Instalar o PowerShell Core no Linux</span><span class="sxs-lookup"><span data-stu-id="e72ad-115">Install PowerShell Core on Linux</span></span>](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a><span data-ttu-id="e72ad-116">Instalar o Azure PowerShell para o .NET Core</span><span class="sxs-lookup"><span data-stu-id="e72ad-116">Install Azure PowerShell for .NET Core</span></span>

<span data-ttu-id="e72ad-117">O PowerShell Core v6 é fornecido com o módulo PowerShellGet já instalado.</span><span class="sxs-lookup"><span data-stu-id="e72ad-117">PowerShell Core v6 comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="e72ad-118">o que facilita a instalação de qualquer módulo que seja publicado na Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e72ad-118">This makes it easy to install any module that is published to the PowerShell Gallery.</span></span> <span data-ttu-id="e72ad-119">Para instalar o Azure PowerShell, abra uma nova sessão do PowerShell e execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="e72ad-119">To install Azure PowerShell, open a new PowerShell session and run the following command:</span></span>

```powershell
Install-Module AzureRM.NetCore
```

## <a name="load-the-azurermnetcore-module"></a><span data-ttu-id="e72ad-120">Carregar o módulo AzureRM.Netcore</span><span class="sxs-lookup"><span data-stu-id="e72ad-120">Load the AzureRM.Netcore module</span></span>

<span data-ttu-id="e72ad-121">Uma vez que o módulo seja instalado, terá de carregar o módulo para a sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e72ad-121">Once the module is installed, you need to load the module into your PowerShell session.</span></span> <span data-ttu-id="e72ad-122">Os módulos são carregados com o cmdlet `Import-Module`, da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="e72ad-122">Modules are loaded using the `Import-Module` cmdlet, as follows:</span></span>

```powershell
Import-Module AzureRM.Netcore
Import-Module AzureRM.Profile.Netcore
```

<span data-ttu-id="e72ad-123">Quando a importação terminar, pode testar o módulo que acabou de instalar ao tentar iniciar sessão no Azure através do seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="e72ad-123">After the import completes, you can test your newly installed and module by attempting to sign into Azure using the following command:</span></span>

```powershell
Connect-AzureRmAccount
```

<span data-ttu-id="e72ad-124">O comando acima deve pedir-lhe para aceder a `https://aka.ms/devicelogin` e introduzir o código fornecido.</span><span class="sxs-lookup"><span data-stu-id="e72ad-124">The above command should prompt you to go to `https://aka.ms/devicelogin` and enter the provided code.</span></span>

## <a name="available-cmdlets"></a><span data-ttu-id="e72ad-125">Cmdlets disponíveis</span><span class="sxs-lookup"><span data-stu-id="e72ad-125">Available cmdlets</span></span>

<span data-ttu-id="e72ad-126">Os módulos do Azure PowerShell para .NET Standard ainda estão em desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="e72ad-126">The Azure PowerShell modules for .NET Standard are still in development.</span></span> <span data-ttu-id="e72ad-127">Estes módulos não fornecem o conjunto completo de cmdlets que estão disponíveis para a versão do Windows dos módulos.</span><span class="sxs-lookup"><span data-stu-id="e72ad-127">These modules do not provide the full set of cmdlets that are available for the Windows version of the modules.</span></span> <span data-ttu-id="e72ad-128">As seguintes funções estão implementadas nos módulos AzureRM.Netcore:</span><span class="sxs-lookup"><span data-stu-id="e72ad-128">The following functions are implemented in AzureRM.Netcore modules:</span></span>

* <span data-ttu-id="e72ad-129">Gestão de contas</span><span class="sxs-lookup"><span data-stu-id="e72ad-129">Account management</span></span>
  - <span data-ttu-id="e72ad-130">Inicie sessão com a conta Microsoft, a conta Organizacional ou o Principal de Serviço através do Microsoft Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="e72ad-130">Login with Microsoft account, Organizational account, or Service Principal through Microsoft Azure Active Directory</span></span>
  - <span data-ttu-id="e72ad-131">Guarde as Credenciais no disco com o AzureRmContext guardar e carregue as credenciais guardadas com o Import-AzureRmContext</span><span class="sxs-lookup"><span data-stu-id="e72ad-131">Save Credentials to disk with Save-AzureRmContext and load saved credentials using Import-AzureRmContext</span></span>
* <span data-ttu-id="e72ad-132">Ambiente</span><span class="sxs-lookup"><span data-stu-id="e72ad-132">Environment</span></span>
  - <span data-ttu-id="e72ad-133">Obtenha os diferentes ambientes do Microsoft Azure prontos a utilizar</span><span class="sxs-lookup"><span data-stu-id="e72ad-133">Get the different out-of-box Microsoft Azure environments</span></span>
  - <span data-ttu-id="e72ad-134">Adicione/Defina/Remova ambientes personalizados (por exemplo, os ambientes do Azure Stack ou do Windows Azure Pack)</span><span class="sxs-lookup"><span data-stu-id="e72ad-134">Add/Set/Remove customized environments (like your Azure Stack or Windows Azure Pack environments)</span></span>
* <span data-ttu-id="e72ad-135">Cmdlets do plano de gestão para os serviços do Azure através das interfaces do Resource Manager e da Gestão do Serviço.</span><span class="sxs-lookup"><span data-stu-id="e72ad-135">Management plane cmdlets for Azure services using Resource Manager and Service Management interfaces.</span></span>
  - <span data-ttu-id="e72ad-136">Máquina Virtual</span><span class="sxs-lookup"><span data-stu-id="e72ad-136">Virtual Machine</span></span>
  - <span data-ttu-id="e72ad-137">Serviço de Aplicações (Sites)</span><span class="sxs-lookup"><span data-stu-id="e72ad-137">App Service (Websites)</span></span>
  - <span data-ttu-id="e72ad-138">SQL Database</span><span class="sxs-lookup"><span data-stu-id="e72ad-138">SQL Database</span></span>
  - <span data-ttu-id="e72ad-139">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e72ad-139">Storage</span></span>
  - <span data-ttu-id="e72ad-140">Rede</span><span class="sxs-lookup"><span data-stu-id="e72ad-140">Network</span></span>

## <a name="next-steps"></a><span data-ttu-id="e72ad-141">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="e72ad-141">Next Steps</span></span>

<span data-ttu-id="e72ad-142">Para obter mais informações sobre como utilizar o Azure PowerShell, veja o artigo [Introdução ao Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="e72ad-142">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
