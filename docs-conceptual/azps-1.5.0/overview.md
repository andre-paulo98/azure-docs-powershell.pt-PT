---
title: Descrição Geral do Azure PowerShell
description: Uma descrição geral do módulo do Az do Azure PowerShell, com informações sobre como instalar e começar a utilizar.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.manager: carmonm
ms.date: 01/10/2019
ms.openlocfilehash: 45ab083dd133c8c7b8dbe902484c92564bc216b9
ms.sourcegitcommit: 447276d46ffeeb37f0c07a570536665e36c5ddb8
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/14/2019
ms.locfileid: "57882393"
---
# <a name="overview-of-azure-powershell"></a><span data-ttu-id="c9222-103">Descrição Geral do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c9222-103">Overview of Azure PowerShell</span></span>

<span data-ttu-id="c9222-104">O Azure PowerShell fornece um conjunto de cmdlets que utilizam o modelo do [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) para gerir os recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="c9222-104">Azure PowerShell provides a set of cmdlets that use the [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) model for managing your Azure resources.</span></span> <span data-ttu-id="c9222-105">O Azure PowerShell utiliza o .NET Standard, o que significa que o mesmo está disponível para Windows, macOS e Linux.</span><span class="sxs-lookup"><span data-stu-id="c9222-105">Azure PowerShell uses .NET Standard, making it available for Windows, macOS, and Linux.</span></span>
<span data-ttu-id="c9222-106">O Azure PowerShell também está disponível no Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="c9222-106">Azure PowerShell is also available on Azure Cloud Shell.</span></span>

## <a name="about-the-new-az-module"></a><span data-ttu-id="c9222-107">Acerca do novo módulo do Az</span><span class="sxs-lookup"><span data-stu-id="c9222-107">About the new Az module</span></span>

<span data-ttu-id="c9222-108">Esta documentação descreve o novo módulo do Az para o Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c9222-108">This documentation describes the new Az module for Azure PowerShell.</span></span> <span data-ttu-id="c9222-109">Este novo módulo foi escrito de raiz com base no .NET Standard.</span><span class="sxs-lookup"><span data-stu-id="c9222-109">This new module is written from the ground up in .NET Standard.</span></span> <span data-ttu-id="c9222-110">A utilização do .NET Standard permite executar o Azure PowerShell no PowerShell 5, no Windows ou no PowerShell 6 em qualquer plataforma.</span><span class="sxs-lookup"><span data-stu-id="c9222-110">Using .NET Standard allows Azure PowerShell to run under PowerShell 5 on Windows or PowerShell 6 on any platform.</span></span> <span data-ttu-id="c9222-111">O módulo do Az é agora o modo com se deve interagir com o Azure através do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c9222-111">The Az module is now the intended way to interact with Azure through PowerShell.</span></span>
<span data-ttu-id="c9222-112">O AzureRM irá continuar a ser alvo de correções de erros, mas deixará de receber novas funcionalidades.</span><span class="sxs-lookup"><span data-stu-id="c9222-112">AzureRM will continue to get bug fixes, but no longer receive new features.</span></span>

<span data-ttu-id="c9222-113">Obtenha os detalhes completos sobre o novo módulo, incluindo a mudança de nome dos comandos e os planos de manutenção para o AzureRM, no artigo [Apresentação do módulo do Az do Azure PowerShell](new-azureps-module-az.md).</span><span class="sxs-lookup"><span data-stu-id="c9222-113">Learn the full details about the new module, including how commands have been renamed and the maintenance plans for AzureRM, in the [Introducing the Azure PowerShell Az module](new-azureps-module-az.md).</span></span> <span data-ttu-id="c9222-114">Se pretender começar a utilizar imediatamente o novo módulo, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).</span><span class="sxs-lookup"><span data-stu-id="c9222-114">If you want to get started with using the new module right away, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>

<span data-ttu-id="c9222-115">Também existe [documentação do AzureRM](/powershell/azure/azurerm) disponível.</span><span class="sxs-lookup"><span data-stu-id="c9222-115">The [AzureRM documentation](/powershell/azure/azurerm) is also available.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="c9222-116">Apesar de a documentação do Azure estar a ser alvo de atualizações de modo a refletir os novos nomes de cmdlets do módulo, é possível que os artigos ainda utilizem os comandos do AzureRM.</span><span class="sxs-lookup"><span data-stu-id="c9222-116">While the Azure documentation is being updated to reflect the new module cmdlet names, articles may still use the AzureRM commands.</span></span> <span data-ttu-id="c9222-117">Depois de instalar o módulo do Az, recomenda-se que ative os aliases de cmdlets do AzureRM com `Enable-AzureRmAlias`.</span><span class="sxs-lookup"><span data-stu-id="c9222-117">After installing the Az module, it's recommended that you enable the AzureRM cmdlet aliases with `Enable-AzureRmAlias`.</span></span> <span data-ttu-id="c9222-118">Veja o artigo [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="c9222-118">See the [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md) article for more details.</span></span>

## <a name="run-or-install"></a><span data-ttu-id="c9222-119">Executar ou instalar</span><span class="sxs-lookup"><span data-stu-id="c9222-119">Run or install</span></span>

