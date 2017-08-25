---
title: "Outros modos de instalação do Azure PowerShell | Microsoft Docs"
description: "Como instalar o Azure PowerShell através do pacote MSI ou do Instalador de Plataforma Web."
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2017
ms.openlocfilehash: 9cee582f74b7f3260c6ae167a8ac358d360ad8ab
ms.sourcegitcommit: 45587b5091293288e16cfae8ac412e0d42f8f450
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/15/2017
---
# <a name="other-installation-methods"></a><span data-ttu-id="6c61d-103">Outros métodos de instalação</span><span class="sxs-lookup"><span data-stu-id="6c61d-103">Other installation methods</span></span>

<span data-ttu-id="6c61d-104">O Azure PowerShell tem múltiplos métodos de instalação.</span><span class="sxs-lookup"><span data-stu-id="6c61d-104">Azure PowerShell has multiple installation methods.</span></span> <span data-ttu-id="6c61d-105">A utilização do PowerShellGet com a Galeria do PowerShell é o método preferencial.</span><span class="sxs-lookup"><span data-stu-id="6c61d-105">Using PowerShellGet with the PowerShell Gallery is the preferred method.</span></span> <span data-ttu-id="6c61d-106">O Azure PowerShell pode ser instalado através do Instalador de Plataforma Web (WebPI) ou do ficheiro MSI disponível a partir do [GitHub](https://github.com/Azure/azure-powershell/releases/latest).</span><span class="sxs-lookup"><span data-stu-id="6c61d-106">Azure PowerShell can be installed using the Web Platform Installer (WebPI) or by using the MSI file available from [GitHub](https://github.com/Azure/azure-powershell/releases/latest).</span></span>

## <a name="docker"></a><span data-ttu-id="6c61d-107">Docker</span><span class="sxs-lookup"><span data-stu-id="6c61d-107">Docker</span></span>

<span data-ttu-id="6c61d-108">Mantemos uma imagem do Docker pré-configurada com o Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6c61d-108">We maintain a Docker image preconfigured with Azure PowerShell.</span></span>

<span data-ttu-id="6c61d-109">Execute o contentor com `docker run`.</span><span class="sxs-lookup"><span data-stu-id="6c61d-109">Run the container with `docker run`.</span></span>

```powershell
docker run azuresdk/azure-powershell
```

<span data-ttu-id="6c61d-110">Além disso, mantemos um subconjunto de cmdlets como contentor do PowerShell Core.</span><span class="sxs-lookup"><span data-stu-id="6c61d-110">In addition, we maintain a subset of cmdlets as a PowerShell Core container.</span></span>

<span data-ttu-id="6c61d-111">Para Mac/Linux, utilize a imagem `latest`.</span><span class="sxs-lookup"><span data-stu-id="6c61d-111">For Mac/Linux, use the `latest` image.</span></span>

```bash
docker run azuresdk/azure-powershell-core:latest
```

<span data-ttu-id="6c61d-112">Para Windows, utilize a imagem `nanoserver`.</span><span class="sxs-lookup"><span data-stu-id="6c61d-112">For Windows, use the `nanoserver` image.</span></span>

```powershell
docker run azuresdk/azure-powershell-core:nanoserver
```

<span data-ttu-id="6c61d-113">O Azure PowerShell está instalado na imagem através do `Install-Module` da [Galeria do PowerShell](https://www.powershellgallery.com/).</span><span class="sxs-lookup"><span data-stu-id="6c61d-113">Azure PowerShell is installed on the image via `Install-Module` from the [PowerShell Gallery](https://www.powershellgallery.com/).</span></span>

## <a name="install-using-the-web-platform-installer"></a><span data-ttu-id="6c61d-114">Instalar através do Instalador de Plataforma Web</span><span class="sxs-lookup"><span data-stu-id="6c61d-114">Install using the Web Platform Installer</span></span>

<span data-ttu-id="6c61d-115">Instalar o Azure PowerShell mais recente a partir do WebPI é o mesmo que para versões anteriores.</span><span class="sxs-lookup"><span data-stu-id="6c61d-115">Installing the latest Azure PowerShell from WebPI is the same as it was for previous versions.</span></span>
<span data-ttu-id="6c61d-116">Transfira o [pacote WebPI do Azure PowerShell](http://aka.ms/webpi-azps) e inicie a instalação.</span><span class="sxs-lookup"><span data-stu-id="6c61d-116">Download the [Azure PowerShell WebPI package](http://aka.ms/webpi-azps) and start the install.</span></span>

> [!NOTE]
> <span data-ttu-id="6c61d-117">Se tiver instalado anteriormente os módulos do Azure a partir da Galeria do PowerShell, o instalador irá removê-los automaticamente.</span><span class="sxs-lookup"><span data-stu-id="6c61d-117">If you have previously installed Azure modules from the PowerShell Gallery, the installer automatically removes them.</span></span> <span data-ttu-id="6c61d-118">Isto simplifica o seu ambiente ao assegurar que está instalada apenas uma versão do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6c61d-118">This simplifies your environment by ensuring that only one version of Azure PowerShell is installed.</span></span> <span data-ttu-id="6c61d-119">No entanto, existem cenários onde poderá precisar de múltiplas versões instaladas ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="6c61d-119">However, there are scenarios where you may need multiple versions installed at the same time.</span></span>
>
> <span data-ttu-id="6c61d-120">Os módulos da Galeria do PowerShell instalam módulos em `$env:ProgramFiles\WindowsPowerShell\Modules`.</span><span class="sxs-lookup"><span data-stu-id="6c61d-120">PowerShell Gallery modules install modules in `$env:ProgramFiles\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="6c61d-121">Em contrapartida, o instalador WebPI instalará os módulos do Azure em `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`.</span><span class="sxs-lookup"><span data-stu-id="6c61d-121">In contrast, the WebPI installer installs the Azure modules in `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`.</span></span>
>
> <span data-ttu-id="6c61d-122">Se ocorrer um erro durante a instalação, pode remover manualmente as pastas Azure* na pasta `$env:ProgramFiles\WindowsPowerShell\Modules` e tentar efetuar novamente a instalação.</span><span class="sxs-lookup"><span data-stu-id="6c61d-122">If an error occurs during install, you can manually remove the Azure* folders in your `$env:ProgramFiles\WindowsPowerShell\Modules` folder, and try the installation again.</span></span>

<span data-ttu-id="6c61d-123">Depois de concluída a instalação, a definição `$env:PSModulePath` deve incluir os diretórios que contêm os cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6c61d-123">Once the installation completes, your `$env:PSModulePath` setting should include the directories containing the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="6c61d-124">Pode ser utilizado o comando seguinte para verificar se o Azure PowerShell está instalado corretamente.</span><span class="sxs-lookup"><span data-stu-id="6c61d-124">The following command can be used to verify that the Azure PowerShell is installed properly.</span></span>

```powershell
# To make sure the Azure PowerShell module is available after you install
Get-Module -ListAvailable Azure* | Select-Object Name, Version, Path
```

> [!NOTE]
> <span data-ttu-id="6c61d-125">Existe um problema conhecido que pode ocorrer ao instalar a partir do WebPI.</span><span class="sxs-lookup"><span data-stu-id="6c61d-125">There is a known issue that can occur when installing from WebPI.</span></span> <span data-ttu-id="6c61d-126">Se o seu computador tiver de ser reiniciado devido a atualizações do sistema ou outras instalações, isto poderá provocar a falha das atualizações em `$env:PSModulePath` para incluir o caminho onde o Azure PowerShell está instalado.</span><span class="sxs-lookup"><span data-stu-id="6c61d-126">If your computer requires a restart due to system updates or other installations, it may cause updates to `$env:PSModulePath` to fail to include the path where Azure PowerShell is installed.</span></span>

<span data-ttu-id="6c61d-127">Ao tentar carregar ou executar os cmdlets após a instalação, pode receber a seguinte mensagem de erro:</span><span class="sxs-lookup"><span data-stu-id="6c61d-127">When attempting to load or execute cmdlets after installation, you can receive the following error message:</span></span>

```
PS C:\> Login-AzureRmAccount
Login-AzureRmAccount : The term 'Login-AzureRmAccount' is not recognized as the name of a cmdlet,
function, script file, or operable program. Check the spelling of the name, or if a path was
included, verify that the path is correct and try again.
At line:1 char:1
+ Login-AzureRmAccount
+ ~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (Login-AzureRmAccount:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
```

<span data-ttu-id="6c61d-128">Este erro pode ser corrigido ao reiniciar o computador ou ao importar o módulo através do caminho totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="6c61d-128">This error can be corrected by restarting the machine or importing the module using the fully qualified path.</span></span> <span data-ttu-id="6c61d-129">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="6c61d-129">For example:</span></span>

```powershell
Import-Module "$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\AzureRM.psd1"
```

## <a name="install-using-the-msi-package"></a><span data-ttu-id="6c61d-130">Instalar através do Pacote MSI</span><span class="sxs-lookup"><span data-stu-id="6c61d-130">Install using the MSI Package</span></span>

<span data-ttu-id="6c61d-131">O Azure PowerShell pode ser instalado através do ficheiro MSI disponível a partir do [GitHub](https://github.com/Azure/azure-powershell/releases/latest).</span><span class="sxs-lookup"><span data-stu-id="6c61d-131">Azure PowerShell can be installed using the MSI file available from [GitHub](https://github.com/Azure/azure-powershell/releases/latest).</span></span> <span data-ttu-id="6c61d-132">Se tiver versões anteriores dos módulos do Azure instaladas, o instalador remove-as automaticamente.</span><span class="sxs-lookup"><span data-stu-id="6c61d-132">If you have installed previous versions of Azure modules, the installer automatically removes them.</span></span> <span data-ttu-id="6c61d-133">O pacote MSI instala os módulos em `$env:ProgramFiles\WindowsPowerShell\Modules`, mas não cria pastas específicas da versão.</span><span class="sxs-lookup"><span data-stu-id="6c61d-133">The MSI package installs modules in `$env:ProgramFiles\WindowsPowerShell\Modules` but does not create version-specific folders.</span></span>
