---
title: "Descrição geral do Azure PowerShell | Microsoft Docs"
description: "Descrição geral da instalação e da configuração do Azure PowerShell."
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.manager: carmonm
ms.date: 07/26/2017
ms.openlocfilehash: 02bfc15fec83ed4078d9a054b450c5a3cd66b8e2
ms.sourcegitcommit: db5c50de90764a9bdc7c1f1dbca3aed5bfeb05fa
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2017
---
# <a name="overview-of-azure-powershell"></a><span data-ttu-id="f2690-103">Descrição Geral do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="f2690-103">Overview of Azure PowerShell</span></span>

<span data-ttu-id="f2690-104">O Azure PowerShell fornece um conjunto de cmdlets que utilizam o modelo do [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) para gerir os recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="f2690-104">Azure PowerShell provides a set of cmdlets that use the [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) model for managing your Azure resources.</span></span>

<span data-ttu-id="f2690-105">Veja o [artigo Install](install-azurerm-ps.md) (Instalar) para configurar o Azure Powershell no seu sistema.</span><span class="sxs-lookup"><span data-stu-id="f2690-105">Review the [Install](install-azurerm-ps.md) article to get Azure PowerShell up and running on your system.</span></span> <span data-ttu-id="f2690-106">Depois, leia o artigo [Get Started](get-started-azureps.md) (Introdução) para começar a utilizá-la.</span><span class="sxs-lookup"><span data-stu-id="f2690-106">Then read the [Get Started](get-started-azureps.md) article to begin using it.</span></span> <span data-ttu-id="f2690-107">Para obter informações sobre a versão mais recente, veja as [notas de versão](release-notes-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="f2690-107">For information about the latest release, see the [release notes](release-notes-azureps.md).</span></span>

<span data-ttu-id="f2690-108">Os exemplos seguintes podem ajudá-lo a saber como utilizar o Azure PowerShell para realizar cenários comuns:</span><span class="sxs-lookup"><span data-stu-id="f2690-108">The following samples can help you learn how to perform common scenarios with Azure PowerShell:</span></span>

* [<span data-ttu-id="f2690-109">Máquinas Virtuais do Linux</span><span class="sxs-lookup"><span data-stu-id="f2690-109">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="f2690-110">Máquinas Virtuais do Windows</span><span class="sxs-lookup"><span data-stu-id="f2690-110">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="f2690-111">Aplicações Web</span><span class="sxs-lookup"><span data-stu-id="f2690-111">Web Apps</span></span>](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="f2690-112">Bases de Dados SQL</span><span class="sxs-lookup"><span data-stu-id="f2690-112">SQL Databases</span></span>](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

> [!NOTE]<span data-ttu-id="f2690-113"> > Se tiver implementações que utilizam o modelo de implementação clássico que não é possível converter, pode instalar a versão de Gestão de Serviço do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f2690-113"> > If you have deployments that use the classic deployment model that cannot be converted, you can install the Service Management version of Azure PowerShell.</span></span> <span data-ttu-id="f2690-114">Para obter mais informações, veja [Instalar o módulo Service Management do Azure PowerShell](/powershell/azure/servicemanagement/install-azure-ps).</span><span class="sxs-lookup"><span data-stu-id="f2690-114">For more information, see [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span>

### <a name="need-help-with-powershell"></a><span data-ttu-id="f2690-115">Necessita ajuda com o PowerShell?</span><span class="sxs-lookup"><span data-stu-id="f2690-115">Need help with PowerShell?</span></span>

<span data-ttu-id="f2690-116">Se não está familiarizado com o PowerShell, uma introdução ao PowerShell poderá útil.</span><span class="sxs-lookup"><span data-stu-id="f2690-116">If you are unfamiliar with PowerShell, you may find an introduction to PowerShell helpful.</span></span>

* [<span data-ttu-id="f2690-117">Instalar o PowerShell</span><span class="sxs-lookup"><span data-stu-id="f2690-117">Installing PowerShell</span></span>](/powershell/scripting/installing-windows-powershell)
* [<span data-ttu-id="f2690-118">Scripting com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="f2690-118">Scripting with PowerShell</span></span>](/powershell/scripting/scripting-with-windows-powershell)

<span data-ttu-id="f2690-119">Também pode ver este vídeo: [Noções básicas do PowerShell: (parte 1) Começar a Trabalhar com o PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span><span class="sxs-lookup"><span data-stu-id="f2690-119">You can also watch this video: [PowerShell Basics: (Part 1) Getting Started with PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span></span>

## <a name="other-azure-powershell-modules"></a><span data-ttu-id="f2690-120">Outros módulos do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="f2690-120">Other Azure PowerShell modules</span></span>

* [<span data-ttu-id="f2690-121">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="f2690-121">Azure Active Directory</span></span>](/powershell/azure/active-directory/)
* [<span data-ttu-id="f2690-122">Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="f2690-122">Azure Information Protection</span></span>](/powershell/azure/aip/)
* [<span data-ttu-id="f2690-123">Azure Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f2690-123">Azure Service Fabric</span></span>](/powershell/azure/service-fabric/)
* [<span data-ttu-id="f2690-124">Azure ElasticDB</span><span class="sxs-lookup"><span data-stu-id="f2690-124">Azure ElasticDB</span></span>](/powershell/azure/elasticdbjobs/)
