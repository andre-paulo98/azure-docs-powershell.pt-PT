---
title: Registo de alterações do Azure PowerShell | Microsoft Docs
description: Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente.
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: b42ad6f22f47e10c9190cf5a919f781375ff26f2
ms.sourcegitcommit: 5971c92cb023bdd1d71fa2ad0a3b378abfbd092a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/23/2018
---
# <a name="release-notes"></a><span data-ttu-id="25dd6-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="25dd6-103">Release notes</span></span>

<span data-ttu-id="25dd6-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="25dd6-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-129"></a><span data-ttu-id="25dd6-105">Versão 1.2.9</span><span class="sxs-lookup"><span data-stu-id="25dd6-105">Version 1.2.9</span></span>

<span data-ttu-id="25dd6-106">Alterações nesta Versão</span><span class="sxs-lookup"><span data-stu-id="25dd6-106">Changes This Release</span></span>

* <span data-ttu-id="25dd6-107">Módulo AzureRm.AzureStackAdmin</span><span class="sxs-lookup"><span data-stu-id="25dd6-107">AzureRm.AzureStackAdmin Module</span></span>
    + <span data-ttu-id="25dd6-108">Alterações no cmdlet Add-AzureRmResourceProviderRegistration para o suporte do Azure Resource Manager de Administrador e divisão do Azure Resource Manager de inquilino.</span><span class="sxs-lookup"><span data-stu-id="25dd6-108">Changes in the Add-AzureRmResourceProviderRegistration cmdlet for the support of Admin Azure resource manager and tenant azure resource manager split.</span></span> <span data-ttu-id="25dd6-109">Foi adicionado um novo parâmetro -ResourceManagerType.</span><span class="sxs-lookup"><span data-stu-id="25dd6-109">A new parameter -ResourceManagerType has been added.</span></span>
    + <span data-ttu-id="25dd6-110">Remoção dos parâmetros - AdminUri, -ApiVersion, -SubscriptionId e -Token de cada um dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="25dd6-110">Removal of the parameters -AdminUri, -ApiVersion, -SubscriptionId and -Token from each cmdlets.</span></span> <span data-ttu-id="25dd6-111">Temos publicado avisos de que estes parâmetros serão preteridos e agora foram removidos.</span><span class="sxs-lookup"><span data-stu-id="25dd6-111">We have been printing warnings that these parameters will be deprecated and now they got removed.</span></span>
* <span data-ttu-id="25dd6-112">Módulo AzureStackStorage</span><span class="sxs-lookup"><span data-stu-id="25dd6-112">AzureStackStorage module</span></span>
    + <span data-ttu-id="25dd6-113">Novos cmdlets adicionados para suportar cenários de migração de contentores.</span><span class="sxs-lookup"><span data-stu-id="25dd6-113">Added new cmdlets to support container migration scenarios.</span></span>
    + <span data-ttu-id="25dd6-114">Remoção dos cmdlets que fazem referência a componentes internos e funcionalidades subjacentes.</span><span class="sxs-lookup"><span data-stu-id="25dd6-114">Removed cmdlets referring to internal components and underlying features.</span></span>
* <span data-ttu-id="25dd6-115">AzureRM.BootStrapper</span><span class="sxs-lookup"><span data-stu-id="25dd6-115">AzureRM.BootStrapper</span></span>
    + <span data-ttu-id="25dd6-116">Novo módulo criado para a gestão de versões de cmdlets do Azure PowerShell através da utilização de perfis de versão</span><span class="sxs-lookup"><span data-stu-id="25dd6-116">Created new module to manage versions of Azure PowerShell cmdlets through the use of version profiles</span></span>