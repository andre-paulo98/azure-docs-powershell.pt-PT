---
title: Instalar e configurar o Azure PowerShell | Microsoft Docs
description: Como instalar e configurar o Azure PowerShell para uma primeira utilização.
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/27/2018
ms.openlocfilehash: c6b8e2e8aa4afb9e58a2d357c4e51e19410a8188
ms.sourcegitcommit: 37bfbf11fd0967a8e7977c692ab829d286baf88a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/08/2018
ms.locfileid: "33913612"
---
# <a name="install-and-configure-azure-powershell"></a><span data-ttu-id="bd301-103">Instalar e configurar o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="bd301-103">Install and configure Azure PowerShell</span></span>

<span data-ttu-id="bd301-104">Este artigo explica os passos para instalar os módulos do Azure PowerShell no ambiente do Windows.</span><span class="sxs-lookup"><span data-stu-id="bd301-104">This article explains the steps to install the Azure PowerShell modules in a Windows environment.</span></span>
<span data-ttu-id="bd301-105">Se quiser utilizar o Azure PowerShell no macOS ou Linux, veja o seguinte artigo: [Instalar e configurar o Azure PowerShell no macOS e Linux](install-azurermps-maclinux.md).</span><span class="sxs-lookup"><span data-stu-id="bd301-105">If you want to use Azure PowerShell on macOS or Linux, see the following article: [Install and configure Azure PowerShell on macOS and Linux](install-azurermps-maclinux.md).</span></span>

## <a name="system-requirements"></a><span data-ttu-id="bd301-106">Requisitos de sistema</span><span class="sxs-lookup"><span data-stu-id="bd301-106">System requirements</span></span>

<span data-ttu-id="bd301-107">A versão do Azure PowerShell 6.0.0 exige a versão 5.0 (ou superior) do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bd301-107">Azure PowerShell version 6.0.0 requires version 5.0 (or higher) of PowerShell.</span></span> <span data-ttu-id="bd301-108">As versões anteriores do Azure PowerShell exigiram, _pelo menos_, a versão 3.0 do PowerShell para executar qualquer cmdlet. Para obter informações sobre a atualização para o PowerShell 5.0, veja [esta tabela](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="bd301-108">Previous versions of Azure PowerShell required _at least_ version 3.0 of PowerShell to run any cmdlet.For information on upgrading to PowerShell 5.0, please see [this table](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell).</span></span>

## <a name="step-1-install-powershellget"></a><span data-ttu-id="bd301-109">Passo 1: Instalar o PowerShellGet</span><span class="sxs-lookup"><span data-stu-id="bd301-109">Step 1: Install PowerShellGet</span></span>

<span data-ttu-id="bd301-110">Instalar o Azure PowerShell a partir da Galeria do PowerShell é o método de instalação preferencial.</span><span class="sxs-lookup"><span data-stu-id="bd301-110">Installing Azure PowerShell from the PowerShell Gallery is the preferred method of installation.</span></span>

<span data-ttu-id="bd301-111">A instalação de itens a partir da Galeria do PowerShell requer o módulo PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="bd301-111">Installing items from the PowerShell Gallery requires the PowerShellGet module.</span></span> <span data-ttu-id="bd301-112">Certifique-se de que tem a versão adequada do PowerShellGet e outros requisitos de sistema.</span><span class="sxs-lookup"><span data-stu-id="bd301-112">Make sure you have the appropriate version of PowerShellGet and other system requirements.</span></span> <span data-ttu-id="bd301-113">Execute o seguinte comando para ver se tem o PowerShellGet instalado no sistema.</span><span class="sxs-lookup"><span data-stu-id="bd301-113">Run the following command to see if you have PowerShellGet installed on your system.</span></span>

```powershell
Get-Module -Name PowerShellGet -ListAvailable | Select-Object -Property Name,Version,Path
```

<span data-ttu-id="bd301-114">Deverá ver algo semelhante à saída seguinte:</span><span class="sxs-lookup"><span data-stu-id="bd301-114">You should see something similar to the following output:</span></span>

```Output
Name          Version Path
----          ------- ----
Name          Version Path
----          ------- ----
PowerShellGet 1.6.0   C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.6.0\PowerShellGet.psd1
PowerShellGet 1.0.0.1 C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PowerShellGet.psd1
```

