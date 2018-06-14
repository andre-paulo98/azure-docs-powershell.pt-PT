---
title: Registo de alterações do Azure PowerShell | Microsoft Docs
description: Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: 91d97260568a36e1135196899503fb0c8e1c6731
ms.sourcegitcommit: c98e3a21037ebd82936828bcb544eed902b24212
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/08/2018
ms.locfileid: "34853020"
---
# <a name="release-notes"></a><span data-ttu-id="d6889-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="d6889-103">Release notes</span></span>

<span data-ttu-id="d6889-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="d6889-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-129"></a><span data-ttu-id="d6889-105">Versão 1.2.9</span><span class="sxs-lookup"><span data-stu-id="d6889-105">Version 1.2.9</span></span>

<span data-ttu-id="d6889-106">Alterações nesta Versão</span><span class="sxs-lookup"><span data-stu-id="d6889-106">Changes This Release</span></span>

* <span data-ttu-id="d6889-107">Módulo AzureRm.AzureStackAdmin</span><span class="sxs-lookup"><span data-stu-id="d6889-107">AzureRm.AzureStackAdmin Module</span></span>
    + <span data-ttu-id="d6889-108">Alterações no cmdlet Add-AzureRmResourceProviderRegistration para o suporte do Azure Resource Manager de Administrador e divisão do Azure Resource Manager de inquilino.</span><span class="sxs-lookup"><span data-stu-id="d6889-108">Changes in the Add-AzureRmResourceProviderRegistration cmdlet for the support of Admin Azure resource manager and tenant azure resource manager split.</span></span> <span data-ttu-id="d6889-109">Foi adicionado um novo parâmetro -ResourceManagerType.</span><span class="sxs-lookup"><span data-stu-id="d6889-109">A new parameter -ResourceManagerType has been added.</span></span>
    + <span data-ttu-id="d6889-110">Remoção dos parâmetros - AdminUri, -ApiVersion, -SubscriptionId e -Token de cada um dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="d6889-110">Removal of the parameters -AdminUri, -ApiVersion, -SubscriptionId and -Token from each cmdlets.</span></span> <span data-ttu-id="d6889-111">Temos publicado avisos de que estes parâmetros serão preteridos e agora foram removidos.</span><span class="sxs-lookup"><span data-stu-id="d6889-111">We have been printing warnings that these parameters will be deprecated and now they got removed.</span></span>
* <span data-ttu-id="d6889-112">Módulo AzureStackStorage</span><span class="sxs-lookup"><span data-stu-id="d6889-112">AzureStackStorage module</span></span>
    + <span data-ttu-id="d6889-113">Novos cmdlets adicionados para suportar cenários de migração de contentores.</span><span class="sxs-lookup"><span data-stu-id="d6889-113">Added new cmdlets to support container migration scenarios.</span></span>
    + <span data-ttu-id="d6889-114">Remoção dos cmdlets que fazem referência a componentes internos e funcionalidades subjacentes.</span><span class="sxs-lookup"><span data-stu-id="d6889-114">Removed cmdlets referring to internal components and underlying features.</span></span>
* <span data-ttu-id="d6889-115">AzureRM.BootStrapper</span><span class="sxs-lookup"><span data-stu-id="d6889-115">AzureRM.BootStrapper</span></span>
    + <span data-ttu-id="d6889-116">Novo módulo criado para a gestão de versões de cmdlets do Azure PowerShell através da utilização de perfis de versão</span><span class="sxs-lookup"><span data-stu-id="d6889-116">Created new module to manage versions of Azure PowerShell cmdlets through the use of version profiles</span></span>