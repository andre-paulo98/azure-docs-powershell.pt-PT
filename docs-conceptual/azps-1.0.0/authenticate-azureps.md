---
title: Iniciar sessão com o Azure PowerShell
description: Como iniciar sessão com o Azure PowerShell como um utilizador, principal de serviço ou com identidades geridas para recursos do Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/29/2018
ms.openlocfilehash: 8b085720aeabe26c1293ece193e050b31f99a693
ms.sourcegitcommit: ae81b08a45d8729fc8d40156422e3eb2e94de8c7
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/27/2018
ms.locfileid: "53786684"
---
# <a name="sign-in-with-azure-powershell"></a><span data-ttu-id="823cd-103">Iniciar sessão com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="823cd-103">Sign in with Azure PowerShell</span></span>

<span data-ttu-id="823cd-104">O Azure PowerShell suporta vários métodos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="823cd-104">Azure PowerShell supports several authentication methods.</span></span> <span data-ttu-id="823cd-105">A forma mais simples de começar é iniciar sessão interativamente na linha de comandos.</span><span class="sxs-lookup"><span data-stu-id="823cd-105">The simplest way to get started is to sign in interactively at the command line.</span></span>

## <a name="sign-in-interactively"></a><span data-ttu-id="823cd-106">Iniciar sessão interativamente</span><span class="sxs-lookup"><span data-stu-id="823cd-106">Sign in interactively</span></span>

<span data-ttu-id="823cd-107">Para iniciar sessão interativamente, utilize o cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).</span><span class="sxs-lookup"><span data-stu-id="823cd-107">To sign in interactively, use the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>

```azurepowershell-interactive
Connect-AzAccount
```

