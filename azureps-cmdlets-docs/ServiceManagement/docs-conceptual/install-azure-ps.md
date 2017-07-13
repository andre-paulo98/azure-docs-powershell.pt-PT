---
title: "<span data-ttu-id=\"9f5de-101\">Instalar e configurar o módulo Gestão do Serviço do Azure PowerShell | Microsoft Docs</span><span class=\"sxs-lookup\"><span data-stu-id=\"9f5de-101\">Install and configure the Azure PowerShell Service Management module | Microsoft Docs</span></span>"
description: "<span data-ttu-id=\"9f5de-102\">Como instalar e configurar o Azure PowerShell para uma primeira utilização.</span><span class=\"sxs-lookup\"><span data-stu-id=\"9f5de-102\">How to install and configure Azure PowerShell for first time use.</span></span>"
services: azure
author: sdwheeler
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/06/2017
ms.openlocfilehash: c51c727c1cb022eca59f819c7f24d8e058c677da
ms.sourcegitcommit: 226527be7cb647acfe2ea9ab151185053ab3c6db
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/29/2017
---
# <span data-ttu-id="9f5de-103">Instalar o módulo Gestão do Serviço do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="9f5de-103">Installing the Azure PowerShell Service Management module</span></span>
<a id="installing-the-azure-powershell-service-management-module" class="xliff"></a>

