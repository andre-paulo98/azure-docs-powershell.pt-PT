---
title: Descrição Geral do Azure PowerShell
description: Uma descrição geral do módulo do Az do Azure PowerShell, com informações sobre como instalar e começar a utilizar.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.manager: carmonm
ms.date: 10/29/2018
ms.openlocfilehash: 7982e122d49db4d558648231d1ab8bfeed80be2d
ms.sourcegitcommit: 4acddc7026522c4fe39de2c4424917d88ee01b7e
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/21/2018
ms.locfileid: "53736465"
---
# <a name="overview-of-azure-powershell"></a><span data-ttu-id="a474e-103">Descrição Geral do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="a474e-103">Overview of Azure PowerShell</span></span>

<span data-ttu-id="a474e-104">O Azure PowerShell fornece um conjunto de cmdlets que utilizam o modelo do [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) para gerir os recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="a474e-104">Azure PowerShell provides a set of cmdlets that use the [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) model for managing your Azure resources.</span></span> <span data-ttu-id="a474e-105">O Azure PowerShell utiliza o .NET Standard, o que significa que o mesmo está disponível para Windows, macOS e Linux.</span><span class="sxs-lookup"><span data-stu-id="a474e-105">Azure PowerShell uses .NET Standard, making it available for Windows, macOS, and Linux.</span></span>
<span data-ttu-id="a474e-106">O Azure PowerShell também está disponível no Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="a474e-106">Azure PowerShell is also available from Azure Cloud Shell.</span></span>

<span data-ttu-id="a474e-107">Utilize o [Azure Cloud Shell](/azure/cloud-shell/overview) para executar o Azure PowerShell no seu browser ou [instale localmente](install-az-ps.md).</span><span class="sxs-lookup"><span data-stu-id="a474e-107">Use [Azure Cloud Shell](/azure/cloud-shell/overview) to run Azure PowerShell in your browser, or [install locally](install-az-ps.md).</span></span> <span data-ttu-id="a474e-108">Consulte o artigo [Introdução](get-started-azureps.md) para se familiarizar com as noções básicas do Azure PowerShell e obter uma introdução ao Azure.</span><span class="sxs-lookup"><span data-stu-id="a474e-108">Check out the [Get Started](get-started-azureps.md) article to learn the Azure PowerShell basics and get started with Azure.</span></span>

<span data-ttu-id="a474e-109">Para obter informações sobre a versão mais recente do Azure PowerShell, veja as [notas de versão](release-notes-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="a474e-109">For information about the latest Azure PowerShell release, see the [release notes](release-notes-azureps.md).</span></span>

## <a name="about-the-new-az-module"></a><span data-ttu-id="a474e-110">Acerca do novo módulo do Az</span><span class="sxs-lookup"><span data-stu-id="a474e-110">About the new Az module</span></span>

<span data-ttu-id="a474e-111">Esta documentação descreve o novo módulo do Az para o Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a474e-111">This documentation describes the new Az module for Azure PowerShell.</span></span> <span data-ttu-id="a474e-112">Este novo módulo foi escrito de raiz com base no .NET Standard.</span><span class="sxs-lookup"><span data-stu-id="a474e-112">This new module is written from the ground up in .NET Standard.</span></span> <span data-ttu-id="a474e-113">A utilização do .NET Standard permite que o Azure PowerShell seja executado no PowerShell 5.x em Windows ou no PowerShell 6 em qualquer plataforma.</span><span class="sxs-lookup"><span data-stu-id="a474e-113">Using .NET Standard allows Azure PowerShell to run under PowerShell 5.x on Windows or PowerShell 6 on any platform.</span></span> <span data-ttu-id="a474e-114">O módulo do Az é agora o modo com se deve interagir com o Azure através do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a474e-114">The Az module is now the intended way to interact with Azure through PowerShell.</span></span>
<span data-ttu-id="a474e-115">O AzureRM irá continuar a ser alvo de correções de erros, mas deixará de receber novas funcionalidades.</span><span class="sxs-lookup"><span data-stu-id="a474e-115">AzureRM will continue to get bug fixes, but no longer receive new features.</span></span>

<span data-ttu-id="a474e-116">Obtenha os detalhes completos sobre o novo módulo, incluindo a mudança de nome dos comandos e os planos de manutenção para o AzureRM, no artigo [Apresentação do módulo do Az do Azure PowerShell](new-azureps-module-az.md).</span><span class="sxs-lookup"><span data-stu-id="a474e-116">Learn the full details about the new module, including how commands have been renamed and the maintenance plans for AzureRM, in the [Introducing the Azure PowerShell Az module](new-azureps-module-az.md).</span></span> <span data-ttu-id="a474e-117">Se pretender começar a utilizar imediatamente o novo módulo, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).</span><span class="sxs-lookup"><span data-stu-id="a474e-117">If you want to get started with using the new module right away, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>

