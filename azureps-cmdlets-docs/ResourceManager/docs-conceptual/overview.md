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
ms.date: 05/15/2017
ms.openlocfilehash: f26b204604018449584c1fd2ff199728487b1515
ms.sourcegitcommit: 226527be7cb647acfe2ea9ab151185053ab3c6db
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/29/2017
---
# <span data-ttu-id="a623c-103">Descrição Geral do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="a623c-103">Overview of Azure PowerShell</span></span>
<a id="overview-of-azure-powershell" class="xliff"></a>

<span data-ttu-id="a623c-104">O Azure PowerShell fornece um conjunto de cmdlets que utilizam o modelo do [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) para gerir os recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="a623c-104">Azure PowerShell provides a set of cmdlets that use the [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) model for managing your Azure resources.</span></span>

<span data-ttu-id="a623c-105">Veja o [artigo Install](install-azurerm-ps.md) (Instalar) para configurar o Azure Powershell no seu sistema.</span><span class="sxs-lookup"><span data-stu-id="a623c-105">Review the [Install](install-azurerm-ps.md) article to get Azure PowerShell up and running on your system.</span></span> <span data-ttu-id="a623c-106">Depois, leia o artigo [Get Started](get-started-azureps.md) (Introdução) para começar a utilizá-la.</span><span class="sxs-lookup"><span data-stu-id="a623c-106">Then read the [Get Started](get-started-azureps.md) article to begin using it.</span></span> <span data-ttu-id="a623c-107">Para obter informações sobre a versão mais recente, veja as [notas de versão](release-notes-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="a623c-107">For information about the latest release, see the [release notes](release-notes-azureps.md).</span></span>

<span data-ttu-id="a623c-108">Os exemplos seguintes podem ajudá-lo a saber como utilizar o Azure PowerShell para realizar cenários comuns:</span><span class="sxs-lookup"><span data-stu-id="a623c-108">The following samples can help you learn how to perform common scenarios with Azure PowerShell:</span></span>

* [<span data-ttu-id="a623c-109">Máquinas Virtuais do Linux</span><span class="sxs-lookup"><span data-stu-id="a623c-109">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="a623c-110">Máquinas Virtuais do Windows</span><span class="sxs-lookup"><span data-stu-id="a623c-110">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="a623c-111">Aplicações Web</span><span class="sxs-lookup"><span data-stu-id="a623c-111">Web Apps</span></span>](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="a623c-112">Bases de Dados SQL</span><span class="sxs-lookup"><span data-stu-id="a623c-112">SQL Databases</span></span>](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

> [!NOTE]
> <span data-ttu-id="a623c-113">Se tiver implementações que utilizam o modelo de implementação clássico que não é possível converter, pode instalar a versão de Gestão de Serviço do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a623c-113">If you have deployments that use the classic deployment model that cannot be converted, you can install the Service Management version of Azure PowerShell.</span></span> <span data-ttu-id="a623c-114">Para obter mais informações, veja</span><span class="sxs-lookup"><span data-stu-id="a623c-114">For more information, see</span></span>

<span data-ttu-id="a623c-115">[Instalar o módulo Gestão do Serviço do Azure PowerShell](/powershell/azure/servicemanagement/install-azure-ps).</span><span class="sxs-lookup"><span data-stu-id="a623c-115">[Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span>


### <span data-ttu-id="a623c-116">Necessita ajuda com o PowerShell?</span><span class="sxs-lookup"><span data-stu-id="a623c-116">Need help with PowerShell?</span></span>
<a id="need-help-with-powershell" class="xliff"></a>

<span data-ttu-id="a623c-117">Se não está familiarizado com o PowerShell, uma introdução ao PowerShell poderá útil.</span><span class="sxs-lookup"><span data-stu-id="a623c-117">If you are unfamiliar with PowerShell, you may find an introduction to PowerShell helpful.</span></span> <span data-ttu-id="a623c-118">Para começar a utilizar com o PowerShell, veja [Scripting com o PowerShell](https://technet.microsoft.com/library/bb978526.aspx).</span><span class="sxs-lookup"><span data-stu-id="a623c-118">To get started with PowerShell, see [Scripting with PowerShell](https://technet.microsoft.com/library/bb978526.aspx).</span></span>

<span data-ttu-id="a623c-119">Também pode ver este vídeo: [Noções básicas do PowerShell: (parte 1) Começar a Trabalhar com o PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span><span class="sxs-lookup"><span data-stu-id="a623c-119">You can also watch this video: [PowerShell Basics: (Part 1) Getting Started with PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span></span>

## <span data-ttu-id="a623c-120">Outros módulos do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="a623c-120">Other Azure PowerShell modules</span></span>
<a id="other-azure-powershell-modules" class="xliff"></a>

* [<span data-ttu-id="a623c-121">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="a623c-121">Azure Active Directory</span></span>](/powershell/azure/active-directory/)
* [<span data-ttu-id="a623c-122">Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a623c-122">Azure Information Protection</span></span>](/powershell/azure/aip/)
* [<span data-ttu-id="a623c-123">Azure Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a623c-123">Azure Service Fabric</span></span>](/powershell/azure/oservice-fabric/)
* [<span data-ttu-id="a623c-124">Azure ElasticDB</span><span class="sxs-lookup"><span data-stu-id="a623c-124">Azure ElasticDB</span></span>](/powershell/azure/elasticdbjobs/)
