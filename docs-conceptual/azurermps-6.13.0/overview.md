---
title: Descrição geral do Azure PowerShell | Microsoft Docs
description: Descrição geral da instalação e da configuração do Azure PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/20/2018
ms.openlocfilehash: 91607252c33deb05efebb2d02608084a4b9c7b35
ms.sourcegitcommit: 7839b82f47ef8dd522eff900081c22de0d089cfc
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/14/2020
ms.locfileid: "83385563"
---
# <a name="overview-of-azure-powershell"></a><span data-ttu-id="c4c9c-103">Descrição Geral do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c4c9c-103">Overview of Azure PowerShell</span></span>

[!INCLUDE[az-replacing-azurerm](../includes/az-replacing-azurerm.md)]

<span data-ttu-id="c4c9c-104">O Azure PowerShell fornece um conjunto de cmdlets que utilizam o modelo do [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) para gerir os recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="c4c9c-104">Azure PowerShell provides a set of cmdlets that use the [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) model for managing your Azure resources.</span></span> <span data-ttu-id="c4c9c-105">Pode utilizá-lo no seu browser com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou pode instalá-lo no seu computador local e utilizá-lo em qualquer sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c4c9c-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can install it on your local machine and use it in any PowerShell session.</span></span>

<span data-ttu-id="c4c9c-106">Utilize o [Cloud Shell](/azure/cloud-shell/overview) para executar o Azure PowerShell no seu browser ou [instale-o](install-azurerm-ps.md) no seu computador.</span><span class="sxs-lookup"><span data-stu-id="c4c9c-106">Use the [Cloud Shell](/azure/cloud-shell/overview) to run the Azure PowerShell in your browser, or [install](install-azurerm-ps.md) it on own computer.</span></span> <span data-ttu-id="c4c9c-107">Depois, leia o artigo [Get Started](get-started-azureps.md) (Introdução) para começar a utilizá-la.</span><span class="sxs-lookup"><span data-stu-id="c4c9c-107">Then read the [Get Started](get-started-azureps.md) article to begin using it.</span></span> <span data-ttu-id="c4c9c-108">Para obter informações sobre a versão mais recente, veja as [notas de versão](release-notes-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="c4c9c-108">For information about the latest release, see the [release notes](release-notes-azureps.md).</span></span>

<span data-ttu-id="c4c9c-109">Os exemplos seguintes podem ajudá-lo a saber como utilizar o Azure PowerShell para realizar cenários comuns:</span><span class="sxs-lookup"><span data-stu-id="c4c9c-109">The following samples can help you learn how to perform common scenarios with Azure PowerShell:</span></span>

* [<span data-ttu-id="c4c9c-110">Máquinas Virtuais do Linux</span><span class="sxs-lookup"><span data-stu-id="c4c9c-110">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="c4c9c-111">Máquinas Virtuais do Windows</span><span class="sxs-lookup"><span data-stu-id="c4c9c-111">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="c4c9c-112">Aplicações Web</span><span class="sxs-lookup"><span data-stu-id="c4c9c-112">Web Apps</span></span>](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="c4c9c-113">Bases de Dados SQL</span><span class="sxs-lookup"><span data-stu-id="c4c9c-113">SQL Databases</span></span>](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

## <a name="learn-powershell-basics"></a><span data-ttu-id="c4c9c-114">Aprenda as noções básicas do PowerShell</span><span class="sxs-lookup"><span data-stu-id="c4c9c-114">Learn PowerShell basics</span></span>

<span data-ttu-id="c4c9c-115">Se não está familiarizado com o PowerShell, uma introdução ao PowerShell pode ser útil.</span><span class="sxs-lookup"><span data-stu-id="c4c9c-115">If you're unfamiliar with PowerShell, an introduction to PowerShell may be helpful.</span></span>

* [<span data-ttu-id="c4c9c-116">Instalar o PowerShell</span><span class="sxs-lookup"><span data-stu-id="c4c9c-116">Installing PowerShell</span></span>](/powershell/scripting/install/installing-windows-powershell)
* [<span data-ttu-id="c4c9c-117">Scripting com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="c4c9c-117">Scripting with PowerShell</span></span>](/powershell/scripting/powershell-scripting)

<span data-ttu-id="c4c9c-118">Também pode ver este vídeo: [Noções básicas do PowerShell: (Parte 1) Introdução ao PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span><span class="sxs-lookup"><span data-stu-id="c4c9c-118">You can also watch this video: [PowerShell Basics: (Part 1) Getting Started with PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span></span>

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="c4c9c-119">Desenvolva as suas competências com o Microsoft Learn</span><span class="sxs-lookup"><span data-stu-id="c4c9c-119">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="c4c9c-120">Utilizar scripts para automatizar as tarefas do Azure com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="c4c9c-120">Automate Azure tasks using scripts with PowerShell</span></span>](/learn/modules/automate-azure-tasks-with-powershell/)
- [<span data-ttu-id="c4c9c-121">Mais aprendizagem interativa...</span><span class="sxs-lookup"><span data-stu-id="c4c9c-121">More interactive learning...</span></span>](/learn/browse/?term=powershell)

## <a name="other-azure-powershell-modules"></a><span data-ttu-id="c4c9c-122">Outros módulos do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c4c9c-122">Other Azure PowerShell modules</span></span>

* [<span data-ttu-id="c4c9c-123">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="c4c9c-123">Azure Active Directory</span></span>](/powershell/azure/active-directory/)
* [<span data-ttu-id="c4c9c-124">Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="c4c9c-124">Azure Information Protection</span></span>](/powershell/azure/aip/)
* [<span data-ttu-id="c4c9c-125">Azure Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c4c9c-125">Azure Service Fabric</span></span>](/powershell/azure/service-fabric/)
* [<span data-ttu-id="c4c9c-126">Azure ElasticDB</span><span class="sxs-lookup"><span data-stu-id="c4c9c-126">Azure ElasticDB</span></span>](/powershell/azure/elasticdbjobs/)
