---
title: Instalar o Azure PowerShell com o PowerShellGet
description: Como instalar o Azure PowerShell com o PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/31/2018
ms.openlocfilehash: 9b7046157e32a5c8473210e9840f9ae1b2f45902
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323106"
---
# <a name="install-azure-powershell-with-powershellget"></a><span data-ttu-id="4835f-103">Instalar o Azure PowerShell com o PowerShellGet</span><span class="sxs-lookup"><span data-stu-id="4835f-103">Install Azure PowerShell with PowerShellGet</span></span>

<span data-ttu-id="4835f-104">Este artigo explica os passos para instalar os módulos do Azure PowerShell num ambiente do Windows com o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="4835f-104">This article explains the steps to install the Azure PowerShell modules in a Windows environment using PowerShellGet.</span></span>  <span data-ttu-id="4835f-105">Esta é a forma preferencial de instalar o Azure PowerShell, mas se preferir instalar com o Instalador de Plataforma Web ou o pacote MSI, veja [Outros métodos de instalação](other-install.md).</span><span class="sxs-lookup"><span data-stu-id="4835f-105">This is the preferred way to install Azure PowerShell, but if you would rather install with the Web Platform Installer or MSI package, see [Other installation methods](other-install.md).</span></span>

<span data-ttu-id="4835f-106">Se quiser utilizar o Azure PowerShell no macOS ou Linux, veja o seguinte artigo: [Instalar e configurar o Azure PowerShell no macOS e Linux](install-azurermps-maclinux.md).</span><span class="sxs-lookup"><span data-stu-id="4835f-106">If you want to use Azure PowerShell on macOS or Linux, see the following article: [Install and configure Azure PowerShell on macOS and Linux](install-azurermps-maclinux.md).</span></span>

## <a name="system-requirements"></a><span data-ttu-id="4835f-107">Requisitos de sistema</span><span class="sxs-lookup"><span data-stu-id="4835f-107">System requirements</span></span>

<span data-ttu-id="4835f-108">A versão 6.1.0 do Azure PowerShell exige a versão 5.0 (ou superior) do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4835f-108">Azure PowerShell version 6.1.0 requires version 5.0 (or higher) of PowerShell.</span></span> <span data-ttu-id="4835f-109">Para obter informações sobre a atualização para o PowerShell 5.0, veja [Atualizar o Windows PowerShell existente](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="4835f-109">For information on upgrading to PowerShell 5.0, see [Upgrading existing Windows PowerShell](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell).</span></span>

<span data-ttu-id="4835f-110">O PowerShellGet está automaticamente incluído no PowerShell 5.0.</span><span class="sxs-lookup"><span data-stu-id="4835f-110">PowerShellGet is automatically included as part of PowerShell 5.0.</span></span>

## <a name="install-or-update-the-azure-powershell-module"></a><span data-ttu-id="4835f-111">Instalar ou atualizar o módulo Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="4835f-111">Install or update the Azure PowerShell module</span></span>

<span data-ttu-id="4835f-112">Instalar o Azure PowerShell a partir da Galeria do PowerShell requer privilégios elevados.</span><span class="sxs-lookup"><span data-stu-id="4835f-112">Installing Azure PowerShell from the PowerShell Gallery requires elevated privileges.</span></span> <span data-ttu-id="4835f-113">Execute o seguinte comando a partir de uma sessão do PowerShell elevada:</span><span class="sxs-lookup"><span data-stu-id="4835f-113">Run the following command from an elevated PowerShell session:</span></span>

```powershell
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module -Name AzureRM -AllowClobber
```

