---
title: "Instalar e configurar o módulo Gestão do Serviço do Azure PowerShell | Microsoft Docs"
description: "Como instalar e configurar o Azure PowerShell para uma primeira utilização."
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/06/2017
ms.openlocfilehash: f46fe25352c100976dd8fc3b1c48ddfc3926f906
ms.sourcegitcommit: 7a1c08518b180de822c915db99b055b93a1459d7
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/17/2017
---
# <a name="installing-the-azure-powershell-service-management-module"></a><span data-ttu-id="426bc-103">Instalar o módulo Gestão do Serviço do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="426bc-103">Installing the Azure PowerShell Service Management module</span></span>

<span data-ttu-id="426bc-104">Instalar o Azure PowerShell a partir da [Galeria do PowerShell](https://www.powershellgallery.com/) é o método de instalação preferencial.</span><span class="sxs-lookup"><span data-stu-id="426bc-104">Installing Azure PowerShell from the [PowerShell Gallery](https://www.powershellgallery.com/) is the preferred method of installation.</span></span>

## <a name="step-1-install-powershellget"></a><span data-ttu-id="426bc-105">Passo 1: Instalar o PowerShellGet</span><span class="sxs-lookup"><span data-stu-id="426bc-105">Step 1: Install PowerShellGet</span></span>

<span data-ttu-id="426bc-106">A instalação de itens a partir da Galeria do PowerShell requer o módulo PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="426bc-106">Installing items from the PowerShell Gallery requires the PowerShellGet module.</span></span> <span data-ttu-id="426bc-107">Certifique-se de que tem a versão adequada do PowerShellGet e outros requisitos de sistema.</span><span class="sxs-lookup"><span data-stu-id="426bc-107">Make sure you have the appropriate version of PowerShellGet and other system requirements.</span></span> <span data-ttu-id="426bc-108">Execute o seguinte comando para ver se tem o PowerShellGet instalado no sistema.</span><span class="sxs-lookup"><span data-stu-id="426bc-108">Run the following command to see if you have PowerShellGet installed on your system.</span></span>

```powershell
Get-Module PowerShellGet -list | Select-Object Name,Version,Path
```

<span data-ttu-id="426bc-109">Deverá ver algo semelhante ao resultado seguinte:</span><span class="sxs-lookup"><span data-stu-id="426bc-109">You should see something similar to the following output:</span></span>

```
Name          Version Path
----          ------- ----
PowerShellGet 1.0.0.1 C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PowerShellGet.psd1
```

<span data-ttu-id="426bc-110">Se não tiver o PowerShellGet instalado, veja [Como obter o PowerShellGet](#how-to-get-powershellget).</span><span class="sxs-lookup"><span data-stu-id="426bc-110">If you do not have PowerShellGet installed, see the [How to get PowerShellGet](#how-to-get-powershellget).</span></span>

## <a name="step-2-install-azure-powershell"></a><span data-ttu-id="426bc-111">Passo 2: Instalar o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="426bc-111">Step 2: Install Azure PowerShell</span></span>

<span data-ttu-id="426bc-112">Execute o comando seguinte a partir da consola do Windows PowerShell em execução como Administrador:</span><span class="sxs-lookup"><span data-stu-id="426bc-112">Run the following command from the Windows PowerShell console running as Administrator:</span></span>

```powershell
Install-Module Azure
```

<span data-ttu-id="426bc-113">O módulo Azure é um módulo de rollup para os cmdlets do Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="426bc-113">The Azure module is a rollup module for the Azure Resource Manager cmdlets.</span></span> <span data-ttu-id="426bc-114">Quando instala o módulo AzureRM, qualquer outro módulo do Azure que não tenha sido anteriormente instalado será transferido e instalado a partir da Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="426bc-114">When you install the AzureRM module, any other Azure modules that have not previously been installed will be downloaded and installed from the PowerShell Gallery.</span></span>

<span data-ttu-id="426bc-115">O módulo Gestão do Serviço do Azure partilha dependências com os módulos Azure PowerShell Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="426bc-115">The Azure Service Management module shares dependencies with the Azure PowerShell Resource Manager modules.</span></span> <span data-ttu-id="426bc-116">Se tiver instalado os módulos Azure PowerShell Resource Manager, terá de adicionar o parâmetro `-AllowClobber` ao comando de instalação.</span><span class="sxs-lookup"><span data-stu-id="426bc-116">If you have installed the Azure PowerShell Resource Manager modules, you will need to add the `-AllowClobber` parameter to the install command.</span></span> <span data-ttu-id="426bc-117">Isto permite a atualização das dependências partilhadas.</span><span class="sxs-lookup"><span data-stu-id="426bc-117">This allows this existing shared dependencies to be updated.</span></span> <span data-ttu-id="426bc-118">Sem este parâmetro, a instalação do módulo falha.</span><span class="sxs-lookup"><span data-stu-id="426bc-118">Without this parameter, installation of the module fails.</span></span>

```powershell
Install-Module Azure -AllowClobber
```

<span data-ttu-id="426bc-119">Depois de instalar este módulo, pode importá-lo ao executar o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="426bc-119">After you install this module, you can import the module by running the following command:</span></span>

```powershell
Import-Module Azure
```

## <a name="to-use-the-cmdlets"></a><span data-ttu-id="426bc-120">Para utilizar os cmdlets</span><span class="sxs-lookup"><span data-stu-id="426bc-120">To use the cmdlets</span></span>

<span data-ttu-id="426bc-121">Para começar a trabalhar com os cmdlets da Gestão do Serviço do Azure, primeiro inicie sessão na sua conta do Azure.</span><span class="sxs-lookup"><span data-stu-id="426bc-121">To start working with the Azure Service Management cmdlets, first log on to your Azure account.</span></span> <span data-ttu-id="426bc-122">Para iniciar sessão na sua conta, execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="426bc-122">To log on to your account, run the following command:</span></span>

```powershell
Add-AzureAccount
```

<span data-ttu-id="426bc-123">Depois de iniciar sessão no Azure, o Azure PowerShell cria um contexto para a sessão fornecida.</span><span class="sxs-lookup"><span data-stu-id="426bc-123">After logging into Azure, Azure PowerShell creates a context for the given session.</span></span> <span data-ttu-id="426bc-124">Esse contexto contém o ambiente, a conta, o inquilino e a subscrição do Azure PowerShell que serão utilizados para todos os cmdlets nessa sessão.</span><span class="sxs-lookup"><span data-stu-id="426bc-124">That context contains the Azure PowerShell environment, account, tenant, and subscription that will be used for all cmdlets within that session.</span></span> <span data-ttu-id="426bc-125">Pode agora utilizar os módulos abaixo.</span><span class="sxs-lookup"><span data-stu-id="426bc-125">Now you are ready to use the modules below.</span></span>

## <a name="azure-service-management-cmdlets"></a><span data-ttu-id="426bc-126">Cmdlets da Gestão do Serviço do Azure</span><span class="sxs-lookup"><span data-stu-id="426bc-126">Azure Service Management cmdlets</span></span>

<span data-ttu-id="426bc-127">Os módulos do Azure PowerShell são atualizados com frequência.</span><span class="sxs-lookup"><span data-stu-id="426bc-127">Azure PowerShell modules are updated frequently.</span></span> <span data-ttu-id="426bc-128">Se reparar que a ajuda do cmdlet online inclui cmdlets ou parâmetros que não estão no módulo, transfira e instale a versão mais recente do módulo.</span><span class="sxs-lookup"><span data-stu-id="426bc-128">If you notice that the online cmdlet help includes cmdlets or parameters that are not in your module, download and install the latest version of the module.</span></span> <span data-ttu-id="426bc-129">Para localizar a versão do seu módulo, escreva: `(Get-Module Azure).Version`.</span><span class="sxs-lookup"><span data-stu-id="426bc-129">To find the version of your module, type: `(Get-Module Azure).Version`.</span></span>

<span data-ttu-id="426bc-130">Para obter scripts de exemplo que podem ajudá-lo a automatizar algumas das tarefas comuns no Azure, veja o [Centro de Scripts do Windows Azure](http://www.windowsazure.com/documentation/scripts/).</span><span class="sxs-lookup"><span data-stu-id="426bc-130">For sample scripts that can help you automate some of the common tasks in Azure, see the [Windows Azure Script Center](http://www.windowsazure.com/documentation/scripts/).</span></span>

<span data-ttu-id="426bc-131">Para obter informações gerais sobre a instalação, formação, utilização e personalização do Windows PowerShell, veja [Scripting com o Windows PowerShell](http://go.microsoft.com/fwlink/p/?linkid=320210).</span><span class="sxs-lookup"><span data-stu-id="426bc-131">For general information about installing, learning, using, and customizing Windows PowerShell, see [Scripting with Windows PowerShell](http://go.microsoft.com/fwlink/p/?linkid=320210).</span></span>

### <a name="how-to-get-powershellget"></a><span data-ttu-id="426bc-132">Como obter o PowerShellGet</span><span class="sxs-lookup"><span data-stu-id="426bc-132">How to get PowerShellGet</span></span>

|<span data-ttu-id="426bc-133">Versão do SO</span><span class="sxs-lookup"><span data-stu-id="426bc-133">OS Version</span></span>|<span data-ttu-id="426bc-134">Instruções de instalação</span><span class="sxs-lookup"><span data-stu-id="426bc-134">Install instructions</span></span>|
|---|---|
|<span data-ttu-id="426bc-135">Tenho o Windows 10 ou o Windows Server 2016</span><span class="sxs-lookup"><span data-stu-id="426bc-135">I have Windows 10 or Windows Server 2016</span></span>|<span data-ttu-id="426bc-136">Incorporado no Windows Management Framework (WMF) 5.0 incluído no SO</span><span class="sxs-lookup"><span data-stu-id="426bc-136">Built into Windows Management Framework (WMF) 5.0 included in the OS</span></span>|
|<span data-ttu-id="426bc-137">Quero atualizar para o PowerShell 5</span><span class="sxs-lookup"><span data-stu-id="426bc-137">I want to upgrade to PowerShell 5</span></span>|[<span data-ttu-id="426bc-138">Instalar a versão mais recente do WMF</span><span class="sxs-lookup"><span data-stu-id="426bc-138">Install the latest version of WMF</span></span>](https://www.microsoft.com/en-us/download/details.aspx?id=54616)|
|<span data-ttu-id="426bc-139">Estou a executar uma versão do Windows com o PowerShell 3 ou o PowerShell 4</span><span class="sxs-lookup"><span data-stu-id="426bc-139">I am running on a version of Windows with PowerShell 3 or PowerShell 4</span></span>|[<span data-ttu-id="426bc-140">Obter os módulos PackageManagement</span><span class="sxs-lookup"><span data-stu-id="426bc-140">Get the PackageManagement modules</span></span>](http://go.microsoft.com/fwlink/?LinkID=746217)|

<a id="helpmechoose"></a>
### <a name="checking-the-version-of-azure-powershell"></a><span data-ttu-id="426bc-141">A verificar a versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="426bc-141">Checking the version of Azure PowerShell</span></span>

<span data-ttu-id="426bc-142">Embora o aconselhemos a atualizar para a versão mais recente o mais cedo possível, são suportadas várias versões do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="426bc-142">Although we encourage you to upgrade to the latest version as early as possible, several versions of Azure PowerShell are support.</span></span> <span data-ttu-id="426bc-143">Para determinar a versão do Azure PowerShell que tem instalada, execute `Get-Module AzureRM` a partir da linha de comandos.</span><span class="sxs-lookup"><span data-stu-id="426bc-143">To determine the version of Azure PowerShell you have installed, run `Get-Module AzureRM` from your command line.</span></span>

```powershell
Get-Module AzureRM -list | Select-Object Name,Version,Path
```