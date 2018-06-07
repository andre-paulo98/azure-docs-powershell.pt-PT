---
title: Outros modos de instalação do Azure PowerShell | Microsoft Docs
description: Como instalar o Azure PowerShell através do pacote MSI ou do Instalador de Plataforma Web.
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/06/2017
ms.openlocfilehash: 354061987951728fd8a5802b01f3cb8b7c60a072
ms.sourcegitcommit: 2eea03b7ac19ad6d7c8097743d33c7ddb9c4df77
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/06/2018
ms.locfileid: "34820481"
---
# <a name="other-installation-methods"></a><span data-ttu-id="5f790-103">Outros métodos de instalação</span><span class="sxs-lookup"><span data-stu-id="5f790-103">Other installation methods</span></span>

<span data-ttu-id="5f790-104">O Azure PowerShell tem múltiplos métodos de instalação.</span><span class="sxs-lookup"><span data-stu-id="5f790-104">Azure PowerShell has multiple installation methods.</span></span> <span data-ttu-id="5f790-105">A utilização do PowerShellGet com a Galeria do PowerShell é o método preferencial.</span><span class="sxs-lookup"><span data-stu-id="5f790-105">Using PowerShellGet with the PowerShell Gallery is the preferred method.</span></span> <span data-ttu-id="5f790-106">O Azure PowerShell pode ser instalado no Windows através do Instalador de Plataforma Web (WebPI) ou do ficheiro MSI disponível a partir do GitHub.</span><span class="sxs-lookup"><span data-stu-id="5f790-106">Azure PowerShell can be installed on Windows using the Web Platform Installer (WebPI) or by using the MSI file available from GitHub.</span></span> <span data-ttu-id="5f790-107">O Azure PowerShell também pode ser instalado num contentor do Docker.</span><span class="sxs-lookup"><span data-stu-id="5f790-107">Azure PowerShell can also be installed in a Docker container.</span></span>

## <a name="install-on-windows-using-the-web-platform-installer"></a><span data-ttu-id="5f790-108">Instalar no Windows através do Instalador de Plataforma Web</span><span class="sxs-lookup"><span data-stu-id="5f790-108">Install on Windows using the Web Platform Installer</span></span>

