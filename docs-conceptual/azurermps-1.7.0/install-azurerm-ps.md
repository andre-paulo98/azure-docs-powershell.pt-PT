---
title: Instalar e configurar o Azure PowerShell | Microsoft Docs
description: "Como instalar e configurar o Azure PowerShell para uma primeira utilização."
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/17/2017
ms.openlocfilehash: 0c1500a8748a3aa4546c6ce1e8d16a635b056edb
ms.sourcegitcommit: b256bf48e15ee98865de0fae50e7b81878b03a54
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/03/2017
---
# <a name="install-and-configure-azure-powershell"></a><span data-ttu-id="14164-103">Instalar e configurar o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="14164-103">Install and configure Azure PowerShell</span></span>

<span data-ttu-id="14164-104">Instalar o Azure PowerShell a partir da Galeria do PowerShell é o método de instalação preferencial.</span><span class="sxs-lookup"><span data-stu-id="14164-104">Installing Azure PowerShell from the PowerShell Gallery is the preferred method of installation.</span></span>

## <a name="step-1-install-powershellget"></a><span data-ttu-id="14164-105">Passo 1: Instalar o PowerShellGet</span><span class="sxs-lookup"><span data-stu-id="14164-105">Step 1: Install PowerShellGet</span></span>

<span data-ttu-id="14164-106">A instalação de itens a partir da Galeria do PowerShell requer o módulo PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="14164-106">Installing items from the PowerShell Gallery requires the PowerShellGet module.</span></span> <span data-ttu-id="14164-107">Certifique-se de que tem a versão adequada do PowerShellGet e outros requisitos de sistema.</span><span class="sxs-lookup"><span data-stu-id="14164-107">Make sure you have the appropriate version of PowerShellGet and other system requirements.</span></span> <span data-ttu-id="14164-108">Execute o seguinte comando para ver se tem o PowerShellGet instalado no sistema.</span><span class="sxs-lookup"><span data-stu-id="14164-108">Run the following command to see if you have PowerShellGet installed on your system.</span></span>

```powershell
Get-Module PowerShellGet -list | Select-Object Name,Version,Path
```

<span data-ttu-id="14164-109">Deverá ver algo semelhante à saída seguinte:</span><span class="sxs-lookup"><span data-stu-id="14164-109">You should see something similar to the following output:</span></span>

```
Name          Version Path
----          ------- ----
PowerShellGet 1.0.0.1 C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PowerShellGet.psd1
```