> [!IMPORTANT]
> <span data-ttu-id="4835f-114">Este comando irá atualizar qualquer instalação existente do Azure PowerShell no seu sistema.</span><span class="sxs-lookup"><span data-stu-id="4835f-114">This command will update any existing installation of Azure PowerShell on your system.</span></span> <span data-ttu-id="4835f-115">Se precisar de ter mais do que uma versão instalada, veja a resposta das FAQ a [Posso instalar várias versões do Azure PowerShell?](#multiple-versions)</span><span class="sxs-lookup"><span data-stu-id="4835f-115">If you need to have more than one version installed, see the FAQ answer for [Can I install multiple versions of Azure PowerShell?](#multiple-versions)</span></span>

<span data-ttu-id="4835f-116">Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="4835f-116">By default, the PowerShell gallery is not configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="4835f-117">Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:</span><span class="sxs-lookup"><span data-stu-id="4835f-117">The first time you use the PSGallery you see the following prompt:</span></span>

```Output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="4835f-118">Responder "Sim" ou "Sim a Todos" para continuar com a instalação.</span><span class="sxs-lookup"><span data-stu-id="4835f-118">Answer 'Yes' or 'Yes to All' to continue with the installation.</span></span>

> [!NOTE]
> <span data-ttu-id="4835f-119">Se tiver uma versão mais antiga do que a 2.8.5.201 do NuGet, será pedido que transfira e instale a versão mais recente do NuGet.</span><span class="sxs-lookup"><span data-stu-id="4835f-119">If you have a version older than 2.8.5.201 of NuGet, you are prompted to download and install the latest version of NuGet.</span></span>

<span data-ttu-id="4835f-120">O módulo de AzureRM é um módulo de rollup para os cmdlets do Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="4835f-120">The AzureRM module is a rollup module for the Azure Resource Manager cmdlets.</span></span> <span data-ttu-id="4835f-121">Quando instala o módulo AzureRM, qualquer outro módulo do Azure PowerShell que não tenha sido instalado anteriormente é transferido a partir da Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4835f-121">When you install the AzureRM module, any Azure PowerShell module not previously installed is downloaded from the PowerShell Gallery.</span></span>

## <a name="load-the-azure-powershell-module"></a><span data-ttu-id="4835f-122">Carregar o módulo Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="4835f-122">Load the Azure PowerShell module</span></span>

<span data-ttu-id="4835f-123">Uma vez que o módulo seja instalado, terá de carregar o módulo para a sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4835f-123">Once the module is installed, you need to load the module into your PowerShell session.</span></span> <span data-ttu-id="4835f-124">Deve fazê-lo numa sessão normal (não avaliada) do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4835f-124">You should do this in a normal (non-elevated) PowerShell session.</span></span> <span data-ttu-id="4835f-125">Os módulos são carregados com o cmdlet `Import-Module`, da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="4835f-125">Modules are loaded using the `Import-Module` cmdlet, as follows:</span></span>

```powershell
Import-Module -Name AzureRM
```

## <a name="reporting-issues-and-feedback"></a><span data-ttu-id="4835f-126">Comunicar problemas e comentários</span><span class="sxs-lookup"><span data-stu-id="4835f-126">Reporting issues and feedback</span></span>

<span data-ttu-id="4835f-127">Se detetar erros na ferramenta, [registe um problema no GitHub](https://github.com/Azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="4835f-127">If you encounter any bugs with the tool, please [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span> <span data-ttu-id="4835f-128">Para enviar comentários a partir da linha de comandos, experimente o cmdlet `Send-Feedback`.</span><span class="sxs-lookup"><span data-stu-id="4835f-128">To provide feedback from the command line, use the `Send-Feedback` cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4835f-129">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="4835f-129">Next Steps</span></span>

<span data-ttu-id="4835f-130">Para mais informações sobre como utilizar o Azure PowerShell, consulte os artigos seguintes:</span><span class="sxs-lookup"><span data-stu-id="4835f-130">For more information about using Azure PowerShell, see the following articles:</span></span>

* [<span data-ttu-id="4835f-131">Introdução ao Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="4835f-131">Get started with Azure PowerShell</span></span>](get-started-azureps.md)

## <a name="frequently-asked-questions"></a><span data-ttu-id="4835f-132">Perguntas mais frequentes</span><span class="sxs-lookup"><span data-stu-id="4835f-132">Frequently asked questions</span></span>

### <a id="helpmechoose"></a><span data-ttu-id="4835f-133">Como posso verificar a versão do Azure PowerShell?</span><span class="sxs-lookup"><span data-stu-id="4835f-133">How do I check the version of Azure PowerShell?</span></span>

<span data-ttu-id="4835f-134">Embora o aconselhemos a atualizar para a versão mais recente o mais cedo possível, são suportadas várias versões do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4835f-134">Although we encourage you to upgrade to the latest version as early as possible, several versions of Azure PowerShell are supported.</span></span> <span data-ttu-id="4835f-135">Para determinar a versão do Azure PowerShell que tem instalada, execute `Get-Module AzureRM` a partir da linha de comandos.</span><span class="sxs-lookup"><span data-stu-id="4835f-135">To determine the version of Azure PowerShell you have installed, run `Get-Module AzureRM` from your command line.</span></span>

```powershell
Get-Module AzureRM -ListAvailable | Select-Object -Property Name,Version,Path
```

### <a name="can-i-use-azure-powershell-for-azure-classic-deployments"></a><span data-ttu-id="4835f-136">Posso utilizar o Azure PowerShell para implementações clássicas do Azure?</span><span class="sxs-lookup"><span data-stu-id="4835f-136">Can I use Azure PowerShell for Azure Classic deployments?</span></span>

<span data-ttu-id="4835f-137">Se tiver implementações que utilizam o modelo de implementação clássico, pode instalar a versão de Gestão de Serviço do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4835f-137">If you have deployments that use the classic deployment model you can install the Service Management version of Azure PowerShell.</span></span> <span data-ttu-id="4835f-138">Para obter mais informações, veja [Instalar o módulo Service Management do Azure PowerShell](/powershell/azure/servicemanagement/install-azure-ps).</span><span class="sxs-lookup"><span data-stu-id="4835f-138">For more information, see [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span> <span data-ttu-id="4835f-139">Os módulos Azure e AzureRM partilham dependências comuns.</span><span class="sxs-lookup"><span data-stu-id="4835f-139">The Azure and AzureRM modules share common dependencies.</span></span> <span data-ttu-id="4835f-140">Se utilizar os módulos do Azure e do AzureRM, deve instalar a mesma versão de cada pacote.</span><span class="sxs-lookup"><span data-stu-id="4835f-140">If you use both the Azure and AzureRM modules, you should install the same version of each package.</span></span>

### <a name="a-namemultiple-versionscan-i-install-multiple-versions-of-azure-powershell"></a><span data-ttu-id="4835f-141"><a name="multiple-versions"/>Posso instalar várias versões do Azure PowerShell?</span><span class="sxs-lookup"><span data-stu-id="4835f-141"><a name="multiple-versions"/>Can I install multiple versions of Azure PowerShell?</span></span>

<span data-ttu-id="4835f-142">O PowerShellGet é o único método de instalação que suporta várias versões.</span><span class="sxs-lookup"><span data-stu-id="4835f-142">PowerShellGet the only method of installation that supports multiple versions.</span></span> <span data-ttu-id="4835f-143">Para instalar várias versões, pode adicionar o parâmetro `-RequiredVersion` ao cmdlet `Install-Module`.</span><span class="sxs-lookup"><span data-stu-id="4835f-143">To install multiple versions, you can add the `-RequiredVersion` parameter to the `Install-Module` cmdlet.</span></span> <span data-ttu-id="4835f-144">Por exemplo, para instalar as versões 6.1.0 e 1.2.9:</span><span class="sxs-lookup"><span data-stu-id="4835f-144">For example, to install both versions 6.1.0 and 1.2.9:</span></span>

```powershell
Install-Module -Name AzureRM -RequiredVersion 6.1.0
Install-Module -Name AzureRM -RequiredVersion 1.2.9
```

<span data-ttu-id="4835f-145">Apenas uma versão do módulo pode ser carregada numa sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4835f-145">Only one version of the module can be loaded in a PowerShell session.</span></span> <span data-ttu-id="4835f-146">Tem de abrir uma nova janela do PowerShell e utilizar `Import-Module` para importar uma versão específica do módulo Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4835f-146">You must open a new PowerShell window and use `Import-Module` to import a specific version of the Azure PowerShell module.</span></span>

```powershell
Import-Module -Name AzureRM -RequiredVersion 1.2.9
```

> [!NOTE]
> <span data-ttu-id="4835f-147">A versão 2.1.0 e a versão 1.2.6 são as primeiras versões do módulo concebidas para serem instaladas e utilizadas lado a lado.</span><span class="sxs-lookup"><span data-stu-id="4835f-147">Version 2.1.0 and version 1.2.6 are the first module versions designed to be installed and used side by side.</span></span> <span data-ttu-id="4835f-148">Ao carregar uma versão anterior do Azure PowerShell, as versões incompatíveis do módulo **AzureRM.Profile** são carregadas.</span><span class="sxs-lookup"><span data-stu-id="4835f-148">When loading an earlier version of the Azure PowerShell, incompatible versions of the **AzureRM.Profile** module are loaded.</span></span> <span data-ttu-id="4835f-149">Isto resulta nos cmdlets solicitando que inicie sessão sempre executar um cmdlet.</span><span class="sxs-lookup"><span data-stu-id="4835f-149">This results in the cmdlets prompting you to log in whenever you execute a cmdlet.</span></span>