<span data-ttu-id="5f790-109">Instalar o Azure PowerShell mais recente a partir do WebPI é o mesmo que para versões anteriores.</span><span class="sxs-lookup"><span data-stu-id="5f790-109">Installing the latest Azure PowerShell from WebPI is the same as it was for previous versions.</span></span>
<span data-ttu-id="5f790-110">Transfira o [pacote WebPI do Azure PowerShell](http://aka.ms/webpi-azps) e inicie a instalação.</span><span class="sxs-lookup"><span data-stu-id="5f790-110">Download the [Azure PowerShell WebPI package](http://aka.ms/webpi-azps) and start the install.</span></span>

> [!NOTE]
> <span data-ttu-id="5f790-111">Se tiver instalado anteriormente os módulos do Azure a partir da Galeria do PowerShell, o instalador irá removê-los automaticamente.</span><span class="sxs-lookup"><span data-stu-id="5f790-111">If you have previously installed Azure modules from the PowerShell Gallery, the installer automatically removes them.</span></span> <span data-ttu-id="5f790-112">Isto simplifica o seu ambiente ao assegurar que está instalada apenas uma versão do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5f790-112">This simplifies your environment by ensuring that only one version of Azure PowerShell is installed.</span></span> <span data-ttu-id="5f790-113">No entanto, existem cenários onde poderá precisar de múltiplas versões instaladas ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="5f790-113">However, there are scenarios where you may need multiple versions installed at the same time.</span></span>
>
> <span data-ttu-id="5f790-114">Os módulos da Galeria do PowerShell instalam módulos em `$env:ProgramFiles\WindowsPowerShell\Modules`.</span><span class="sxs-lookup"><span data-stu-id="5f790-114">PowerShell Gallery modules install modules in `$env:ProgramFiles\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="5f790-115">Em contrapartida, o instalador WebPI instalará os módulos do Azure em `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`.</span><span class="sxs-lookup"><span data-stu-id="5f790-115">In contrast, the WebPI installer installs the Azure modules in `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`.</span></span>
>
> <span data-ttu-id="5f790-116">Se ocorrer um erro durante a instalação, pode remover manualmente as pastas Azure\* na pasta `$env:ProgramFiles\WindowsPowerShell\Modules` e tentar efetuar novamente a instalação.</span><span class="sxs-lookup"><span data-stu-id="5f790-116">If an error occurs during install, you can manually remove the Azure\* folders in your `$env:ProgramFiles\WindowsPowerShell\Modules` folder, and try the installation again.</span></span>

<span data-ttu-id="5f790-117">Depois de concluída a instalação, a definição `$env:PSModulePath` deve incluir os diretórios que contêm os cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5f790-117">Once the installation completes, your `$env:PSModulePath` setting should include the directories containing the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="5f790-118">Pode ser utilizado o comando seguinte para verificar se o Azure PowerShell está instalado corretamente.</span><span class="sxs-lookup"><span data-stu-id="5f790-118">The following command can be used to verify that the Azure PowerShell is installed properly.</span></span>

```powershell
# To make sure the Azure PowerShell module is available after you install
Get-Module -ListAvailable Azure* | Select-Object Name, Version, Path
```

> [!NOTE]
> <span data-ttu-id="5f790-119">Existe um problema conhecido que pode ocorrer ao instalar a partir do WebPI.</span><span class="sxs-lookup"><span data-stu-id="5f790-119">There is a known issue that can occur when installing from WebPI.</span></span> <span data-ttu-id="5f790-120">Se o seu computador tiver de ser reiniciado devido a atualizações do sistema ou outras instalações, isto poderá provocar a falha das atualizações em `$env:PSModulePath` para incluir o caminho onde o Azure PowerShell está instalado.</span><span class="sxs-lookup"><span data-stu-id="5f790-120">If your computer requires a restart due to system updates or other installations, it may cause updates to `$env:PSModulePath` to fail to include the path where Azure PowerShell is installed.</span></span>

<span data-ttu-id="5f790-121">Ao tentar carregar ou executar os cmdlets após a instalação, pode receber a seguinte mensagem de erro:</span><span class="sxs-lookup"><span data-stu-id="5f790-121">When attempting to load or execute cmdlets after installation, you can receive the following error message:</span></span>

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

<span data-ttu-id="5f790-122">Este erro pode ser corrigido ao reiniciar o computador ou ao importar o módulo através do caminho totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="5f790-122">This error can be corrected by restarting the machine or importing the module using the fully qualified path.</span></span> <span data-ttu-id="5f790-123">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="5f790-123">For example:</span></span>

```powershell
Import-Module "$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\AzureRM.psd1"
```

## <a name="install-on-windows-using-the-msi-package"></a><span data-ttu-id="5f790-124">Instalar no Windows através do Pacote MSI</span><span class="sxs-lookup"><span data-stu-id="5f790-124">Install on Windows using the MSI Package</span></span>

<span data-ttu-id="5f790-125">O Azure PowerShell pode ser instalado através do ficheiro MSI disponível a partir do [GitHub](https://github.com/Azure/azure-powershell/releases/latest).</span><span class="sxs-lookup"><span data-stu-id="5f790-125">Azure PowerShell can be installed using the MSI file available from [GitHub](https://github.com/Azure/azure-powershell/releases/latest).</span></span> <span data-ttu-id="5f790-126">Se tiver versões anteriores dos módulos do Azure instaladas, o instalador remove-as automaticamente.</span><span class="sxs-lookup"><span data-stu-id="5f790-126">If you have installed previous versions of Azure modules, the installer automatically removes them.</span></span> <span data-ttu-id="5f790-127">O pacote MSI instala os módulos em `$env:ProgramFiles\WindowsPowerShell\Modules`, mas não cria pastas específicas da versão.</span><span class="sxs-lookup"><span data-stu-id="5f790-127">The MSI package installs modules in `$env:ProgramFiles\WindowsPowerShell\Modules` but does not create version-specific folders.</span></span>

## <a name="install-in-a-docker-container"></a><span data-ttu-id="5f790-128">Instalar num contentor do Docker</span><span class="sxs-lookup"><span data-stu-id="5f790-128">Install in a Docker container</span></span>

<span data-ttu-id="5f790-129">Mantemos uma imagem do Docker pré-configurada com o Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5f790-129">We maintain a Docker image preconfigured with Azure PowerShell.</span></span>

<span data-ttu-id="5f790-130">Execute o contentor com `docker run`.</span><span class="sxs-lookup"><span data-stu-id="5f790-130">Run the container with `docker run`.</span></span>

```powershell
docker run azuresdk/azure-powershell
```

<span data-ttu-id="5f790-131">Além disso, mantemos um subconjunto de cmdlets como contentor do PowerShell Core.</span><span class="sxs-lookup"><span data-stu-id="5f790-131">In addition, we maintain a subset of cmdlets as a PowerShell Core container.</span></span>

<span data-ttu-id="5f790-132">Para Mac/Linux, utilize a imagem `latest`.</span><span class="sxs-lookup"><span data-stu-id="5f790-132">For Mac/Linux, use the `latest` image.</span></span>

```bash
docker run azuresdk/azure-powershell-core:latest
```

<span data-ttu-id="5f790-133">Para Windows, utilize a imagem `nanoserver`.</span><span class="sxs-lookup"><span data-stu-id="5f790-133">For Windows, use the `nanoserver` image.</span></span>

```powershell
docker run azuresdk/azure-powershell-core:nanoserver
```

<span data-ttu-id="5f790-134">O Azure PowerShell está instalado na imagem através do `Install-Module` da [Galeria do PowerShell](https://www.powershellgallery.com/).</span><span class="sxs-lookup"><span data-stu-id="5f790-134">Azure PowerShell is installed on the image via `Install-Module` from the [PowerShell Gallery](https://www.powershellgallery.com/).</span></span>