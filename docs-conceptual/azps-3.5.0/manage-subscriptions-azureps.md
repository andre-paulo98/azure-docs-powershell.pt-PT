---
title: Gerir subscrições do Azure com o Azure PowerShell
description: Gerir subscrições do Azure com o Azure PowerShell
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 02/04/2019
ms.openlocfilehash: 778fdb463a42b609d3a94c910a2c0f9553ef4eb9
ms.sourcegitcommit: a321ef9d134c684fa24ababcbd898f86b00d9364
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/20/2020
ms.locfileid: "77477272"
---
# <a name="use-multiple-azure-subscriptions"></a><span data-ttu-id="41be5-103">Utilizar várias subscrições do Azure</span><span class="sxs-lookup"><span data-stu-id="41be5-103">Use multiple Azure subscriptions</span></span>

<span data-ttu-id="41be5-104">A maioria dos utilizadores do Azure terão apenas uma única subscrição.</span><span class="sxs-lookup"><span data-stu-id="41be5-104">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="41be5-105">No entanto, se fizer parte de várias organizações ou se a sua organização tiver dividido o acesso a determinados recursos entre agrupamentos, pode ter várias subscrições no Azure.</span><span class="sxs-lookup"><span data-stu-id="41be5-105">However, if you are part of more than one organization or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="41be5-106">A CLI suporta a seleção de uma subscrição tanto a nível global como por comando.</span><span class="sxs-lookup"><span data-stu-id="41be5-106">The CLI supports selecting a subscription both globally and per command.</span></span>

<span data-ttu-id="41be5-107">Para obter informações detalhadas sobre subscrições, faturação e gestão de custos, veja a [documentação sobre a gestão da faturação e dos custos](/azure/billing/).</span><span class="sxs-lookup"><span data-stu-id="41be5-107">For detailed information on subscriptions, billing, and cost management, see the [billing and cost management documentation](/azure/billing/).</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="41be5-108">Inquilinos, utilizadores e subscrições</span><span class="sxs-lookup"><span data-stu-id="41be5-108">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="41be5-109">Poderá surgir alguma confusão sobre a diferença entre inquilinos, utilizadores e subscrições no Azure.</span><span class="sxs-lookup"><span data-stu-id="41be5-109">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="41be5-110">Um _inquilino_ é a entidade do Azure Active Directory que abrange uma organização no seu todo.</span><span class="sxs-lookup"><span data-stu-id="41be5-110">A _tenant_ is the Azure Active Directory entity that encompasses a whole organization.</span></span> <span data-ttu-id="41be5-111">Este inquilino tem, pelo menos, uma _subscrição_ e _utilizador_.</span><span class="sxs-lookup"><span data-stu-id="41be5-111">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="41be5-112">Um utilizador é um indivíduo e está associado a apenas um inquilino, a organização a que pertence.</span><span class="sxs-lookup"><span data-stu-id="41be5-112">A user is an individual and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="41be5-113">Os utilizadores são as contas que iniciam sessão no Azure para criar, gerir e utilizar recursos.</span><span class="sxs-lookup"><span data-stu-id="41be5-113">Users are those accounts that sign in to Azure to create, manage, and use resources.</span></span>
<span data-ttu-id="41be5-114">Um utilizador pode ter acesso a várias _subscrições_, que são os contratos com a Microsoft para utilizar serviços cloud, incluindo o Azure.</span><span class="sxs-lookup"><span data-stu-id="41be5-114">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="41be5-115">Cada recurso está associado a uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="41be5-115">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="41be5-116">Para saber mais sobre as diferenças entre inquilinos, utilizadores e subscrições, veja o [Azure cloud terminology dictionary (dicionário de terminologia de cloud do Azure)](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="41be5-116">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>  <span data-ttu-id="41be5-117">Para saber como adicionar uma nova subscrição ao seu inquilino do Azure Active Directory, veja [How to add an Azure subscription to Azure Active Directory (Como adicionar uma subscrição do Azure ao Azure Active Directory)](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="41be5-117">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
<span data-ttu-id="41be5-118">Para saber como iniciar sessão num inquilino específico, veja [Sign in with Azure PowerShell](/powershell/azure/authenticate-azureps) (Iniciar sessão com o Azure PowerShell).</span><span class="sxs-lookup"><span data-stu-id="41be5-118">To learn how to sign in to a specific tenant, see [Sign in with Azure PowerShell](/powershell/azure/authenticate-azureps).</span></span>

## <a name="change-the-active-subscription"></a><span data-ttu-id="41be5-119">Alterar a subscrição ativa</span><span class="sxs-lookup"><span data-stu-id="41be5-119">Change the active subscription</span></span>

<span data-ttu-id="41be5-120">No Azure PowerShell, aceder a recursos para uma subscrição exige a alteração da subscrição associada à sua sessão atual do Azure.</span><span class="sxs-lookup"><span data-stu-id="41be5-120">In Azure PowerShell, accessing the resources for a subscription requires changing the subscription associated with your current Azure session.</span></span>
<span data-ttu-id="41be5-121">Isto é feito ao modificar o contexto da sessão ativa, as informações sobre quais os cmdlets do inquilino, da subscrição e do utilizador devem ser executados.</span><span class="sxs-lookup"><span data-stu-id="41be5-121">This is done by modifying the active session context, the information about which tenant, subscription, and user cmdlets should be run against.</span></span>
<span data-ttu-id="41be5-122">Para alterar as subscrições, é necessário obter primeiro um objeto de contexto do Azure PowerShell com [Get-AzSubscription](/powershell/module/az.accounts/get-azsubscription) e, em seguida, alterar o contexto atual com [Set-AzContext](/powershell/module/az.accounts/set-azcontext).</span><span class="sxs-lookup"><span data-stu-id="41be5-122">In order to change subscriptions, an Azure PowerShell Context object first needs to be retrieved with [Get-AzSubscription](/powershell/module/az.accounts/get-azsubscription) and then the current context changed with [Set-AzContext](/powershell/module/az.accounts/set-azcontext).</span></span>

<span data-ttu-id="41be5-123">O exemplo seguinte mostra como obter uma subscrição no inquilino atualmente ativo e defini-lo como a sessão ativa:</span><span class="sxs-lookup"><span data-stu-id="41be5-123">The next example shows how to get a subscription in the currently active tenant, and set it as the active session:</span></span>

```powershell-interactive
$context = Get-AzSubscription -SubscriptionId ...
Set-AzContext $context
```

<span data-ttu-id="41be5-124">Para obter mais informações sobre contextos do Azure PowerShell, incluindo como guardá-los e alternar rapidamente entre os mesmos para utilizar facilmente múltiplas subscrições, veja [Persist credentials with Azure PowerShell contexts](context-persistence.md) (Manter as credenciais nos contextos do Azure PowerShell).</span><span class="sxs-lookup"><span data-stu-id="41be5-124">To learn more about Azure PowerShell contexts, including how to save them and quickly switch between them for working with multiple subscriptions easily, see [Persist credentials with Azure PowerShell contexts](context-persistence.md).</span></span>