<span data-ttu-id="9f5de-104">Instalar o Azure PowerShell a partir da [Galeria do PowerShell](https://www.powershellgallery.com/) é o método de instalação preferencial.</span><span class="sxs-lookup"><span data-stu-id="9f5de-104">Installing Azure PowerShell from the [PowerShell Gallery](https://www.powershellgallery.com/) is the preferred method of installation.</span></span>

## <span data-ttu-id="9f5de-105">Passo 1: Instalar o PowerShellGet</span><span class="sxs-lookup"><span data-stu-id="9f5de-105">Step 1: Install PowerShellGet</span></span>
<a id="step-1-install-powershellget" class="xliff"></a>

<span data-ttu-id="9f5de-106">A instalação de itens a partir da Galeria do PowerShell requer o módulo PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="9f5de-106">Installing items from the PowerShell Gallery requires the PowerShellGet module.</span></span> <span data-ttu-id="9f5de-107">Certifique-se de que tem a versão adequada do PowerShellGet e outros requisitos de sistema.</span><span class="sxs-lookup"><span data-stu-id="9f5de-107">Make sure you have the appropriate version of PowerShellGet and other system requirements.</span></span> <span data-ttu-id="9f5de-108">Execute o seguinte comando para ver se tem o PowerShellGet instalado no sistema.</span><span class="sxs-lookup"><span data-stu-id="9f5de-108">Run the following command to see if you have PowerShellGet installed on your system.</span></span>

```powershell
Get-Module PowerShellGet -list | Select-Object Name,Version,Path
```

<span data-ttu-id="9f5de-109">Deverá ver algo semelhante ao resultado seguinte:</span><span class="sxs-lookup"><span data-stu-id="9f5de-109">You should see something similar to the following output:</span></span>

```
Name          Version Path
----          ------- ----
PowerShellGet 1.0.0.1 C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PowerShellGet.psd1
```

<span data-ttu-id="9f5de-110">Se não tiver o PowerShellGet instalado, veja [Como obter o PowerShellGet](install-azurerm-ps.md#how-to-get-powershellget).</span><span class="sxs-lookup"><span data-stu-id="9f5de-110">If you do not have PowerShellGet installed, see the [How to get PowerShellGet](install-azurerm-ps.md#how-to-get-powershellget).</span></span>

## <span data-ttu-id="9f5de-111">Passo 2: Instalar o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="9f5de-111">Step 2: Install Azure PowerShell</span></span>
<a id="step-2-install-azure-powershell" class="xliff"></a>

<span data-ttu-id="9f5de-112">Execute o comando seguinte a partir da consola do Windows PowerShell em execução como Administrador:</span><span class="sxs-lookup"><span data-stu-id="9f5de-112">Run the following command from the Windows PowerShell console running as Administrator:</span></span>

```powershell
Install-Module Azure
```

<span data-ttu-id="9f5de-113">O módulo Azure é um módulo de rollup para os cmdlets do Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="9f5de-113">The Azure module is a rollup module for the Azure Resource Manager cmdlets.</span></span> <span data-ttu-id="9f5de-114">Quando instala o módulo AzureRM, qualquer outro módulo do Azure que não tenha sido anteriormente instalado será transferido e instalado a partir da Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9f5de-114">When you install the AzureRM module, any other Azure modules that have not previously been installed will be downloaded and installed from the PowerShell Gallery.</span></span>

<span data-ttu-id="9f5de-115">O módulo Gestão do Serviço do Azure partilha dependências com os módulos Azure PowerShell Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="9f5de-115">The Azure Service Management module shares dependencies with the Azure PowerShell Resource Manager modules.</span></span> <span data-ttu-id="9f5de-116">Se tiver instalado os módulos Azure PowerShell Resource Manager, terá de adicionar o parâmetro `-AllowClobber` ao comando de instalação.</span><span class="sxs-lookup"><span data-stu-id="9f5de-116">If you have installed the Azure PowerShell Resource Manager modules, you will need to add the `-AllowClobber` parameter to the install command.</span></span> <span data-ttu-id="9f5de-117">Isto permite a atualização das dependências partilhadas.</span><span class="sxs-lookup"><span data-stu-id="9f5de-117">This allows this existing shared dependencies to be updated.</span></span> <span data-ttu-id="9f5de-118">Sem este parâmetro, a instalação do módulo falha.</span><span class="sxs-lookup"><span data-stu-id="9f5de-118">Without this parameter, installation of the module fails.</span></span>

```powershell
Install-Module Azure -AllowClobber
```

<span data-ttu-id="9f5de-119">Depois de instalar este módulo, pode importá-lo ao executar o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="9f5de-119">After you install this module, you can import the module by running the following command:</span></span>

```powershell
Import-Module Azure
```

## <span data-ttu-id="9f5de-120">Para utilizar os cmdlets</span><span class="sxs-lookup"><span data-stu-id="9f5de-120">To use the cmdlets</span></span>
<a id="to-use-the-cmdlets" class="xliff"></a>

<span data-ttu-id="9f5de-121">Para começar a trabalhar com os cmdlets da Gestão do Serviço do Azure, primeiro inicie sessão na sua conta do Azure.</span><span class="sxs-lookup"><span data-stu-id="9f5de-121">To start working with the Azure Service Management cmdlets, first log on to your Azure account.</span></span> <span data-ttu-id="9f5de-122">Para iniciar sessão na sua conta, execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="9f5de-122">To log on to your account, run the following command:</span></span>

```powershell
Add-AzureAccount
```

<span data-ttu-id="9f5de-123">Depois de iniciar sessão no Azure, o Azure PowerShell cria um contexto para a sessão fornecida.</span><span class="sxs-lookup"><span data-stu-id="9f5de-123">After logging into Azure, Azure PowerShell creates a context for the given session.</span></span> <span data-ttu-id="9f5de-124">Esse contexto contém o ambiente, a conta, o inquilino e a subscrição do Azure PowerShell que serão utilizados para todos os cmdlets nessa sessão.</span><span class="sxs-lookup"><span data-stu-id="9f5de-124">That context contains the Azure PowerShell environment, account, tenant, and subscription that will be used for all cmdlets within that session.</span></span> <span data-ttu-id="9f5de-125">Pode agora utilizar os módulos abaixo.</span><span class="sxs-lookup"><span data-stu-id="9f5de-125">Now you are ready to use the modules below.</span></span>

## <span data-ttu-id="9f5de-126">Cmdlets da Gestão do Serviço do Azure</span><span class="sxs-lookup"><span data-stu-id="9f5de-126">Azure Service Management cmdlets</span></span>
<a id="azure-service-management-cmdlets" class="xliff"></a>

<span data-ttu-id="9f5de-127">Os módulos do Azure PowerShell são atualizados com frequência.</span><span class="sxs-lookup"><span data-stu-id="9f5de-127">Azure PowerShell modules are updated frequently.</span></span> <span data-ttu-id="9f5de-128">Se reparar que a ajuda do cmdlet online inclui cmdlets ou parâmetros que não estão no módulo, transfira e instale a versão mais recente do módulo.</span><span class="sxs-lookup"><span data-stu-id="9f5de-128">If you notice that the online cmdlet help includes cmdlets or parameters that are not in your module, download and install the latest version of the module.</span></span> <span data-ttu-id="9f5de-129">Para localizar a versão do seu módulo, escreva: `(Get-Module Azure).Version`.</span><span class="sxs-lookup"><span data-stu-id="9f5de-129">To find the version of your module, type: `(Get-Module Azure).Version`.</span></span>

<span data-ttu-id="9f5de-130">Para obter scripts de exemplo que podem ajudá-lo a automatizar algumas das tarefas comuns no Azure, veja o [Centro de Scripts do Windows Azure](http://www.windowsazure.com/documentation/scripts/).</span><span class="sxs-lookup"><span data-stu-id="9f5de-130">For sample scripts that can help you automate some of the common tasks in Azure, see the [Windows Azure Script Center](http://www.windowsazure.com/documentation/scripts/).</span></span>

<span data-ttu-id="9f5de-131">Para obter informações gerais sobre a instalação, formação, utilização e personalização do Windows PowerShell, veja [Scripting com o Windows PowerShell](http://go.microsoft.com/fwlink/p/?linkid=320210).</span><span class="sxs-lookup"><span data-stu-id="9f5de-131">For general information about installing, learning, using, and customizing Windows PowerShell, see [Scripting with Windows PowerShell](http://go.microsoft.com/fwlink/p/?linkid=320210).</span></span>
