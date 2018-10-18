---
title: Outras formas de instalar o Azure PowerShell
description: Como instalar o Azure PowerShell sem o PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/20/2018
ms.openlocfilehash: 2fcd2307667d1f810fbcb3fe4d14e3b0def537ed
ms.sourcegitcommit: f6f5e256143aa6c097de3e57e930d8badea49f30
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2018
ms.locfileid: "49399302"
---
# <a name="install-azure-powershell-on-windows-with-msi-or-web-platform-installer"></a><span data-ttu-id="7af89-103">Instalar o Azure PowerShell no Windows com o MSI ou o Instalador de Plataforma Web</span><span class="sxs-lookup"><span data-stu-id="7af89-103">Install Azure PowerShell on Windows with MSI or Web Platform Installer</span></span>

<span data-ttu-id="7af89-104">Este artigo explica como instalar o Azure PowerShell no Windows com um pacote MSI ou o Instalador de Plataforma Web (WebPI).</span><span class="sxs-lookup"><span data-stu-id="7af89-104">This article explains how to install Azure PowerShell on Windows using an MSI or Web Platform Installer (WebPI).</span></span>  
<span data-ttu-id="7af89-105">Utilize estes métodos de instalação apenas se forem necessários para o seu sistema.</span><span class="sxs-lookup"><span data-stu-id="7af89-105">Use these installation methods only if they're necessary for your system.</span></span> <span data-ttu-id="7af89-106">A forma recomendada para instalar o Azure PowerShell no Windows é com o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="7af89-106">The recommended way to install Azure PowerShell on Windows is with PowerShellGet.</span></span> <span data-ttu-id="7af89-107">Para obter instruções sobre como utilizar o PowerShellGet para instalar o Azure PowerShell, veja [Instalar o Azure PowerShell com o PowerShellGet](install-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="7af89-107">For instructions on using PowerShellGet to install Azure PowerShell, see [Install Azure PowerShell with PowerShellGet](install-azurerm-ps.md).</span></span>

<span data-ttu-id="7af89-108">Para instalar em ambientes Linux ou macOS, veja [Instalar o Azure PowerShell no macOS ou Linux](install-azurermps-maclinux.md).</span><span class="sxs-lookup"><span data-stu-id="7af89-108">To install on Linux or macOS environments, see [Install Azure PowerShell on macOS or Linux](install-azurermps-maclinux.md).</span></span>

## <a name="install-or-update-on-windows-using-the-msi-package"></a><span data-ttu-id="7af89-109">Instalar ou atualizar no Windows com o Pacote MSI</span><span class="sxs-lookup"><span data-stu-id="7af89-109">Install or update on Windows using the MSI Package</span></span>