<span data-ttu-id="823cd-108">Quando é executado, este cmdlet apresenta uma cadeia de token.</span><span class="sxs-lookup"><span data-stu-id="823cd-108">When run, this cmdlet will present a token string.</span></span> <span data-ttu-id="823cd-109">Para iniciar sessão, copie essa cadeia e cole-a em https://microsoft.com/devicelogin num browser.</span><span class="sxs-lookup"><span data-stu-id="823cd-109">To log in, copy this string and paste it into https://microsoft.com/devicelogin in a browser.</span></span> <span data-ttu-id="823cd-110">A sua sessão do PowerShell é autenticada para se ligar ao Azure.</span><span class="sxs-lookup"><span data-stu-id="823cd-110">Your PowerShell session will then be authenticated to connect to Azure.</span></span> <span data-ttu-id="823cd-111">Esta autenticação tem a duração da sessão atual do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="823cd-111">This authentication lasts for the current PowerShell session.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="823cd-112">As suas credenciais são partilhadas entre várias sessões do PowerShell, desde que mantenha a sessão iniciada.</span><span class="sxs-lookup"><span data-stu-id="823cd-112">Your credentials are shared among multiple PowerShell sessions as long as you remain signed in.</span></span>
> <span data-ttu-id="823cd-113">Para obter mais informações, veja o artigo sobre [Credenciais Persistentes](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="823cd-113">For more information, see the article on [Persistent Credentials](context-persistence.md).</span></span>

## <a name="sign-in-with-a-service-principal"></a><span data-ttu-id="823cd-114">Iniciar sessão com um principal de serviço</span><span class="sxs-lookup"><span data-stu-id="823cd-114">Sign in with a service principal</span></span>

<span data-ttu-id="823cd-115">Os principais de serviço são contas não interativas do Azure.</span><span class="sxs-lookup"><span data-stu-id="823cd-115">Service principals are non-interactive Azure accounts.</span></span> <span data-ttu-id="823cd-116">Como outras contas de utilizador, as respetivas permissões são geridas com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="823cd-116">Like other user accounts, their permissions are managed with Azure Active Directory.</span></span> <span data-ttu-id="823cd-117">Ao conceder a um principal de serviço apenas as permissões de que aquele precisa, os seus scripts de automatização permanecem seguros.</span><span class="sxs-lookup"><span data-stu-id="823cd-117">By granting a service principal only the permissions it needs, your automation scripts stay secure.</span></span>

<span data-ttu-id="823cd-118">Para saber como criar um principal de serviço para utilizar com o Azure PowerShell, veja [Criar um principal de serviço do Azure com o Azure PowerShell](create-azure-service-principal-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="823cd-118">To learn how to create a service principal for use with Azure PowerShell, see [Create an Azure service principal with Azure PowerShell](create-azure-service-principal-azureps.md).</span></span>

<span data-ttu-id="823cd-119">Para iniciar sessão com um principal de serviço, utilize o argumento `-ServicePrincipal` com o cmdlet `Connect-AzAccount`.</span><span class="sxs-lookup"><span data-stu-id="823cd-119">To sign in with a service principal, use the `-ServicePrincipal` argument with the `Connect-AzAccount` cmdlet.</span></span> <span data-ttu-id="823cd-120">Também vai precisar do ID de aplicação do principal de serviço, das credenciais de início de sessão e da associação do ID de inquilino ao principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="823cd-120">You'll also need the service principal's application ID, sign-in credentials, and the tenant ID associate with the service principal.</span></span> <span data-ttu-id="823cd-121">Para obter as credenciais do principal de serviço como o objeto adequado, utilize o cmdlet [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential).</span><span class="sxs-lookup"><span data-stu-id="823cd-121">To get the service principal's credentials as the appropriate object, use the [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) cmdlet.</span></span> <span data-ttu-id="823cd-122">Este cmdlet vai apresentar uma linha de comandos para o ID e a palavra-passe de utilizador do principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="823cd-122">This cmdlet will present a prompt for the service principal user ID and password.</span></span>

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
```

## <a name="sign-in-using-an-azure-managed-service-identity"></a><span data-ttu-id="823cd-123">Iniciar sessão com uma Identidade de Serviço Gerida do Azure</span><span class="sxs-lookup"><span data-stu-id="823cd-123">Sign in using an Azure Managed Service Identity</span></span>

<span data-ttu-id="823cd-124">As identidades geridas para os recursos do Azure são uma funcionalidade do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="823cd-124">Managed identities for Azure resources is a feature of Azure Active Directory.</span></span> <span data-ttu-id="823cd-125">Pode utilizar um principal de serviço da identidade gerida para início de sessão e adquirir um token de acesso só de aplicação para aceder a outros recursos.</span><span class="sxs-lookup"><span data-stu-id="823cd-125">You can use a managed identity service principal for sign-in, and acquire an app-only access token to access other resources.</span></span> <span data-ttu-id="823cd-126">As identidades geridas só estão disponíveis em máquinas virtuais em execução numa cloud do Azure.</span><span class="sxs-lookup"><span data-stu-id="823cd-126">Managed identities are only available on virtual machines running in an Azure cloud.</span></span>

<span data-ttu-id="823cd-127">Para obter mais informações sobre identidades geridas para recursos do Azure, veja [Como utilizar identidades geridas para recursos do Azure numa VM do Azure para adquirir um token de acesso](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).</span><span class="sxs-lookup"><span data-stu-id="823cd-127">For more information about managed identities for Azure resources, see [How to use managed identities for Azure resources on an Azure VM to acquire an access token](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).</span></span>

## <a name="sign-in-as-a-cloud-solution-provider-csp"></a><span data-ttu-id="823cd-128">Iniciar a sessão como um Fornecedor de Soluções Cloud (CSP)</span><span class="sxs-lookup"><span data-stu-id="823cd-128">Sign in as a Cloud Solution Provider (CSP)</span></span>

<span data-ttu-id="823cd-129">Um início de sessão do [Fornecedor de Soluções Cloud (CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/) requer a utilização de `-TenantId`.</span><span class="sxs-lookup"><span data-stu-id="823cd-129">A [Cloud Solution Provider (CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/) sign-in requires the use of `-TenantId`.</span></span> <span data-ttu-id="823cd-130">Normalmente, este parâmetro pode ser fornecido como um ID de inquilino ou um nome de domínio.</span><span class="sxs-lookup"><span data-stu-id="823cd-130">Normally, this parameter can be provided as either a tenant ID or a domain name.</span></span> <span data-ttu-id="823cd-131">No entanto, para o início de sessão de CSP, é preciso fornecer um **ID de inquilino**.</span><span class="sxs-lookup"><span data-stu-id="823cd-131">However, for CSP sign-in, it must be provided a **tenant ID**.</span></span>

```azurepowershell-interactive
Connect-AzAccount -TenantId 'xxxx-xxxx-xxxx-xxxx'
```

## <a name="sign-in-to-another-cloud"></a><span data-ttu-id="823cd-132">Iniciar sessão noutra Cloud</span><span class="sxs-lookup"><span data-stu-id="823cd-132">Sign in to another Cloud</span></span>

<span data-ttu-id="823cd-133">Os serviços cloud do Azure oferecem ambientes em conformidade com regulamentos de processamento de dados regionais.</span><span class="sxs-lookup"><span data-stu-id="823cd-133">Azure cloud services offer environments compliant with regional data-handling regulations.</span></span>
<span data-ttu-id="823cd-134">Para as contas numa cloud regional, defina o ambiente quando iniciar sessão com o argumento `-Environment`.</span><span class="sxs-lookup"><span data-stu-id="823cd-134">For accounts in a regional cloud, set the environment when you sign in with the `-Environment` argument.</span></span>
<span data-ttu-id="823cd-135">Por exemplo, se a sua conta está na cloud da China:</span><span class="sxs-lookup"><span data-stu-id="823cd-135">For example, if your account is in the China cloud:</span></span>

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

<span data-ttu-id="823cd-136">O comando seguinte obtém uma lista dos ambientes disponíveis:</span><span class="sxs-lookup"><span data-stu-id="823cd-136">The following command gets a list of available environments:</span></span>

```azurepowershell-interactive
Get-AzEnvironment | Select-Object Name
```

## <a name="learn-more-about-managing-azure-role-based-access"></a><span data-ttu-id="823cd-137">Saiba mais sobre como gerir o acesso baseado em funções do Azure</span><span class="sxs-lookup"><span data-stu-id="823cd-137">Learn more about managing Azure role-based access</span></span>

<span data-ttu-id="823cd-138">Para obter mais informações sobre a gestão de autenticação e de subscrições do Azure, veja [Gerir Contas, Subscrições e Funções Administrativas](/azure/active-directory/role-based-access-control-configure).</span><span class="sxs-lookup"><span data-stu-id="823cd-138">For more information about authentication and subscription management in Azure, see [Manage Accounts, Subscriptions, and Administrative Roles](/azure/active-directory/role-based-access-control-configure).</span></span>

<span data-ttu-id="823cd-139">Cmdlets do Azure PowerShell para a gestão de funções:</span><span class="sxs-lookup"><span data-stu-id="823cd-139">Azure PowerShell cmdlets for role management:</span></span>

* [<span data-ttu-id="823cd-140">Get-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="823cd-140">Get-AzRoleAssignment</span></span>](/powershell/module/az.Resources/Get-azRoleAssignment)
* [<span data-ttu-id="823cd-141">Get-AzRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="823cd-141">Get-AzRoleDefinition</span></span>](/powershell/module/az.Resources/Get-azRoleDefinition)
* [<span data-ttu-id="823cd-142">New-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="823cd-142">New-AzRoleAssignment</span></span>](/powershell/module/az.Resources/New-azRoleAssignment)
* [<span data-ttu-id="823cd-143">New-AzRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="823cd-143">New-AzRoleDefinition</span></span>](/powershell/module/az.Resources/New-azRoleDefinition)
* [<span data-ttu-id="823cd-144">Remove-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="823cd-144">Remove-AzRoleAssignment</span></span>](/powershell/module/az.Resources/Remove-azRoleAssignment)
* [<span data-ttu-id="823cd-145">Remove-AzRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="823cd-145">Remove-AzRoleDefinition</span></span>](/powershell/module/az.Resources/Remove-azRoleDefinition)
* [<span data-ttu-id="823cd-146">Set-AzRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="823cd-146">Set-AzRoleDefinition</span></span>](/powershell/module/az.Resources/Set-azRoleDefinition)