<span data-ttu-id="bd301-115">Precisa da versão 1.1.2.0 ou superior do PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="bd301-115">You need PowerShellGet version 1.1.2.0 or higher.</span></span> <span data-ttu-id="bd301-116">Para atualizar o PowerShellGet, utilize o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="bd301-116">To update PowerShellGet, use the following command:</span></span>

```powershell
Install-Module PowerShellGet -Force
```

<span data-ttu-id="bd301-117">Se não tiver o PowerShellGet instalado, veja a secção [Como obter o PowerShellGet](#how-to-get-powershellget) deste artigo.</span><span class="sxs-lookup"><span data-stu-id="bd301-117">If you do not have PowerShellGet installed, see the [How to get PowerShellGet](#how-to-get-powershellget) section of this article.</span></span>

> [!NOTE]
> <span data-ttu-id="bd301-118">A utilização do PowerShellGet requer uma Política de Execução que lhe permita executar scripts.</span><span class="sxs-lookup"><span data-stu-id="bd301-118">Using PowerShellGet requires an Execution Policy that allows you to run scripts.</span></span> <span data-ttu-id="bd301-119">Para obter mais informações sobre a Política de Execução do PowerShell, veja [About Execution Policies (Sobre as Políticas de Execução)](/powershell/module/microsoft.powershell.core/about/about_execution_policies).</span><span class="sxs-lookup"><span data-stu-id="bd301-119">For more information about PowerShell's Execution Policy, see [About Execution Policies](/powershell/module/microsoft.powershell.core/about/about_execution_policies).</span></span>

## <a name="step-2-install-azure-powershell"></a><span data-ttu-id="bd301-120">Passo 2: Instalar o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="bd301-120">Step 2: Install Azure PowerShell</span></span>

<span data-ttu-id="bd301-121">Instalar o Azure PowerShell a partir da Galeria do PowerShell requer privilégios elevados.</span><span class="sxs-lookup"><span data-stu-id="bd301-121">Installing Azure PowerShell from the PowerShell Gallery requires elevated privileges.</span></span> <span data-ttu-id="bd301-122">Execute o seguinte comando a partir de uma sessão do PowerShell elevada:</span><span class="sxs-lookup"><span data-stu-id="bd301-122">Run the following command from an elevated PowerShell session:</span></span>

```powershell
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module -Name AzureRM -AllowClobber
```

<span data-ttu-id="bd301-123">Por predefinição, a galeria do PowerShell não está configurada como um repositório Fidedigno para PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="bd301-123">By default, the PowerShell gallery is not configured as a Trusted repository for PowerShellGet.</span></span> <span data-ttu-id="bd301-124">Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:</span><span class="sxs-lookup"><span data-stu-id="bd301-124">The first time you use the PSGallery you see the following prompt:</span></span>

```Output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"): Y
```

<span data-ttu-id="bd301-125">Responder "Sim" ou "Sim a Todos" para continuar com a instalação.</span><span class="sxs-lookup"><span data-stu-id="bd301-125">Answer 'Yes' or 'Yes to All' to continue with the installation.</span></span>

> [!NOTE]
> <span data-ttu-id="bd301-126">Se tiver uma versão mais antiga do que a 2.8.5.201 do NuGet, será pedido que transfira e instale a versão mais recente do NuGet.</span><span class="sxs-lookup"><span data-stu-id="bd301-126">If you have a version older than 2.8.5.201 of NuGet, you are prompted to download and install the latest version of NuGet.</span></span>

<span data-ttu-id="bd301-127">O módulo de AzureRM é um módulo de rollup para os cmdlets do Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="bd301-127">The AzureRM module is a rollup module for the Azure Resource Manager cmdlets.</span></span> <span data-ttu-id="bd301-128">Quando instala o módulo AzureRM, qualquer outro módulo do Azure PowerShell que não tenha sido anteriormente instalado será transferido a partir da Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bd301-128">When you install the AzureRM module, any Azure PowerShell module not previously installed is downloaded and from the PowerShell Gallery.</span></span>

<span data-ttu-id="bd301-129">Se tiver uma versão anterior do Azure PowerShell instalado poderá receber um erro.</span><span class="sxs-lookup"><span data-stu-id="bd301-129">If you have a previous version of Azure PowerShell installed you may receive an error.</span></span> <span data-ttu-id="bd301-130">Para resolver este problema, veja a secção [Updating to a new version of Azure PowerShell](#update-azps)(Atualizar para uma versão nova do Azure PowerShell) deste artigo.</span><span class="sxs-lookup"><span data-stu-id="bd301-130">To resolve this issue, see the [Updating to a new version of Azure PowerShell](#update-azps) section of this article.</span></span>

## <a name="step-3-load-the-azurerm-module"></a><span data-ttu-id="bd301-131">Passo 3: carregar o módulo de AzureRM</span><span class="sxs-lookup"><span data-stu-id="bd301-131">Step 3: Load the AzureRM module</span></span>
<span data-ttu-id="bd301-132">Uma vez que o módulo seja instalado, terá de carregar o módulo para a sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bd301-132">Once the module is installed, you need to load the module into your PowerShell session.</span></span> <span data-ttu-id="bd301-133">Deve fazê-lo numa sessão normal (não avaliada) do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bd301-133">You should do this in a normal (non-elevated) PowerShell session.</span></span> <span data-ttu-id="bd301-134">Os módulos são carregados com o cmdlet `Import-Module`, da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="bd301-134">Modules are loaded using the `Import-Module` cmdlet, as follows:</span></span>

```powershell
Import-Module -Name AzureRM
```

## <a name="next-steps"></a><span data-ttu-id="bd301-135">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="bd301-135">Next Steps</span></span>

<span data-ttu-id="bd301-136">Para mais informações sobre como utilizar o Azure PowerShell, consulte os artigos seguintes:</span><span class="sxs-lookup"><span data-stu-id="bd301-136">For more information about using Azure PowerShell, see the following articles:</span></span>

* [<span data-ttu-id="bd301-137">Introdução ao Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="bd301-137">Get started with Azure PowerShell</span></span>](get-started-azureps.md)

## <a name="reporting-issues-and-feedback"></a><span data-ttu-id="bd301-138">Comunicar problemas e comentários</span><span class="sxs-lookup"><span data-stu-id="bd301-138">Reporting issues and feedback</span></span>

<span data-ttu-id="bd301-139">Se encontrar quaisquer erros com a ferramenta, comunique o assunto na secção [Problemas](https://github.com/Azure/azure-powershell/issues) do nosso repositório do GitHub.</span><span class="sxs-lookup"><span data-stu-id="bd301-139">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-powershell/issues) section of our GitHub repo.</span></span> <span data-ttu-id="bd301-140">Para enviar comentários a partir da linha de comandos, experimente o cmdlet `Send-Feedback`.</span><span class="sxs-lookup"><span data-stu-id="bd301-140">To provide feedback from the command line, use the `Send-Feedback` cmdlet.</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="bd301-141">Perguntas mais frequentes</span><span class="sxs-lookup"><span data-stu-id="bd301-141">Frequently asked questions</span></span>

### <a name="how-to-get-powershellget"></a><span data-ttu-id="bd301-142">Como obter o PowerShellGet</span><span class="sxs-lookup"><span data-stu-id="bd301-142">How to get PowerShellGet</span></span>

|<span data-ttu-id="bd301-143">Cenário</span><span class="sxs-lookup"><span data-stu-id="bd301-143">Scenario</span></span>|<span data-ttu-id="bd301-144">Instruções de instalação</span><span class="sxs-lookup"><span data-stu-id="bd301-144">Install instructions</span></span>|
|---|---|
|<span data-ttu-id="bd301-145">Windows 10</span><span class="sxs-lookup"><span data-stu-id="bd301-145">Windows 10</span></span><br/><span data-ttu-id="bd301-146">Windows Server 2016</span><span class="sxs-lookup"><span data-stu-id="bd301-146">Windows Server 2016</span></span>|<span data-ttu-id="bd301-147">Incorporado no Windows Management Framework (WMF) 5.0 incluído no SO</span><span class="sxs-lookup"><span data-stu-id="bd301-147">Built into Windows Management Framework (WMF) 5.0 included in the OS</span></span>|
|<span data-ttu-id="bd301-148">Quero atualizar para o PowerShell 5</span><span class="sxs-lookup"><span data-stu-id="bd301-148">I want to upgrade to PowerShell 5</span></span>|<ol><li>[<span data-ttu-id="bd301-149">Instalar a versão mais recente do WMF</span><span class="sxs-lookup"><span data-stu-id="bd301-149">Install the latest version of WMF</span></span>](https://www.microsoft.com/en-us/download/details.aspx?id=54616)</li><li><span data-ttu-id="bd301-150">Execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="bd301-150">Run the following command:</span></span><br/>```Install-Module PowerShellGet -Force```</li></ol>|
|<span data-ttu-id="bd301-151">Estou a executar uma versão do Windows com o PowerShell 3 ou o PowerShell 4</span><span class="sxs-lookup"><span data-stu-id="bd301-151">I am running on a version of Windows with PowerShell 3 or PowerShell 4</span></span>|<ol><span data-ttu-id="bd301-152"><il>[Obter os módulos PackageManagement](http://go.microsoft.com/fwlink/?LinkID=746217)</il></span><span class="sxs-lookup"><span data-stu-id="bd301-152"><il>[Get the PackageManagement modules](http://go.microsoft.com/fwlink/?LinkID=746217)</il></span></span><li><span data-ttu-id="bd301-153">Execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="bd301-153">Run the following command:</span></span><br/>```Install-Module PowerShellGet -Force```</li></ol>|

<a id="helpmechoose"></a>
### <a name="checking-the-version-of-azure-powershell"></a><span data-ttu-id="bd301-154">A verificar a versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="bd301-154">Checking the version of Azure PowerShell</span></span>

<span data-ttu-id="bd301-155">Embora o aconselhemos a atualizar para a versão mais recente o mais cedo possível, são suportadas várias versões do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bd301-155">Although we encourage you to upgrade to the latest version as early as possible, several versions of Azure PowerShell are supported.</span></span> <span data-ttu-id="bd301-156">Para determinar a versão do Azure PowerShell que tem instalada, execute `Get-Module AzureRM` a partir da linha de comandos.</span><span class="sxs-lookup"><span data-stu-id="bd301-156">To determine the version of Azure PowerShell you have installed, run `Get-Module AzureRM` from your command line.</span></span>

```powershell
Get-Module AzureRM -ListAvailable | Select-Object -Property Name,Version,Path
```

### <a name="support-for-classic-deployment-methods"></a><span data-ttu-id="bd301-157">Suporte para os métodos de implementação clássicos</span><span class="sxs-lookup"><span data-stu-id="bd301-157">Support for classic deployment methods</span></span>

<span data-ttu-id="bd301-158">Se tiver implementações que utilizam o modelo de implementação clássico, pode instalar a versão de Gestão de Serviço do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bd301-158">If you have deployments that use the classic deployment model you can install the Service Management version of Azure PowerShell.</span></span> <span data-ttu-id="bd301-159">Para obter mais informações, veja [Instalar o módulo Service Management do Azure PowerShell](/powershell/azure/servicemanagement/install-azure-ps).</span><span class="sxs-lookup"><span data-stu-id="bd301-159">For more information, see [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span> <span data-ttu-id="bd301-160">Os módulos Azure e AzureRM partilham dependências comuns.</span><span class="sxs-lookup"><span data-stu-id="bd301-160">The Azure and AzureRM modules share common dependencies.</span></span> <span data-ttu-id="bd301-161">Se utilizar os módulos do Azure e do AzureRM, deve instalar a mesma versão de cada pacote.</span><span class="sxs-lookup"><span data-stu-id="bd301-161">If you use both the Azure and AzureRM modules, you should install the same version of each package.</span></span>

### <a id="update-azps"></a><span data-ttu-id="bd301-162">Atualizar para a nova versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="bd301-162">Updating to a new version of Azure PowerShell</span></span>

<span data-ttu-id="bd301-163">Se tiver uma versão anterior do Azure PowerShell instalada, que inclui o módulo de Gestão de Serviço, poderá receber o erro seguinte:</span><span class="sxs-lookup"><span data-stu-id="bd301-163">If you have a previous version of Azure PowerShell installed that includes the Service Management module, you may receive the following error:</span></span>

```Output
PackageManagement\Install-Package : A command with name 'Get-AzureStorageContainerAcl' is already
available on this system. This module 'Azure.Storage' may override the existing commands. If you
still want to install this module 'Azure.Storage', use -AllowClobber parameter.

At C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PSModule.psm1:1772 char:21
+ ...          $null = PackageManagement\Install-Package @PSBoundParameters
+                      ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : InvalidOperation: (Microsoft.Power....InstallPackage:InstallPackage) [Install-Package], Exception
    + FullyQualifiedErrorId : CommandAlreadyAvailable,Validate-ModuleCommandAlreadyAvailable,Microsoft.PowerShell.PackageManagement.Cmdlets.InstallPackage
```

<span data-ttu-id="bd301-164">Como a mensagem de erro indica, tem de utilizar o parâmetro -AllowClobber para instalar o módulo.</span><span class="sxs-lookup"><span data-stu-id="bd301-164">As the error message states, you need to use the -AllowClobber parameter to install the module.</span></span> <span data-ttu-id="bd301-165">Utilize o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="bd301-165">Use the following command:</span></span>

```powershell
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module -Name AzureRM -AllowClobber
```

<span data-ttu-id="bd301-166">Para mais informações, veja o tópico de ajuda para [Install-Module](https://msdn.microsoft.com/powershell/reference/5.1/PowerShellGet/install-module).</span><span class="sxs-lookup"><span data-stu-id="bd301-166">For more information, see the help topic for [Install-Module](https://msdn.microsoft.com/powershell/reference/5.1/PowerShellGet/install-module).</span></span>

### <a name="installing-module-versions-side-by-side"></a><span data-ttu-id="bd301-167">Instalar as versões do módulo lado a lado</span><span class="sxs-lookup"><span data-stu-id="bd301-167">Installing module versions side by side</span></span>

<span data-ttu-id="bd301-168">O método de instalação do PowerShellGet é o único método que suporta a instalação de várias versões.</span><span class="sxs-lookup"><span data-stu-id="bd301-168">The PowerShellGet method of installation is the only method that supports the installation of multiple versions.</span></span> <span data-ttu-id="bd301-169">Por exemplo, poderá ter scripts escritos utilizando uma versão anterior do Azure PowerShell Azure que não têm o tempo ou recursos atualizados.</span><span class="sxs-lookup"><span data-stu-id="bd301-169">For example, you may have scripts written using a previous version of Azure PowerShell that you don't have the time or resources to updated.</span></span> <span data-ttu-id="bd301-170">Os comandos seguintes ilustram como instalar várias versões do Azure PowerShell:</span><span class="sxs-lookup"><span data-stu-id="bd301-170">The following commands illustrate how to install multiple versions of Azure PowerShell:</span></span>

```powershell
Install-Module -Name AzureRM -RequiredVersion 3.7.0
Install-Module -Name AzureRM -RequiredVersion 1.2.9
```

<span data-ttu-id="bd301-171">Apenas uma versão do módulo pode ser carregada numa sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bd301-171">Only one version of the module can be loaded in a PowerShell session.</span></span> <span data-ttu-id="bd301-172">Tem de abrir uma nova janela do PowerShell e utilizar `Import-Module` para importar uma versão específica dos cmdlets do AzureRM:</span><span class="sxs-lookup"><span data-stu-id="bd301-172">You must open a new PowerShell window and use `Import-Module` to import a specific version of the AzureRM cmdlets:</span></span>

```powershell
Import-Module -Name AzureRM -RequiredVersion 1.2.9
```

> [!NOTE]
> <span data-ttu-id="bd301-173">A versão 2.1.0 e a versão 1.2.6 são as primeiras versões do módulo concebidas para serem instaladas e utilizadas lado a lado.</span><span class="sxs-lookup"><span data-stu-id="bd301-173">Version 2.1.0 and version 1.2.6 are the first module versions designed to be installed and used side by side.</span></span> <span data-ttu-id="bd301-174">Ao carregar uma versão anterior do Azure PowerShell, as versões incompatíveis do módulo **AzureRM.Profile** são carregadas.</span><span class="sxs-lookup"><span data-stu-id="bd301-174">When loading an earlier version of the Azure PowerShell, incompatible versions of the **AzureRM.Profile** module are loaded.</span></span> <span data-ttu-id="bd301-175">Isto resulta nos cmdlets solicitando que inicie sessão sempre executar um cmdlet.</span><span class="sxs-lookup"><span data-stu-id="bd301-175">This results in the cmdlets prompting you to log in whenever you execute a cmdlet.</span></span>

### <a name="other-installation-methods"></a><span data-ttu-id="bd301-176">Outros métodos de instalação</span><span class="sxs-lookup"><span data-stu-id="bd301-176">Other installation methods</span></span>

<span data-ttu-id="bd301-177">Para obter informações sobre a instalação com o Instalador de Plataforma Web ou o Pacote MSI, veja [Outros métodos de instalação](other-install.md)</span><span class="sxs-lookup"><span data-stu-id="bd301-177">For information about installing using the Web Platform Installer or the MSI Package, see [Other installation methods](other-install.md)</span></span>