<span data-ttu-id="14164-110">Se não tiver o PowerShellGet instalado, veja a secção [Como obter o PowerShellGet](#how-to-get-powershellget) deste artigo.</span><span class="sxs-lookup"><span data-stu-id="14164-110">If you do not have PowerShellGet installed, see the [How to get PowerShellGet](#how-to-get-powershellget) section of this article.</span></span>

> [!NOTE]
> <span data-ttu-id="14164-111">A utilização do PowerShellGet requer uma Política de Execução que lhe permita executar scripts.</span><span class="sxs-lookup"><span data-stu-id="14164-111">Using PowerShellGet requires an Execution Policy that allows you to run scripts.</span></span> <span data-ttu-id="14164-112">Para obter mais informações sobre a Política de Execução do PowerShell, veja [About Execution Policies (Sobre as Políticas de Execução)](https://msdn.microsoft.com/powershell/reference/5.1/microsoft.powershell.core/about/about_execution_policies).</span><span class="sxs-lookup"><span data-stu-id="14164-112">For more information about PowerShell's Execution Policy, see [About Execution Policies](https://msdn.microsoft.com/powershell/reference/5.1/microsoft.powershell.core/about/about_execution_policies).</span></span>

## <a name="step-2-install-azure-powershell"></a><span data-ttu-id="14164-113">Passo 2: Instalar o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="14164-113">Step 2: Install Azure PowerShell</span></span>

<span data-ttu-id="14164-114">Instalar o Azure PowerShell a partir da Galeria do PowerShell requer privilégios elevados.</span><span class="sxs-lookup"><span data-stu-id="14164-114">Installing Azure PowerShell from the PowerShell Gallery requires elevated privileges.</span></span> <span data-ttu-id="14164-115">Execute o seguinte comando a partir de uma sessão do PowerShell elevada:</span><span class="sxs-lookup"><span data-stu-id="14164-115">Run the following command from an elevated PowerShell session:</span></span>

```powershell
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module AzureRM
```

<span data-ttu-id="14164-116">Por predefinição, a galeria do PowerShell não está configurada como um repositório Fidedigno para PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="14164-116">By default, the PowerShell gallery is not configured as a Trusted repository for PowerShellGet.</span></span> <span data-ttu-id="14164-117">Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:</span><span class="sxs-lookup"><span data-stu-id="14164-117">The first time you use the PSGallery you see the following prompt:</span></span>

```
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"): Y
```

<span data-ttu-id="14164-118">Responder "Sim" ou "Sim a Todos" para continuar com a instalação.</span><span class="sxs-lookup"><span data-stu-id="14164-118">Answer 'Yes' or 'Yes to All' to continue with the installation.</span></span>

> [!NOTE]
> <span data-ttu-id="14164-119">Se tiver uma versão mais antiga do que a 2.8.5.201 do NuGet, será pedido que transfira e instale a versão mais recente do NuGet.</span><span class="sxs-lookup"><span data-stu-id="14164-119">If you have a version older than 2.8.5.201 of NuGet, you are prompted to download and install the latest version of NuGet.</span></span>

<span data-ttu-id="14164-120">O módulo de AzureRM é um módulo de rollup para os cmdlets do Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="14164-120">The AzureRM module is a rollup module for the Azure Resource Manager cmdlets.</span></span> <span data-ttu-id="14164-121">Quando instala o módulo AzureRM, qualquer outro módulo do Azure PowerShell que não tenha sido anteriormente instalado será transferido a partir da Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="14164-121">When you install the AzureRM module, any Azure PowerShell module not previously installed is downloaded and from the PowerShell Gallery.</span></span>

<span data-ttu-id="14164-122">Se tiver uma versão anterior do Azure PowerShell instalado poderá receber um erro.</span><span class="sxs-lookup"><span data-stu-id="14164-122">If you have a previous version of Azure PowerShell installed you may receive an error.</span></span> <span data-ttu-id="14164-123">Para resolver este problema, veja a secção [Updating to a new version of Azure PowerShell](#update-azps)(Atualizar para uma versão nova do Azure PowerShell) deste artigo.</span><span class="sxs-lookup"><span data-stu-id="14164-123">To resolve this issue, see the [Updating to a new version of Azure PowerShell](#update-azps) section of this article.</span></span>

## <a name="step-3-load-the-azurerm-module"></a><span data-ttu-id="14164-124">Passo 3: carregar o módulo de AzureRM</span><span class="sxs-lookup"><span data-stu-id="14164-124">Step 3: Load the AzureRM module</span></span>
<span data-ttu-id="14164-125">Uma vez que o módulo seja instalado, terá de carregar o módulo para a sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="14164-125">Once the module is installed, you need to load the module into your PowerShell session.</span></span> <span data-ttu-id="14164-126">Deve fazê-lo numa sessão normal (não avaliada) do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="14164-126">You should do this in a normal (non-elevated) PowerShell session.</span></span> <span data-ttu-id="14164-127">Os módulos são carregados com o cmdlet `Import-Module`, da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="14164-127">Modules are loaded using the `Import-Module` cmdlet, as follows:</span></span>

```powershell
Import-Module AzureRM
```

## <a name="next-steps"></a><span data-ttu-id="14164-128">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="14164-128">Next Steps</span></span>

<span data-ttu-id="14164-129">Para mais informações sobre como utilizar o Azure PowerShell, consulte os artigos seguintes:</span><span class="sxs-lookup"><span data-stu-id="14164-129">For more information about using Azure PowerShell, see the following articles:</span></span>

* [<span data-ttu-id="14164-130">Introdução ao Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="14164-130">Get started with Azure PowerShell</span></span>](get-started-azureps.md)

## <a name="frequently-asked-questions"></a><span data-ttu-id="14164-131">Perguntas mais frequentes</span><span class="sxs-lookup"><span data-stu-id="14164-131">Frequently asked questions</span></span>

### <a name="how-to-get-powershellget"></a><span data-ttu-id="14164-132">Como obter o PowerShellGet</span><span class="sxs-lookup"><span data-stu-id="14164-132">How to get PowerShellGet</span></span>

|<span data-ttu-id="14164-133">Versão do SO</span><span class="sxs-lookup"><span data-stu-id="14164-133">OS Version</span></span>|<span data-ttu-id="14164-134">Instruções de instalação</span><span class="sxs-lookup"><span data-stu-id="14164-134">Install instructions</span></span>|
|---|---|
|<span data-ttu-id="14164-135">Tenho o Windows 10 ou o Windows Server 2016</span><span class="sxs-lookup"><span data-stu-id="14164-135">I have Windows 10 or Windows Server 2016</span></span>|<span data-ttu-id="14164-136">Incorporado no Windows Management Framework (WMF) 5.0 incluído no SO</span><span class="sxs-lookup"><span data-stu-id="14164-136">Built into Windows Management Framework (WMF) 5.0 included in the OS</span></span>|
|<span data-ttu-id="14164-137">Quero atualizar para o PowerShell 5</span><span class="sxs-lookup"><span data-stu-id="14164-137">I want to upgrade to PowerShell 5</span></span>|[<span data-ttu-id="14164-138">Instalar a versão mais recente do WMF</span><span class="sxs-lookup"><span data-stu-id="14164-138">Install the latest version of WMF</span></span>](https://www.microsoft.com/en-us/download/details.aspx?id=54616)|
|<span data-ttu-id="14164-139">Estou a executar uma versão do Windows com o PowerShell 3 ou o PowerShell 4</span><span class="sxs-lookup"><span data-stu-id="14164-139">I am running on a version of Windows with PowerShell 3 or PowerShell 4</span></span>|[<span data-ttu-id="14164-140">Obter os módulos PackageManagement</span><span class="sxs-lookup"><span data-stu-id="14164-140">Get the PackageManagement modules</span></span>](http://go.microsoft.com/fwlink/?LinkID=746217)|

<a id="helpmechoose"></a>
### <a name="checking-the-version-of-azure-powershell"></a><span data-ttu-id="14164-141">A verificar a versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="14164-141">Checking the version of Azure PowerShell</span></span>

<span data-ttu-id="14164-142">Embora o aconselhemos a atualizar para a versão mais recente o mais cedo possível, são suportadas várias versões do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="14164-142">Although we encourage you to upgrade to the latest version as early as possible, several versions of Azure PowerShell are support.</span></span> <span data-ttu-id="14164-143">Para determinar a versão do Azure PowerShell que tem instalada, execute `Get-Module AzureRM` a partir da linha de comandos.</span><span class="sxs-lookup"><span data-stu-id="14164-143">To determine the version of Azure PowerShell you have installed, run `Get-Module AzureRM` from your command line.</span></span>

```powershell
Get-Module AzureRM -list | Select-Object Name,Version,Path
```

### <a name="support-for-classic-deployment-methods"></a><span data-ttu-id="14164-144">Suporte para os métodos de implementação clássicos</span><span class="sxs-lookup"><span data-stu-id="14164-144">Support for classic deployment methods</span></span>

<span data-ttu-id="14164-145">Se tiver implementações que utilizam o modelo de implementação clássico, pode instalar a versão de Gestão de Serviço do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="14164-145">If you have deployments that use the classic deployment model you can install the Service Management version of Azure PowerShell.</span></span> <span data-ttu-id="14164-146">Para obter mais informações, veja [Instalar o módulo Service Management do Azure PowerShell](/powershell/azure/servicemanagement/install-azure-ps).</span><span class="sxs-lookup"><span data-stu-id="14164-146">For more information, see [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span> <span data-ttu-id="14164-147">Os módulos Azure e AzureRM partilham dependências comuns.</span><span class="sxs-lookup"><span data-stu-id="14164-147">The Azure and AzureRM modules share common dependencies.</span></span> <span data-ttu-id="14164-148">Se utilizar os módulos do Azure e do AzureRM, deve instalar a mesma versão de cada pacote.</span><span class="sxs-lookup"><span data-stu-id="14164-148">If you use both the Azure and AzureRM modules, you should install the same version of each package.</span></span>

### <a id="update-azps"></a><span data-ttu-id="14164-149">Atualizar para a nova versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="14164-149">Updating to a new version of Azure PowerShell</span></span>

<span data-ttu-id="14164-150">Se tiver uma versão anterior do Azure PowerShell instalada, que inclui o módulo de Gestão de Serviço, poderá receber o erro seguinte:</span><span class="sxs-lookup"><span data-stu-id="14164-150">If you have a previous version of Azure PowerShell installed that includes the Service Management module, you may receive the following error:</span></span>

```
PackageManagement\Install-Package : A command with name 'Get-AzureStorageContainerAcl' is already
available on this system. This module 'Azure.Storage' may override the existing commands. If you
still want to install this module 'Azure.Storage', use -AllowClobber parameter.

At C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PSModule.psm1:1772 char:21
+ ...          $null = PackageManagement\Install-Package @PSBoundParameters
+                      ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : InvalidOperation: (Microsoft.Power....InstallPackage:InstallPackage) [Install-Package], Exception
    + FullyQualifiedErrorId : CommandAlreadyAvailable,Validate-ModuleCommandAlreadyAvailable,Microsoft.PowerShell.PackageManagement.Cmdlets.InstallPackage
```

<span data-ttu-id="14164-151">Como a mensagem de erro indica, tem de utilizar o parâmetro -AllowClobber para instalar o módulo.</span><span class="sxs-lookup"><span data-stu-id="14164-151">As the error message states, you need to use the -AllowClobber parameter to install the module.</span></span> <span data-ttu-id="14164-152">Utilize o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="14164-152">Use the following command:</span></span>

```powershell
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module AzureRM -AllowClobber
```

<span data-ttu-id="14164-153">Para mais informações, veja o tópico de ajuda para [Install-Module](https://msdn.microsoft.com/powershell/reference/5.1/PowerShellGet/install-module).</span><span class="sxs-lookup"><span data-stu-id="14164-153">For more information, see the help topic for [Install-Module](https://msdn.microsoft.com/powershell/reference/5.1/PowerShellGet/install-module).</span></span>

### <a name="installing-module-versions-side-by-side"></a><span data-ttu-id="14164-154">Instalar as versões do módulo lado a lado</span><span class="sxs-lookup"><span data-stu-id="14164-154">Installing module versions side by side</span></span>

<span data-ttu-id="14164-155">O método de instalação do PowerShellGet é o único método que suporta a instalação de várias versões.</span><span class="sxs-lookup"><span data-stu-id="14164-155">The PowerShellGet method of installation is the only method that supports the installation of multiple versions.</span></span> <span data-ttu-id="14164-156">Por exemplo, poderá ter scripts escritos utilizando uma versão anterior do Azure PowerShell Azure que não têm o tempo ou recursos atualizados.</span><span class="sxs-lookup"><span data-stu-id="14164-156">For example, you may have scripts written using a previous version of Azure PowerShell that you don't have the time or resources to updated.</span></span> <span data-ttu-id="14164-157">Os comandos seguintes ilustram como instalar várias versões do Azure PowerShell:</span><span class="sxs-lookup"><span data-stu-id="14164-157">The following commands illustrate how to install multiple versions of Azure PowerShell:</span></span>

```powershell
Install-Module -Name AzureRM -RequiredVersion 3.7.0
Install-Module -Name AzureRM -RequiredVersion 1.2.9
```

<span data-ttu-id="14164-158">Apenas uma versão do módulo pode ser carregada numa sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="14164-158">Only one version of the module can be loaded in a PowerShell session.</span></span> <span data-ttu-id="14164-159">Tem de abrir uma nova janela do PowerShell e utilizar `Import-Module` para importar uma versão específica dos cmdlets do AzureRM:</span><span class="sxs-lookup"><span data-stu-id="14164-159">You must open a new PowerShell window and use `Import-Module` to import a specific version of the AzureRM cmdlets:</span></span>

```powershell
Import-Module AzureRM -RequiredVersion 1.2.9
```

> [!NOTE]
> <span data-ttu-id="14164-160">A versão 2.1.0 e a versão 1.2.6 são as primeiras versões do módulo concebidas para serem instaladas e utilizadas lado a lado.</span><span class="sxs-lookup"><span data-stu-id="14164-160">Version 2.1.0 and version 1.2.6 are the first module versions designed to be installed and used side by side.</span></span> <span data-ttu-id="14164-161">Ao carregar uma versão anterior do Azure PowerShell, as versões incompatíveis do módulo **AzureRM.Profile** são carregadas.</span><span class="sxs-lookup"><span data-stu-id="14164-161">When loading an earlier version of the Azure PowerShell, incompatible versions of the **AzureRM.Profile** module are loaded.</span></span> <span data-ttu-id="14164-162">Isto resulta nos cmdlets solicitando que inicie sessão sempre executar um cmdlet.</span><span class="sxs-lookup"><span data-stu-id="14164-162">This results in the cmdlets prompting you to log in whenever you execute a cmdlet.</span></span>

### <a name="other-installation-methods"></a><span data-ttu-id="14164-163">Outros métodos de instalação</span><span class="sxs-lookup"><span data-stu-id="14164-163">Other installation methods</span></span>

<span data-ttu-id="14164-164">Para obter informações sobre a instalação com o Instalador de Plataforma Web ou o Pacote MSI, veja [Outros métodos de instalação](other-install.md)</span><span class="sxs-lookup"><span data-stu-id="14164-164">For information about installing using the Web Platform Installer or the MSI Package, see [Other installation methods](other-install.md)</span></span>
