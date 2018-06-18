---
title: Outras formas de instalar o Azure PowerShell
description: Como instalar o Azure PowerShell através do pacote MSI ou do Instalador de Plataforma Web.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 0919583d9cb05a75fae3b812eed84109be8b28aa
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323276"
---
# <a name="other-installation-methods"></a><span data-ttu-id="d2f6a-103">Outros métodos de instalação</span><span class="sxs-lookup"><span data-stu-id="d2f6a-103">Other installation methods</span></span>

<span data-ttu-id="d2f6a-104">Este artigo explica como instalar o Azure PowerShell com um pacote MSI ou o Instalador de Plataforma Web (WebPI).</span><span class="sxs-lookup"><span data-stu-id="d2f6a-104">This article explains how to install Azure PowerShell using an MSI or Web Platform Installer (WebPI).</span></span> <span data-ttu-id="d2f6a-105">Também pode executar o Azure PowerShell a partir de um contentor de Docker.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-105">You can also run Azure PowerShell from inside of a Docker container.</span></span> <span data-ttu-id="d2f6a-106">Utilize estes métodos de instalação apenas se forem necessários para o seu sistema.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-106">Use these installation methods only if they're necessary for your system.</span></span> <span data-ttu-id="d2f6a-107">A forma canónica de instalar o Azure PowerShell é através do PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-107">The canonical way to install Azure PowerShell is through PowerShellGet.</span></span> <span data-ttu-id="d2f6a-108">Para obter instruções sobre como utilizar o PowerShellGet para instalar o Azure PowerShell, veja [Instalar o Azure PowerShell com o PowerShellGet](install-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="d2f6a-108">For instructions on using PowerShellGet to install Azure PowerShell, see [Install Azure PowerShell with PowerShellGet](install-azurerm-ps.md).</span></span>

<span data-ttu-id="d2f6a-109">Para instalar em ambientes Linux ou macOS, veja [Instalar o Azure PowerShell no macOS ou Linux](install-azurermps-maclinux.md).</span><span class="sxs-lookup"><span data-stu-id="d2f6a-109">To install on Linux or macOS environments, see [Install Azure PowerShell on macOS or Linux](install-azurermps-maclinux.md).</span></span>

## <a name="install-or-update-on-windows-using-the-web-platform-installer"></a><span data-ttu-id="d2f6a-110">Instalar ou atualizar no Windows com o Instalador de Plataforma Web</span><span class="sxs-lookup"><span data-stu-id="d2f6a-110">Install or update on Windows using the Web Platform Installer</span></span>

