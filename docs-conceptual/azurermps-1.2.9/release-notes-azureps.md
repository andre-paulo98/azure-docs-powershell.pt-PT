---
title: Registo de alterações do Azure PowerShell | Microsoft Docs
description: Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente.
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: c57ba563b5a4d4d19944fe8eca2cb4244ee5ed9e
ms.sourcegitcommit: 2eea03b7ac19ad6d7c8097743d33c7ddb9c4df77
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/06/2018
ms.locfileid: "34819716"
---
# <a name="release-notes"></a><span data-ttu-id="01a14-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="01a14-103">Release notes</span></span>

<span data-ttu-id="01a14-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="01a14-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-129"></a><span data-ttu-id="01a14-105">Versão 1.2.9</span><span class="sxs-lookup"><span data-stu-id="01a14-105">Version 1.2.9</span></span>

<span data-ttu-id="01a14-106">Alterações nesta Versão</span><span class="sxs-lookup"><span data-stu-id="01a14-106">Changes This Release</span></span>

* <span data-ttu-id="01a14-107">Módulo AzureRm.AzureStackAdmin</span><span class="sxs-lookup"><span data-stu-id="01a14-107">AzureRm.AzureStackAdmin Module</span></span>
    + <span data-ttu-id="01a14-108">Alterações no cmdlet Add-AzureRmResourceProviderRegistration para o suporte do Azure Resource Manager de Administrador e divisão do Azure Resource Manager de inquilino.</span><span class="sxs-lookup"><span data-stu-id="01a14-108">Changes in the Add-AzureRmResourceProviderRegistration cmdlet for the support of Admin Azure resource manager and tenant azure resource manager split.</span></span> <span data-ttu-id="01a14-109">Foi adicionado um novo parâmetro -ResourceManagerType.</span><span class="sxs-lookup"><span data-stu-id="01a14-109">A new parameter -ResourceManagerType has been added.</span></span>
    + <span data-ttu-id="01a14-110">Remoção dos parâmetros - AdminUri, -ApiVersion, -SubscriptionId e -Token de cada um dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="01a14-110">Removal of the parameters -AdminUri, -ApiVersion, -SubscriptionId and -Token from each cmdlets.</span></span> <span data-ttu-id="01a14-111">Temos publicado avisos de que estes parâmetros serão preteridos e agora foram removidos.</span><span class="sxs-lookup"><span data-stu-id="01a14-111">We have been printing warnings that these parameters will be deprecated and now they got removed.</span></span>
* <span data-ttu-id="01a14-112">Módulo AzureStackStorage</span><span class="sxs-lookup"><span data-stu-id="01a14-112">AzureStackStorage module</span></span>
    + <span data-ttu-id="01a14-113">Novos cmdlets adicionados para suportar cenários de migração de contentores.</span><span class="sxs-lookup"><span data-stu-id="01a14-113">Added new cmdlets to support container migration scenarios.</span></span>
    + <span data-ttu-id="01a14-114">Remoção dos cmdlets que fazem referência a componentes internos e funcionalidades subjacentes.</span><span class="sxs-lookup"><span data-stu-id="01a14-114">Removed cmdlets referring to internal components and underlying features.</span></span>
* <span data-ttu-id="01a14-115">AzureRM.BootStrapper</span><span class="sxs-lookup"><span data-stu-id="01a14-115">AzureRM.BootStrapper</span></span>
    + <span data-ttu-id="01a14-116">Novo módulo criado para a gestão de versões de cmdlets do Azure PowerShell através da utilização de perfis de versão</span><span class="sxs-lookup"><span data-stu-id="01a14-116">Created new module to manage versions of Azure PowerShell cmdlets through the use of version profiles</span></span>