---
title: Outras formas de instalar o Azure PowerShell
description: Como instalar o Azure PowerShell sem o PowerShellGet utilizar um MSI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/11/2018
ms.openlocfilehash: 9fa5790e0a2aca4f933b40256634f772c258b189
ms.sourcegitcommit: ac4b53bb42a25aae013a9d8cd9ae98ada9397274
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/08/2018
ms.locfileid: "51274471"
---
# <a name="install-azure-powershell-on-windows-with-msi"></a><span data-ttu-id="05575-103">Instalar o Azure PowerShell no Windows com o MSI</span><span class="sxs-lookup"><span data-stu-id="05575-103">Install Azure PowerShell on Windows with MSI</span></span>

<span data-ttu-id="05575-104">Este artigo explica como instalar o Azure PowerShell no Windows com um Instalador do MSI.</span><span class="sxs-lookup"><span data-stu-id="05575-104">This article explains how to install Azure PowerShell on Windows using an MSI installer.</span></span>  
<span data-ttu-id="05575-105">Utilize estes métodos de instalação apenas se forem necessários para o seu sistema.</span><span class="sxs-lookup"><span data-stu-id="05575-105">Use these installation methods only if they're necessary for your system.</span></span> <span data-ttu-id="05575-106">A forma recomendada para instalar o Azure PowerShell no Windows é com o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="05575-106">The recommended way to install Azure PowerShell on Windows is with PowerShellGet.</span></span> <span data-ttu-id="05575-107">Para obter instruções sobre como utilizar o PowerShellGet para instalar o Azure PowerShell, veja [Instalar o Azure PowerShell com o PowerShellGet](install-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="05575-107">For instructions on using PowerShellGet to install Azure PowerShell, see [Install Azure PowerShell with PowerShellGet](install-azurerm-ps.md).</span></span>

> [!NOTE]
> <span data-ttu-id="05575-108">O método de instalação do Instalador de Plataforma Web já não está disponível para as versões 6.x e superiores do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="05575-108">The Web Platform Installer method of installation is no longer available for versions of Azure PowerShell 6.x and higher.</span></span> <span data-ttu-id="05575-109">Se precisar de utilizar o Instalador de Plataforma Web, considere utilizar o MSI em alternativa ou instale uma versão anterior do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="05575-109">If you require use of the Web Platform Installer please consider using the MSI instead, or you can install an earlier version of Azure PowerShell.</span></span>

<span data-ttu-id="05575-110">Para instalar em ambientes Linux ou macOS, veja [Instalar o Azure PowerShell no macOS ou Linux](install-azurermps-maclinux.md).</span><span class="sxs-lookup"><span data-stu-id="05575-110">To install on Linux or macOS environments, see [Install Azure PowerShell on macOS or Linux](install-azurermps-maclinux.md).</span></span>

## <a name="install-or-update-on-windows-using-the-msi-package"></a><span data-ttu-id="05575-111">Instalar ou atualizar no Windows com o Pacote MSI</span><span class="sxs-lookup"><span data-stu-id="05575-111">Install or update on Windows using the MSI Package</span></span>

<span data-ttu-id="05575-112">O Azure PowerShell pode ser instalado através do ficheiro MSI disponível a partir do [GitHub](https://github.com/Azure/azure-powershell/releases/latest).</span><span class="sxs-lookup"><span data-stu-id="05575-112">Azure PowerShell can be installed using the MSI file available from [GitHub](https://github.com/Azure/azure-powershell/releases/latest).</span></span> <span data-ttu-id="05575-113">Se tiver instalado as versões anteriores dos módulos do Azure como um MSI, o instalador remove-as automaticamente.</span><span class="sxs-lookup"><span data-stu-id="05575-113">If you have installed previous versions of Azure modules as an MSI, the installer automatically removes them.</span></span> <span data-ttu-id="05575-114">O pacote do MSI instala os módulos em `${env:ProgramFiles}\WindowsPowerShell\Modules`.</span><span class="sxs-lookup"><span data-stu-id="05575-114">The MSI package installs modules in `${env:ProgramFiles}\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="05575-115">Ambos os módulos `AzureRM` e `Azure` são instalados.</span><span class="sxs-lookup"><span data-stu-id="05575-115">Both the `AzureRM` and `Azure` modules are installed.</span></span>

> [!NOTE]
> <span data-ttu-id="05575-116">Utilize o módulo `Azure` apenas se estiver a trabalhar com o modelo de implementação clássica do Azure.</span><span class="sxs-lookup"><span data-stu-id="05575-116">Only use the `Azure` module if you are working with the Azure classic deployment model.</span></span>

<span data-ttu-id="05575-117">Para começar a utilizar o Azure PowerShell, precisa de carregar `AzureRM` para a sua sessão atual do PowerShell com o cmdlet [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) e, em seguida, iniciar sessão com as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="05575-117">To start working with Azure PowerShell, you need to load `AzureRM` into your current PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span>

```powershell-interactive
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="05575-118">Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada.</span><span class="sxs-lookup"><span data-stu-id="05575-118">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="05575-119">A importação automática do módulo `AzureRM` implica configurar um perfil do PowerShell, um processo sobre o qual pode obter mais informações em [Acerca de Perfis](/powershell/module/microsoft.powershell.core/about/about_profiles).</span><span class="sxs-lookup"><span data-stu-id="05575-119">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="05575-120">Para saber como manter o início de sessão do Azure entre as sessões, veja [Manter credenciais do utilizador nas sessões do PowerShell](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="05575-120">To learn how to persist your Azure sign-in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>