<span data-ttu-id="d2f6a-111">Instalar o Azure PowerShell mais recente a partir do WebPI é o mesmo que para versões anteriores.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-111">Installing the latest Azure PowerShell from WebPI is the same as it was for previous versions.</span></span>
<span data-ttu-id="d2f6a-112">Transfira o [pacote WebPI do Azure PowerShell](http://aka.ms/webpi-azps) e inicie a instalação.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-112">Download the [Azure PowerShell WebPI package](http://aka.ms/webpi-azps) and start the install.</span></span>

> [!NOTE]
> <span data-ttu-id="d2f6a-113">Se tiver instalado anteriormente os módulos do Azure a partir da Galeria do PowerShell, o instalador irá removê-los automaticamente.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-113">If you have previously installed Azure modules from the PowerShell Gallery, the installer automatically removes them.</span></span> <span data-ttu-id="d2f6a-114">Isto simplifica o seu ambiente ao assegurar que está instalada apenas uma versão do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-114">This simplifies your environment by ensuring that only one version of Azure PowerShell is installed.</span></span> <span data-ttu-id="d2f6a-115">No entanto, existem cenários onde poderá precisar de múltiplas versões instaladas ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-115">However, there are scenarios where you may need multiple versions installed at the same time.</span></span>
>
> <span data-ttu-id="d2f6a-116">Os módulos da Galeria do PowerShell instalam módulos em `$env:ProgramFiles\WindowsPowerShell\Modules`.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-116">PowerShell Gallery modules install modules in `$env:ProgramFiles\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="d2f6a-117">Em contrapartida, o instalador WebPI instalará os módulos do Azure em `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-117">In contrast, the WebPI installer installs the Azure modules in `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`.</span></span>
>
> <span data-ttu-id="d2f6a-118">Se ocorrer um erro durante a instalação, pode remover manualmente as pastas `Azure*` na pasta `$env:ProgramFiles\WindowsPowerShell\Modules` e tentar instalar novamente.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-118">If an error occurs during install, you can manually remove the `Azure*` folders in your `$env:ProgramFiles\WindowsPowerShell\Modules` folder, and try the installation again.</span></span>

<span data-ttu-id="d2f6a-119">Depois de concluída a instalação, a definição `$env:PSModulePath` deve incluir os diretórios que contêm os cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-119">Once the installation completes, your `$env:PSModulePath` setting should include the directories containing the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="d2f6a-120">O comando que se segue pode ser utilizado para verificar se o Azure PowerShell está instalado corretamente:</span><span class="sxs-lookup"><span data-stu-id="d2f6a-120">The following command can be used to verify that the Azure PowerShell is installed properly:</span></span>

```powershell
# To make sure the Azure PowerShell module is available after you install
Get-Module -ListAvailable Azure* | Select-Object Name, Version, Path
```

> [!NOTE]
> <span data-ttu-id="d2f6a-121">Existe um problema conhecido que pode ocorrer ao instalar a partir do WebPI.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-121">There is a known issue that can occur when installing from WebPI.</span></span> <span data-ttu-id="d2f6a-122">Se o seu computador tiver de ser reiniciado devido a atualizações do sistema ou outras instalações, isto poderá provocar a falha das atualizações em `$env:PSModulePath` para incluir o caminho onde o Azure PowerShell está instalado.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-122">If your computer requires a restart due to system updates or other installations, it may cause updates to `$env:PSModulePath` to fail to include the path where Azure PowerShell is installed.</span></span>

<span data-ttu-id="d2f6a-123">Ao tentar carregar ou executar os cmdlets após a instalação, pode receber a seguinte mensagem de erro:</span><span class="sxs-lookup"><span data-stu-id="d2f6a-123">When attempting to load or execute cmdlets after installation, you can receive the following error message:</span></span>

```
PS C:\> Connect-AzureRmAccount
Connect-AzureRmAccount : The term 'Connect-AzureRmAccount' is not recognized as the name of a cmdlet,
function, script file, or operable program. Check the spelling of the name, or if a path was
included, verify that the path is correct and try again.
At line:1 char:1
+ Connect-AzureRmAccount
+ ~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (Connect-AzureRmAccount:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
```

<span data-ttu-id="d2f6a-124">Este erro pode ser corrigido ao reiniciar o computador ou ao importar o módulo através do caminho totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-124">This error can be corrected by restarting the machine or importing the module using the fully qualified path.</span></span>

```powershell
Import-Module "$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\AzureRM.psd1"
```

## <a name="install-or-update-on-windows-using-the-msi-package"></a><span data-ttu-id="d2f6a-125">Instalar ou atualizar no Windows com o Pacote MSI</span><span class="sxs-lookup"><span data-stu-id="d2f6a-125">Install or update on Windows using the MSI Package</span></span>

<span data-ttu-id="d2f6a-126">O Azure PowerShell pode ser instalado através do ficheiro MSI disponível a partir do [GitHub](https://aka.ms/azps-release).</span><span class="sxs-lookup"><span data-stu-id="d2f6a-126">Azure PowerShell can be installed using the MSI file available from [GitHub](https://aka.ms/azps-release).</span></span> <span data-ttu-id="d2f6a-127">Se tiver versões anteriores dos módulos do Azure instaladas, o instalador remove-as automaticamente.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-127">If you have installed previous versions of Azure modules, the installer automatically removes them.</span></span> <span data-ttu-id="d2f6a-128">O pacote MSI instala os módulos em `$env:ProgramFiles\WindowsPowerShell\Modules`, mas não cria pastas específicas da versão.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-128">The MSI package installs modules in `$env:ProgramFiles\WindowsPowerShell\Modules` but does not create version-specific folders.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="d2f6a-129">Executar num contentor do Docker</span><span class="sxs-lookup"><span data-stu-id="d2f6a-129">Run in a Docker container</span></span>

<span data-ttu-id="d2f6a-130">Mantemos um conjunto de imagens do Docker pré-configuradas com o Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-130">We maintain a set of Docker images preconfigured with Azure PowerShell.</span></span> <span data-ttu-id="d2f6a-131">Existem dois tipos de contentor disponíveis: contentores com o PowerShell tradicional em execução no Windows e um contentor com o PowerShell Core em execução no Windows ou Linux.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-131">There are two types of containers available: Those running traditional PowerShell on Windows, and a container running PowerShell Core on either Windows or Linux.</span></span>

| <span data-ttu-id="d2f6a-132">Ambiente</span><span class="sxs-lookup"><span data-stu-id="d2f6a-132">Environment</span></span> | <span data-ttu-id="d2f6a-133">Imagem do Docker</span><span class="sxs-lookup"><span data-stu-id="d2f6a-133">Docker image</span></span> |
|-------------|--------------|
| <span data-ttu-id="d2f6a-134">PowerShell no Windows</span><span class="sxs-lookup"><span data-stu-id="d2f6a-134">PowerShell on Windows</span></span> | [<span data-ttu-id="d2f6a-135">azuresdk/azure-powershell</span><span class="sxs-lookup"><span data-stu-id="d2f6a-135">azuresdk/azure-powershell</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| <span data-ttu-id="d2f6a-136">PowerShell Core no Windows</span><span class="sxs-lookup"><span data-stu-id="d2f6a-136">PowerShell Core on Windows</span></span> | [<span data-ttu-id="d2f6a-137">azuresdk/azure-powershell-core:nanoserver</span><span class="sxs-lookup"><span data-stu-id="d2f6a-137">azuresdk/azure-powershell-core:nanoserver</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| <span data-ttu-id="d2f6a-138">PowerShell Core no Linux</span><span class="sxs-lookup"><span data-stu-id="d2f6a-138">PowerShell Core on Linux</span></span> | [<span data-ttu-id="d2f6a-139">azuresdk/azure-powershell-core:latest</span><span class="sxs-lookup"><span data-stu-id="d2f6a-139">azuresdk/azure-powershell-core:latest</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

<span data-ttu-id="d2f6a-140">Para executar qualquer um destes contentores, utilize `docker run -it $ImageName` para obter um terminal interativo.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-140">To run any of these containers, you use `docker run -it $ImageName` to get an interactive terminal.</span></span> <span data-ttu-id="d2f6a-141">Por exemplo, para executar o PowerShell Core no contentor do Linux, utilize:</span><span class="sxs-lookup"><span data-stu-id="d2f6a-141">For example, to run the PowerShell Core on Linux container, use:</span></span>

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> <span data-ttu-id="d2f6a-142">Para executar um contentor do Windows no Docker, o SO anfitrião tem de ser o Windows e o Docker tem de estar definido para executar contentores do Windows.</span><span class="sxs-lookup"><span data-stu-id="d2f6a-142">To run a Windows container in Docker, your host OS must be Windows and Docker must be set to run Windows containers.</span></span> <span data-ttu-id="d2f6a-143">Para saber mais sobre como alternar entre os ambientes Windows e Linux no Docker, veja a documentação do Docker [Alternar entre os contentores do Windows e do Linux](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers).</span><span class="sxs-lookup"><span data-stu-id="d2f6a-143">To learn about switching between Windows and Linux environments in Docker, see the Docker documentation [Switch between Windows and Linux containers](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers).</span></span>