<span data-ttu-id="c9222-120">Pode instalar o Azure PowerShell no PowerShell 5.1 ou superior no Windows e no PowerShell 6 em qualquer plataforma, ou pode optar por executá-lo no Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="c9222-120">You can install Azure PowerShell on PowerShell 5.1 or higher on Windows, PowerShell 6 on any platform, or run in Azure Cloud Shell.</span></span>

* <span data-ttu-id="c9222-121">Para executar no browser com o Azure Cloud Shell, veja [Início Rápido do PowerShell no Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span><span class="sxs-lookup"><span data-stu-id="c9222-121">To run in your browser with Azure Cloud Shell, see [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
* <span data-ttu-id="c9222-122">Para instalar o Azure PowerShell no seu sistema, veja [Instalar o Azure PowerShell](install-az-ps.md).</span><span class="sxs-lookup"><span data-stu-id="c9222-122">To install Azure PowerShell on your system, see [Install Azure PowerShell](install-az-ps.md).</span></span>

<span data-ttu-id="c9222-123">Para obter informações sobre a versão mais recente do Azure PowerShell, veja as [notas de versão](release-notes-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="c9222-123">For information about the latest Azure PowerShell release, see the [release notes](release-notes-azureps.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="c9222-124">Introdução</span><span class="sxs-lookup"><span data-stu-id="c9222-124">Get Started</span></span>

<span data-ttu-id="c9222-125">Leia o artigo [Introdução ao Azure PowerShell](get-started-azureps.md) para aprender as noções básicas do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c9222-125">Read the [Get Started with Azure PowerShell](get-started-azureps.md) article to learn the Azure PowerShell basics.</span></span> <span data-ttu-id="c9222-126">Se não está familiarizado com o PowerShell, uma introdução poderá revelar-se útil:</span><span class="sxs-lookup"><span data-stu-id="c9222-126">If you're not familiar with PowerShell, an introduction might be helpful:</span></span>

* [<span data-ttu-id="c9222-127">Instalar o PowerShell</span><span class="sxs-lookup"><span data-stu-id="c9222-127">Install PowerShell</span></span>](/powershell/scripting/install/installing-powershell)
* [<span data-ttu-id="c9222-128">Scripting com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="c9222-128">Scripting with PowerShell</span></span>](/powershell/scripting/powershell-scripting)
* [<span data-ttu-id="c9222-129">Noções básicas do PowerShell: (Parte 1) Introdução ao PowerShell</span><span class="sxs-lookup"><span data-stu-id="c9222-129">PowerShell Basics: (Part 1) Getting Started with PowerShell</span></span>](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1)
* <span data-ttu-id="c9222-130">[Introdução ao Arranque do PowerShell](https://mva.microsoft.com/liveevents/powershell-jumpstart) da Microsoft Virtual Academy</span><span class="sxs-lookup"><span data-stu-id="c9222-130">Microsoft Virtual Academy's [Getting Started with PowerShell Jumpstart](https://mva.microsoft.com/liveevents/powershell-jumpstart)</span></span>

<span data-ttu-id="c9222-131">Os exemplos seguintes podem ajudá-lo com algumas utilizações comuns do Azure:</span><span class="sxs-lookup"><span data-stu-id="c9222-131">The following samples can help you with some common uses of Azure:</span></span>

* [<span data-ttu-id="c9222-132">Máquinas Virtuais do Linux</span><span class="sxs-lookup"><span data-stu-id="c9222-132">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="c9222-133">Máquinas Virtuais do Windows</span><span class="sxs-lookup"><span data-stu-id="c9222-133">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="c9222-134">Aplicações Web</span><span class="sxs-lookup"><span data-stu-id="c9222-134">Web Apps</span></span>](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="c9222-135">Bases de Dados SQL</span><span class="sxs-lookup"><span data-stu-id="c9222-135">SQL Databases</span></span>](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="c9222-136">Desenvolva as suas competências com o Microsoft Learn</span><span class="sxs-lookup"><span data-stu-id="c9222-136">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="c9222-137">Utilizar scripts para automatizar as tarefas do Azure com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="c9222-137">Automate Azure tasks using scripts with PowerShell</span></span>](/learn/modules/automate-azure-tasks-with-powershell/)
- [<span data-ttu-id="c9222-138">Mais aprendizagem interativa...</span><span class="sxs-lookup"><span data-stu-id="c9222-138">More interactive learning...</span></span>](/learn/browse/?term=powershell)

## <a name="other-azure-powershell-modules"></a><span data-ttu-id="c9222-139">Outros módulos do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c9222-139">Other Azure PowerShell modules</span></span>

* [<span data-ttu-id="c9222-140">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="c9222-140">Azure Active Directory</span></span>](/powershell/azure/active-directory/)
* [<span data-ttu-id="c9222-141">Azure Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c9222-141">Azure Service Fabric</span></span>](/powershell/azure/service-fabric/)
* [<span data-ttu-id="c9222-142">Azure ElasticDB</span><span class="sxs-lookup"><span data-stu-id="c9222-142">Azure ElasticDB</span></span>](/powershell/azure/elasticdbjobs/)