<span data-ttu-id="7af89-110">O Azure PowerShell pode ser instalado através do ficheiro MSI disponível a partir do [GitHub](https://github.com/Azure/azure-powershell/releases/tag/v5.7.0-April2018).</span><span class="sxs-lookup"><span data-stu-id="7af89-110">Azure PowerShell can be installed using the MSI file available from [GitHub](https://github.com/Azure/azure-powershell/releases/tag/v5.7.0-April2018).</span></span> <span data-ttu-id="7af89-111">Se tiver instalado as versões anteriores dos módulos do Azure como um MSI, o instalador remove-as automaticamente.</span><span class="sxs-lookup"><span data-stu-id="7af89-111">If you have installed previous versions of Azure modules as an MSI, the installer automatically removes them.</span></span> <span data-ttu-id="7af89-112">O pacote do MSI instala os módulos em `${env:ProgramFiles}\WindowsPowerShell\Modules`.</span><span class="sxs-lookup"><span data-stu-id="7af89-112">The MSI package installs modules in `${env:ProgramFiles}\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="7af89-113">Ambos os módulos `AzureRM` e `Azure` são instalados.</span><span class="sxs-lookup"><span data-stu-id="7af89-113">Both the `AzureRM` and `Azure` modules are installed.</span></span>

> [!NOTE]
> <span data-ttu-id="7af89-114">Utilize o módulo `Azure` apenas se estiver a trabalhar com o modelo de implementação clássica do Azure.</span><span class="sxs-lookup"><span data-stu-id="7af89-114">Only use the `Azure` module if you are working with the Azure classic deployment model.</span></span>

<span data-ttu-id="7af89-115">Para começar a utilizar o Azure PowerShell, precisa de carregar `AzureRM` para a sua sessão atual do PowerShell com o cmdlet [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) e, em seguida, iniciar sessão com as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="7af89-115">To start working with Azure PowerShell, you need to load `AzureRM` into your current PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span>

```powershell
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="7af89-116">Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada.</span><span class="sxs-lookup"><span data-stu-id="7af89-116">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="7af89-117">A importação automática do módulo `AzureRM` implica configurar um perfil do PowerShell, um processo sobre o qual pode obter mais informações em [Acerca de Perfis](/powershell/module/microsoft.powershell.core/about/about_profiles).</span><span class="sxs-lookup"><span data-stu-id="7af89-117">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="7af89-118">Para saber como manter o início de sessão do Azure entre as sessões, veja [Manter credenciais do utilizador nas sessões do PowerShell](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="7af89-118">To learn how to persist your Azure sign in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="install-or-update-on-windows-using-the-web-platform-installer"></a><span data-ttu-id="7af89-119">Instalar ou atualizar no Windows com o Instalador de Plataforma Web</span><span class="sxs-lookup"><span data-stu-id="7af89-119">Install or update on Windows using the Web Platform Installer</span></span>

<span data-ttu-id="7af89-120">Transfira o [pacote WebPI do Azure PowerShell](http://aka.ms/webpi-azps) e inicie a instalação.</span><span class="sxs-lookup"><span data-stu-id="7af89-120">Download the [Azure PowerShell WebPI package](http://aka.ms/webpi-azps) and start the install.</span></span> <span data-ttu-id="7af89-121">Se tiver versões anteriores dos módulos do Azure instaladas a partir de um MSI ou com o WebPI, o instalador remove-as automaticamente.</span><span class="sxs-lookup"><span data-stu-id="7af89-121">If you have installed previous versions of Azure modules from an MSI or with WebPI, the installer automatically removes them.</span></span> <span data-ttu-id="7af89-122">Os módulos são instalados no `${env:ProgramFiles}\WindowsPowerShell\Modules`.</span><span class="sxs-lookup"><span data-stu-id="7af89-122">Modules are installed into `${env:ProgramFiles}\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="7af89-123">Os módulos `AzureRM` e `Azure` estão instalados.</span><span class="sxs-lookup"><span data-stu-id="7af89-123">Both the `AzureRM` and `Azure` modules are installed.</span></span>

> [!NOTE]
> <span data-ttu-id="7af89-124">Utilize o módulo `Azure` apenas se estiver a trabalhar com o modelo de implementação clássica do Azure.</span><span class="sxs-lookup"><span data-stu-id="7af89-124">Only use the `Azure` module if you are working with the Azure classic deployment model.</span></span>

<span data-ttu-id="7af89-125">Para começar a utilizar o Azure PowerShell, precisa de carregar `AzureRM` para a sua sessão atual do PowerShell com o cmdlet [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) e, em seguida, iniciar sessão com as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="7af89-125">To start working with Azure PowerShell, you need to load `AzureRM` into your current PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span>

```powershell
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="7af89-126">Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada.</span><span class="sxs-lookup"><span data-stu-id="7af89-126">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="7af89-127">A importação automática do módulo `AzureRM` implica configurar um perfil do PowerShell, um processo sobre o qual pode obter mais informações em [Acerca de Perfis](/powershell/module/microsoft.powershell.core/about/about_profiles).</span><span class="sxs-lookup"><span data-stu-id="7af89-127">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="7af89-128">Para saber como manter o início de sessão do Azure entre as sessões, veja [Manter credenciais do utilizador nas sessões do PowerShell](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="7af89-128">To learn how to persist your Azure sign in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>
