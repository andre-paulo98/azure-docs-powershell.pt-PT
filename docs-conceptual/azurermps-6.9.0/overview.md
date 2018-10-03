---
title: Descrição geral do Azure PowerShell | Microsoft Docs
description: Descrição geral da instalação e da configuração do Azure PowerShell.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.manager: carmonm
ms.date: 09/11/2018
ms.openlocfilehash: f03243f6f560407b63aff154494cf164d670d810
ms.sourcegitcommit: 19dffee617477001f98d43e39a50ce1fad087b74
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2018
ms.locfileid: "47178668"
---
# <a name="overview-of-azure-powershell"></a><span data-ttu-id="7aa8f-103">Descrição Geral do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="7aa8f-103">Overview of Azure PowerShell</span></span>

<span data-ttu-id="7aa8f-104">O Azure PowerShell fornece um conjunto de cmdlets que utilizam o modelo do [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) para gerir os recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="7aa8f-104">Azure PowerShell provides a set of cmdlets that use the [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) model for managing your Azure resources.</span></span> <span data-ttu-id="7aa8f-105">Pode utilizá-lo no seu browser com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou pode instalá-lo no seu computador local e utilizá-lo em qualquer sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7aa8f-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can install it on your local machine and use it in any PowerShell session.</span></span>

<span data-ttu-id="7aa8f-106">Utilize o [Cloud Shell](/azure/cloud-shell/overview) para executar o Azure PowerShell no seu browser ou [instale-o](install-azurerm-ps.md) no seu computador.</span><span class="sxs-lookup"><span data-stu-id="7aa8f-106">Use the [Cloud Shell](/azure/cloud-shell/overview) to run the Azure PowerShell in your browser, or [install](install-azurerm-ps.md) it on own computer.</span></span> <span data-ttu-id="7aa8f-107">Depois, leia o artigo [Get Started](get-started-azureps.md) (Introdução) para começar a utilizá-la.</span><span class="sxs-lookup"><span data-stu-id="7aa8f-107">Then read the [Get Started](get-started-azureps.md) article to begin using it.</span></span> <span data-ttu-id="7aa8f-108">Para obter informações sobre a versão mais recente, veja as [notas de versão](release-notes-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="7aa8f-108">For information about the latest release, see the [release notes](release-notes-azureps.md).</span></span>

<span data-ttu-id="7aa8f-109">Os exemplos seguintes podem ajudá-lo a saber como utilizar o Azure PowerShell para realizar cenários comuns:</span><span class="sxs-lookup"><span data-stu-id="7aa8f-109">The following samples can help you learn how to perform common scenarios with Azure PowerShell:</span></span>

* [<span data-ttu-id="7aa8f-110">Máquinas Virtuais do Linux</span><span class="sxs-lookup"><span data-stu-id="7aa8f-110">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="7aa8f-111">Máquinas Virtuais do Windows</span><span class="sxs-lookup"><span data-stu-id="7aa8f-111">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="7aa8f-112">Aplicações Web</span><span class="sxs-lookup"><span data-stu-id="7aa8f-112">Web Apps</span></span>](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="7aa8f-113">Bases de Dados SQL</span><span class="sxs-lookup"><span data-stu-id="7aa8f-113">SQL Databases</span></span>](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

> [!NOTE]
> <span data-ttu-id="7aa8f-114">Se tiver implementações que utilizam o modelo de implementação clássico que não é possível converter, pode instalar a versão de Gestão de Serviço do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7aa8f-114">If you have deployments that use the classic deployment model that cannot be converted, you can install the Service Management version of Azure PowerShell.</span></span> <span data-ttu-id="7aa8f-115">Para obter mais informações, veja [Instalar o módulo Service Management do Azure PowerShell](/powershell/azure/servicemanagement/install-azure-ps).</span><span class="sxs-lookup"><span data-stu-id="7aa8f-115">For more information, see [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span>

## <a name="learn-powershell-basics"></a><span data-ttu-id="7aa8f-116">Aprenda as noções básicas do PowerShell</span><span class="sxs-lookup"><span data-stu-id="7aa8f-116">Learn PowerShell basics</span></span>

<span data-ttu-id="7aa8f-117">Se não está familiarizado com o PowerShell, uma introdução ao PowerShell pode ser útil.</span><span class="sxs-lookup"><span data-stu-id="7aa8f-117">If you're unfamiliar with PowerShell, an introduction to PowerShell may be helpful.</span></span>

* [<span data-ttu-id="7aa8f-118">Instalar o PowerShell</span><span class="sxs-lookup"><span data-stu-id="7aa8f-118">Installing PowerShell</span></span>](/powershell/scripting/setup/installing-windows-powershell)
* [<span data-ttu-id="7aa8f-119">Scripting com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="7aa8f-119">Scripting with PowerShell</span></span>](/powershell/scripting/powershell-scripting)

<span data-ttu-id="7aa8f-120">Também pode ver este vídeo: [Noções básicas do PowerShell: (parte 1) Começar a Trabalhar com o PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span><span class="sxs-lookup"><span data-stu-id="7aa8f-120">You can also watch this video: [PowerShell Basics: (Part 1) Getting Started with PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span></span>

<span data-ttu-id="7aa8f-121">Ou assista à [Introdução ao Arranque do PowerShell](https://mva.microsoft.com/liveevents/powershell-jumpstart) da Microsoft Virtual Academy.</span><span class="sxs-lookup"><span data-stu-id="7aa8f-121">Or attend the Microsoft Virtual Academy's [Getting Started with PowerShell Jumpstart](https://mva.microsoft.com/liveevents/powershell-jumpstart).</span></span>

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="7aa8f-122">Desenvolva as suas competências com o Microsoft Learn</span><span class="sxs-lookup"><span data-stu-id="7aa8f-122">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="7aa8f-123">Utilizar scripts para automatizar as tarefas do Azure com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="7aa8f-123">Automate Azure tasks using scripts with PowerShell</span></span>](/learn/modules/automate-azure-tasks-with-powershell/)
- [<span data-ttu-id="7aa8f-124">Mais aprendizagem interativa...</span><span class="sxs-lookup"><span data-stu-id="7aa8f-124">More interactive learning...</span></span>](/learn/browse/?term=powershell)

## <a name="other-azure-powershell-modules"></a><span data-ttu-id="7aa8f-125">Outros módulos do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="7aa8f-125">Other Azure PowerShell modules</span></span>

* [<span data-ttu-id="7aa8f-126">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="7aa8f-126">Azure Active Directory</span></span>](/powershell/azure/active-directory/)
* [<span data-ttu-id="7aa8f-127">Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="7aa8f-127">Azure Information Protection</span></span>](/powershell/azure/aip/)
* [<span data-ttu-id="7aa8f-128">Azure Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7aa8f-128">Azure Service Fabric</span></span>](/powershell/azure/service-fabric/)
* [<span data-ttu-id="7aa8f-129">Azure ElasticDB</span><span class="sxs-lookup"><span data-stu-id="7aa8f-129">Azure ElasticDB</span></span>](/powershell/azure/elasticdbjobs/)