---
title: Descrição geral do Azure PowerShell | Microsoft Docs
description: Descrição geral da instalação e da configuração do Azure PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 08/31/2017
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: 7d220266bd6e36fd083f56290cb6cee8f2e80d3e
ms.sourcegitcommit: 8b3126b5c79f453464d90669f0046ba86b7a3424
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/01/2020
ms.locfileid: "89243706"
---
# <a name="overview-of-azure-powershell"></a><span data-ttu-id="366c8-103">Descrição Geral do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="366c8-103">Overview of Azure PowerShell</span></span>

[!INCLUDE [migrate-to-az-banner](../../includes/migrate-to-az-banner.md)]

<span data-ttu-id="366c8-104">O Azure PowerShell fornece um conjunto de cmdlets que utilizam o modelo do [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) para gerir os recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="366c8-104">Azure PowerShell provides a set of cmdlets that use the [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) model for managing your Azure resources.</span></span> <span data-ttu-id="366c8-105">Pode utilizá-lo no seu browser com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou pode instalá-lo no seu computador local e utilizá-lo em qualquer sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="366c8-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can install it on your local machine and use it in any PowerShell session.</span></span>

<span data-ttu-id="366c8-106">Utilize o [Cloud Shell](/azure/cloud-shell/overview) para executar o Azure PowerShell no seu browser ou [instale-o](install-azurerm-ps.md) no seu computador.</span><span class="sxs-lookup"><span data-stu-id="366c8-106">Use the [Cloud Shell](/azure/cloud-shell/overview) to run the Azure PowerShell in your browser, or [install](install-azurerm-ps.md) it on own computer.</span></span> <span data-ttu-id="366c8-107">Depois, leia o artigo [Get Started](get-started-azureps.md) (Introdução) para começar a utilizá-la.</span><span class="sxs-lookup"><span data-stu-id="366c8-107">Then read the [Get Started](get-started-azureps.md) article to begin using it.</span></span> <span data-ttu-id="366c8-108">Para obter informações sobre a versão mais recente, veja as [notas de versão](release-notes-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="366c8-108">For information about the latest release, see the [release notes](release-notes-azureps.md).</span></span>

<span data-ttu-id="366c8-109">Os exemplos seguintes podem ajudá-lo a saber como utilizar o Azure PowerShell para realizar cenários comuns:</span><span class="sxs-lookup"><span data-stu-id="366c8-109">The following samples can help you learn how to perform common scenarios with Azure PowerShell:</span></span>

- [<span data-ttu-id="366c8-110">Máquinas Virtuais do Linux</span><span class="sxs-lookup"><span data-stu-id="366c8-110">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
- [<span data-ttu-id="366c8-111">Máquinas Virtuais do Windows</span><span class="sxs-lookup"><span data-stu-id="366c8-111">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
- [<span data-ttu-id="366c8-112">Aplicações Web</span><span class="sxs-lookup"><span data-stu-id="366c8-112">Web Apps</span></span>](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
- [<span data-ttu-id="366c8-113">Bases de Dados SQL</span><span class="sxs-lookup"><span data-stu-id="366c8-113">SQL Databases</span></span>](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

## <a name="learn-powershell-basics"></a><span data-ttu-id="366c8-114">Aprenda as noções básicas do PowerShell</span><span class="sxs-lookup"><span data-stu-id="366c8-114">Learn PowerShell basics</span></span>

<span data-ttu-id="366c8-115">Se não está familiarizado com o PowerShell, uma introdução ao PowerShell poderá útil.</span><span class="sxs-lookup"><span data-stu-id="366c8-115">If you are unfamiliar with PowerShell, you may find an introduction to PowerShell helpful.</span></span>

- [<span data-ttu-id="366c8-116">Instalar o PowerShell</span><span class="sxs-lookup"><span data-stu-id="366c8-116">Installing PowerShell</span></span>](/powershell/scripting/install/installing-powershell)
- [<span data-ttu-id="366c8-117">Recursos de aprendizagem do PowerShell</span><span class="sxs-lookup"><span data-stu-id="366c8-117">PowerShell learning resources</span></span>](/powershell/scripting/learn/more-powershell-learning)

<span data-ttu-id="366c8-118">Também pode ver este vídeo: [Noções básicas do PowerShell: (Parte 1) Introdução ao PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span><span class="sxs-lookup"><span data-stu-id="366c8-118">You can also watch this video: [PowerShell Basics: (Part 1) Getting Started with PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span></span>

## <a name="other-azure-powershell-modules"></a><span data-ttu-id="366c8-119">Outros módulos do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="366c8-119">Other Azure PowerShell modules</span></span>

- [<span data-ttu-id="366c8-120">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="366c8-120">Azure Active Directory</span></span>](/powershell/azure/active-directory/)
- [<span data-ttu-id="366c8-121">Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="366c8-121">Azure Information Protection</span></span>](/powershell/azure/aip/)
- [<span data-ttu-id="366c8-122">Azure Service Fabric</span><span class="sxs-lookup"><span data-stu-id="366c8-122">Azure Service Fabric</span></span>](/powershell/azure/service-fabric/)
- [<span data-ttu-id="366c8-123">Azure ElasticDB</span><span class="sxs-lookup"><span data-stu-id="366c8-123">Azure ElasticDB</span></span>](/powershell/azure/elasticdbjobs/)
