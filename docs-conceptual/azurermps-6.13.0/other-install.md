---
title: Outras formas de instalar o Azure PowerShell
description: Como instalar o Azure PowerShell sem o PowerShellGet utilizar um MSI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/16/2018
ms.openlocfilehash: 8fdf5598050cea2ef3f7422d53b22f9e49fe7477
ms.sourcegitcommit: b37b8bb6f8e39ecea5b50ceec48601eed313add7
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/09/2019
ms.locfileid: "65511674"
---
# <a name="install-azure-powershell-on-windows-with-msi"></a><span data-ttu-id="3850e-103">Instalar o Azure PowerShell no Windows com o MSI</span><span class="sxs-lookup"><span data-stu-id="3850e-103">Install Azure PowerShell on Windows with MSI</span></span>

<span data-ttu-id="3850e-104">Este artigo explica como instalar o Azure PowerShell no Windows com um Instalador do MSI.</span><span class="sxs-lookup"><span data-stu-id="3850e-104">This article explains how to install Azure PowerShell on Windows using an MSI installer.</span></span>  
<span data-ttu-id="3850e-105">Utilize estes métodos de instalação apenas se forem necessários para o seu sistema.</span><span class="sxs-lookup"><span data-stu-id="3850e-105">Use these installation methods only if they're necessary for your system.</span></span> <span data-ttu-id="3850e-106">A forma recomendada para instalar o Azure PowerShell no Windows é com o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="3850e-106">The recommended way to install Azure PowerShell on Windows is with PowerShellGet.</span></span> <span data-ttu-id="3850e-107">Para obter instruções sobre como utilizar o PowerShellGet para instalar o Azure PowerShell, veja [Instalar o Azure PowerShell com o PowerShellGet](install-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="3850e-107">For instructions on using PowerShellGet to install Azure PowerShell, see [Install Azure PowerShell with PowerShellGet](install-azurerm-ps.md).</span></span>

> [!NOTE]
> <span data-ttu-id="3850e-108">O método de instalação do Instalador de Plataforma Web já não está disponível para as versões 6.x e superiores do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3850e-108">The Web Platform Installer method of installation is no longer available for versions of Azure PowerShell 6.x and higher.</span></span> <span data-ttu-id="3850e-109">Se precisar de utilizar o Instalador de Plataforma Web, considere utilizar o MSI em alternativa ou instale uma versão anterior do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3850e-109">If you require use of the Web Platform Installer please consider using the MSI instead, or you can install an earlier version of Azure PowerShell.</span></span>

## <a name="install-or-update-on-windows-using-the-msi-package"></a><span data-ttu-id="3850e-110">Instalar ou atualizar no Windows com o Pacote MSI</span><span class="sxs-lookup"><span data-stu-id="3850e-110">Install or update on Windows using the MSI Package</span></span>

<span data-ttu-id="3850e-111">O Azure PowerShell para o Windows PowerShell 5.x pode ser instalado através do ficheiro MSI disponível a partir do [GitHub](https://github.com/Azure/azure-powershell/releases/tag/v6.13.1-November2018).</span><span class="sxs-lookup"><span data-stu-id="3850e-111">Azure PowerShell for Windows PowerShell 5.x can be installed using the MSI file available from [GitHub](https://github.com/Azure/azure-powershell/releases/tag/v6.13.1-November2018).</span></span> <span data-ttu-id="3850e-112">Se tiver instalado as versões anteriores dos módulos do Azure como um MSI, o instalador remove-as automaticamente.</span><span class="sxs-lookup"><span data-stu-id="3850e-112">If you have installed previous versions of Azure modules as an MSI, the installer automatically removes them.</span></span> <span data-ttu-id="3850e-113">O pacote do MSI instala os módulos em `${env:ProgramFiles}\WindowsPowerShell\Modules`.</span><span class="sxs-lookup"><span data-stu-id="3850e-113">The MSI package installs modules in `${env:ProgramFiles}\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="3850e-114">Ambos os módulos `AzureRM` e `Azure` são instalados.</span><span class="sxs-lookup"><span data-stu-id="3850e-114">Both the `AzureRM` and `Azure` modules are installed.</span></span>

> [!NOTE]
> <span data-ttu-id="3850e-115">Utilize o módulo `Azure` apenas se estiver a trabalhar com o modelo de implementação clássica do Azure.</span><span class="sxs-lookup"><span data-stu-id="3850e-115">Only use the `Azure` module if you are working with the Azure classic deployment model.</span></span>

<span data-ttu-id="3850e-116">Para começar a trabalhar com o Azure PowerShell, inicie sessão com as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="3850e-116">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

> [!NOTE]
>
> <span data-ttu-id="3850e-117">Se tiver desativado o carregamento automático do módulo, tem de importar o módulo manualmente com `Import-Module AzureRM`.</span><span class="sxs-lookup"><span data-stu-id="3850e-117">If you've disabled module autoloading, you need to manually import the module with `Import-Module AzureRM`.</span></span> <span data-ttu-id="3850e-118">Devido à forma como o módulo está estruturado, esta operação pode demorar alguns segundos.</span><span class="sxs-lookup"><span data-stu-id="3850e-118">Because of the way the module is structured, this can take a few seconds.</span></span>

<span data-ttu-id="3850e-119">Terá de repetir este passo para cada nova sessão do PowerShell que iniciar.</span><span class="sxs-lookup"><span data-stu-id="3850e-119">You'll need to repeat this step for every new PowerShell session you start.</span></span> <span data-ttu-id="3850e-120">Para saber como manter o início de sessão do Azure nas sessões do PowerShell, veja [Manter as credenciais do utilizador nas sessões do PowerShell](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="3850e-120">To learn how to persist your Azure sign-in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>
