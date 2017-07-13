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
ms.openlocfilehash: 368404bcb5218814b4965bb1bcda1e2876441d2a
ms.sourcegitcommit: 226527be7cb647acfe2ea9ab151185053ab3c6db
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/29/2017
---
# <span data-ttu-id="b23db-103">Outros métodos de instalação</span><span class="sxs-lookup"><span data-stu-id="b23db-103">Other installation methods</span></span>
<a id="other-installation-methods" class="xliff"></a>

<span data-ttu-id="b23db-104">O Azure PowerShell tem múltiplos métodos de instalação.</span><span class="sxs-lookup"><span data-stu-id="b23db-104">Azure PowerShell has multiple installation methods.</span></span> <span data-ttu-id="b23db-105">A utilização do PowerShellGet com a Galeria do PowerShell é o método preferencial.</span><span class="sxs-lookup"><span data-stu-id="b23db-105">Using PowerShellGet with the PowerShell Gallery is the preferred method.</span></span> <span data-ttu-id="b23db-106">O Azure PowerShell pode ser instalado através do Instalador de Plataforma Web (WebPI) ou do ficheiro MSI disponível a partir do [GitHub](https://github.com/Azure/azure-powershell/releases/latest).</span><span class="sxs-lookup"><span data-stu-id="b23db-106">Azure PowerShell can be installed using the Web Platform Installer (WebPI) or by using the MSI file available from [GitHub](https://github.com/Azure/azure-powershell/releases/latest).</span></span>

## <span data-ttu-id="b23db-107">Instalar através do Instalador de Plataforma Web</span><span class="sxs-lookup"><span data-stu-id="b23db-107">Install using the Web Platform Installer</span></span>
<a id="install-using-the-web-platform-installer" class="xliff"></a>

<span data-ttu-id="b23db-108">Instalar o Azure PowerShell mais recente a partir do WebPI é o mesmo que para versões anteriores.</span><span class="sxs-lookup"><span data-stu-id="b23db-108">Installing the latest Azure PowerShell from WebPI is the same as it was for previous versions.</span></span>
<span data-ttu-id="b23db-109">Transfira o [pacote WebPI do Azure PowerShell](http://aka.ms/webpi-azps) e inicie a instalação.</span><span class="sxs-lookup"><span data-stu-id="b23db-109">Download the [Azure PowerShell WebPI package](http://aka.ms/webpi-azps) and start the install.</span></span>

> [!NOTE]
> <span data-ttu-id="b23db-110">Se tiver instalado anteriormente os módulos do Azure a partir da Galeria do PowerShell, o instalador irá removê-los automaticamente.</span><span class="sxs-lookup"><span data-stu-id="b23db-110">If you have previously installed Azure modules from the PowerShell Gallery, the installer automatically removes them.</span></span> <span data-ttu-id="b23db-111">Isto simplifica o seu ambiente ao assegurar que está instalada apenas uma versão do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b23db-111">This simplifies your environment by ensuring that only one version of Azure PowerShell is installed.</span></span> <span data-ttu-id="b23db-112">No entanto, existem cenários onde poderá precisar de múltiplas versões instaladas ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="b23db-112">However, there are scenarios where you may need multiple versions installed at the same time.</span></span>
>
> <span data-ttu-id="b23db-113">Os módulos da Galeria do PowerShell instalam módulos em `$env:ProgramFiles\WindowsPowerShell\Modules`.</span><span class="sxs-lookup"><span data-stu-id="b23db-113">PowerShell Gallery modules install modules in `$env:ProgramFiles\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="b23db-114">Em contrapartida, o instalador WebPI instalará os módulos do Azure em `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`.</span><span class="sxs-lookup"><span data-stu-id="b23db-114">In contrast, the WebPI installer installs the Azure modules in `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`.</span></span>
>
> <span data-ttu-id="b23db-115">Se ocorrer um erro durante a instalação, pode remover manualmente as pastas Azure* na pasta `$env:ProgramFiles\WindowsPowerShell\Modules` e tentar efetuar novamente a instalação.</span><span class="sxs-lookup"><span data-stu-id="b23db-115">If an error occurs during install, you can manually remove the Azure* folders in your `$env:ProgramFiles\WindowsPowerShell\Modules` folder, and try the installation again.</span></span>

<span data-ttu-id="b23db-116">Depois de concluída a instalação, a definição `$env:PSModulePath` deve incluir os diretórios que contêm os cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b23db-116">Once the installation completes, your `$env:PSModulePath` setting should include the directories containing the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="b23db-117">Pode ser utilizado o comando seguinte para verificar se o Azure PowerShell está instalado corretamente.</span><span class="sxs-lookup"><span data-stu-id="b23db-117">The following command can be used to verify that the Azure PowerShell is installed properly.</span></span>

```powershell
# To make sure the Azure PowerShell module is available after you install
Get-Module -ListAvailable Azure* | Select-Object Name, Version, Path
```

> [!NOTE]
> <span data-ttu-id="b23db-118">Existe um problema conhecido que pode ocorrer ao instalar a partir do WebPI.</span><span class="sxs-lookup"><span data-stu-id="b23db-118">There is a known issue that can occur when installing from WebPI.</span></span> <span data-ttu-id="b23db-119">Se o seu computador tiver de ser reiniciado devido a atualizações do sistema ou outras instalações, isto poderá provocar a falha das atualizações em `$env:PSModulePath` para incluir o caminho onde o Azure PowerShell está instalado.</span><span class="sxs-lookup"><span data-stu-id="b23db-119">If your computer requires a restart due to system updates or other installations, it may cause updates to `$env:PSModulePath` to fail to include the path where Azure PowerShell is installed.</span></span>

<span data-ttu-id="b23db-120">Ao tentar carregar ou executar os cmdlets após a instalação, pode receber a seguinte mensagem de erro:</span><span class="sxs-lookup"><span data-stu-id="b23db-120">When attempting to load or execute cmdlets after installation, you can receive the following error message:</span></span>

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

<span data-ttu-id="b23db-121">Este erro pode ser corrigido ao reiniciar o computador ou ao importar o módulo através do caminho totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="b23db-121">This error can be corrected by restarting the machine or importing the module using the fully qualified path.</span></span> <span data-ttu-id="b23db-122">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="b23db-122">For example:</span></span>

```powershell
Import-Module "$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\AzureRM.psd1"
```

## <span data-ttu-id="b23db-123">Instalar através do Pacote MSI</span><span class="sxs-lookup"><span data-stu-id="b23db-123">Install using the MSI Package</span></span>
<a id="install-using-the-msi-package" class="xliff"></a>

<span data-ttu-id="b23db-124">O Azure PowerShell pode ser instalado através do ficheiro MSI disponível a partir do [GitHub](https://github.com/Azure/azure-powershell/releases/latest).</span><span class="sxs-lookup"><span data-stu-id="b23db-124">Azure PowerShell can be installed using the MSI file available from [GitHub](https://github.com/Azure/azure-powershell/releases/latest).</span></span> <span data-ttu-id="b23db-125">Se tiver versões anteriores dos módulos do Azure instaladas, o instalador remove-as automaticamente.</span><span class="sxs-lookup"><span data-stu-id="b23db-125">If you have installed previous versions of Azure modules, the installer automatically removes them.</span></span> <span data-ttu-id="b23db-126">O pacote MSI instala os módulos em `$env:ProgramFiles\WindowsPowerShell\Modules`, mas não cria pastas específicas da versão.</span><span class="sxs-lookup"><span data-stu-id="b23db-126">The MSI package installs modules in `$env:ProgramFiles\WindowsPowerShell\Modules` but does not create version-specific folders.</span></span>