<span data-ttu-id="a474e-118">Também existe [documentação do AzureRM](/powershell/azure/azurerm) disponível.</span><span class="sxs-lookup"><span data-stu-id="a474e-118">The [AzureRM documentation](/powershell/azure/azurerm) is also available.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="a474e-119">Apesar de a documentação do Azure estar a ser alvo de atualizações de modo a refletir os novos nomes de cmdlets do módulo, é possível que os artigos ainda utilizem os comandos do AzureRM.</span><span class="sxs-lookup"><span data-stu-id="a474e-119">While the Azure documentation is being updated to reflect the new module cmdlet names, articles may still use the AzureRM commands.</span></span> <span data-ttu-id="a474e-120">Depois de instalar o módulo do Az, recomenda-se que ative os aliases de cmdlets do AzureRM com `Enable-AzureRmAlias`.</span><span class="sxs-lookup"><span data-stu-id="a474e-120">After installing the Az module, it's recommended that you enable the AzureRM cmdlet aliases with `Enable-AzureRmAlias`.</span></span> <span data-ttu-id="a474e-121">Veja o artigo [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="a474e-121">See the [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md) article for more details.</span></span>

## <a name="common-scenarios"></a><span data-ttu-id="a474e-122">Cenários comuns</span><span class="sxs-lookup"><span data-stu-id="a474e-122">Common scenarios</span></span>

<span data-ttu-id="a474e-123">Os exemplos seguintes podem ajudá-lo a saber como utilizar o Azure PowerShell para realizar cenários comuns:</span><span class="sxs-lookup"><span data-stu-id="a474e-123">The following samples can help you learn how to perform common scenarios with Azure PowerShell:</span></span>

* [<span data-ttu-id="a474e-124">Máquinas Virtuais do Linux</span><span class="sxs-lookup"><span data-stu-id="a474e-124">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="a474e-125">Máquinas Virtuais do Windows</span><span class="sxs-lookup"><span data-stu-id="a474e-125">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="a474e-126">Aplicações Web</span><span class="sxs-lookup"><span data-stu-id="a474e-126">Web Apps</span></span>](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="a474e-127">Bases de Dados SQL</span><span class="sxs-lookup"><span data-stu-id="a474e-127">SQL Databases</span></span>](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

## <a name="learn-powershell-basics"></a><span data-ttu-id="a474e-128">Aprenda as noções básicas do PowerShell</span><span class="sxs-lookup"><span data-stu-id="a474e-128">Learn PowerShell basics</span></span>

<span data-ttu-id="a474e-129">Se não está familiarizado com o PowerShell, uma introdução poderá revelar-se útil.</span><span class="sxs-lookup"><span data-stu-id="a474e-129">If you're unfamiliar with PowerShell, an introduction may be helpful.</span></span>

* [<span data-ttu-id="a474e-130">Instalar o PowerShell</span><span class="sxs-lookup"><span data-stu-id="a474e-130">Installing PowerShell</span></span>](/powershell/scripting/setup/installing-windows-powershell)
* [<span data-ttu-id="a474e-131">Scripting com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="a474e-131">Scripting with PowerShell</span></span>](/powershell/scripting/powershell-scripting)

<span data-ttu-id="a474e-132">Também pode ver este vídeo: [Noções básicas do PowerShell: (Parte 1) Introdução ao PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span><span class="sxs-lookup"><span data-stu-id="a474e-132">You can also watch this video: [PowerShell Basics: (Part 1) Getting Started with PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span></span>

<span data-ttu-id="a474e-133">Ou assista à [Introdução ao Arranque do PowerShell](https://mva.microsoft.com/liveevents/powershell-jumpstart) da Microsoft Virtual Academy.</span><span class="sxs-lookup"><span data-stu-id="a474e-133">Or attend the Microsoft Virtual Academy's [Getting Started with PowerShell Jumpstart](https://mva.microsoft.com/liveevents/powershell-jumpstart).</span></span>

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="a474e-134">Desenvolva as suas competências com o Microsoft Learn</span><span class="sxs-lookup"><span data-stu-id="a474e-134">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="a474e-135">Utilizar scripts para automatizar as tarefas do Azure com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="a474e-135">Automate Azure tasks using scripts with PowerShell</span></span>](/learn/modules/automate-azure-tasks-with-powershell/)
- [<span data-ttu-id="a474e-136">Mais aprendizagem interativa...</span><span class="sxs-lookup"><span data-stu-id="a474e-136">More interactive learning...</span></span>](/learn/browse/?term=powershell)

## <a name="other-azure-powershell-modules"></a><span data-ttu-id="a474e-137">Outros módulos do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="a474e-137">Other Azure PowerShell modules</span></span>

* [<span data-ttu-id="a474e-138">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="a474e-138">Azure Active Directory</span></span>](/powershell/azure/active-directory/)
* [<span data-ttu-id="a474e-139">Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a474e-139">Azure Information Protection</span></span>](/powershell/azure/aip/)
* [<span data-ttu-id="a474e-140">Azure Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a474e-140">Azure Service Fabric</span></span>](/powershell/azure/service-fabric/)
* [<span data-ttu-id="a474e-141">Azure ElasticDB</span><span class="sxs-lookup"><span data-stu-id="a474e-141">Azure ElasticDB</span></span>](/powershell/azure/elasticdbjobs/)
