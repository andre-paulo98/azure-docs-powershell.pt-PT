---
title: Iniciar sessão com o Azure PowerShell
description: Como iniciar sessão com o Azure PowerShell como um utilizador, principal de serviço ou com identidades geridas para recursos do Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/09/2018
ms.openlocfilehash: c19d9ade0f69f4af9f14c68ad22b327c27c8ccfd
ms.sourcegitcommit: 5f946a535eccca0b3ddf3db8f617b32564a88938
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/25/2018
ms.locfileid: "50001308"
---
# <a name="sign-in-with-azure-powershell"></a><span data-ttu-id="f3216-103">Iniciar sessão com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="f3216-103">Sign in with Azure PowerShell</span></span>

<span data-ttu-id="f3216-104">O Azure PowerShell suporta vários métodos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="f3216-104">Azure PowerShell supports several authentication methods.</span></span> <span data-ttu-id="f3216-105">A forma mais simples de começar é iniciar sessão interativamente na linha de comandos.</span><span class="sxs-lookup"><span data-stu-id="f3216-105">The simplest way to get started is to sign in interactively at the command line.</span></span>

## <a name="sign-in-interactively"></a><span data-ttu-id="f3216-106">Iniciar sessão interativamente</span><span class="sxs-lookup"><span data-stu-id="f3216-106">Sign in interactively</span></span>

<span data-ttu-id="f3216-107">Para iniciar sessão interativamente, utilize o cmdlet [Connect-AzureRmAccount](/powershell/module/azurerm.profile/connect-azurermaccount).</span><span class="sxs-lookup"><span data-stu-id="f3216-107">To sign in interactively, use the [Connect-AzureRmAccount](/powershell/module/azurerm.profile/connect-azurermaccount) cmdlet.</span></span>

```azurepowershell
Connect-AzureRmAccount
```

<span data-ttu-id="f3216-108">Quando é executado, este cmdlet apresenta uma caixa de diálogo que lhe pede para indicar o endereço de e-mail e a palavra-passe associados à sua conta do Azure.</span><span class="sxs-lookup"><span data-stu-id="f3216-108">When run, this cmdlet will bring up a dialog box prompting you for your email address and password associated with your Azure account.</span></span> <span data-ttu-id="f3216-109">Esta autenticação tem a duração da sessão atual do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f3216-109">This authentication lasts for the current PowerShell session.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f3216-110">A partir do Azure PowerShell 6.3.0, as suas credenciais são partilhadas entre várias sessões do PowerShell, desde que mantenha sessão iniciada no Windows.</span><span class="sxs-lookup"><span data-stu-id="f3216-110">As of Azure PowerShell 6.3.0, your credentials are shared among multiple PowerShell sessions as long as you remain signed in to Windows.</span></span> <span data-ttu-id="f3216-111">Para obter mais informações, veja o artigo sobre [Credenciais Persistentes](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="f3216-111">For more information, see the article on [Persistent Credentials](context-persistence.md).</span></span>

## <a name="sign-in-with-a-service-principal"></a><span data-ttu-id="f3216-112">Iniciar sessão com um principal de serviço</span><span class="sxs-lookup"><span data-stu-id="f3216-112">Sign in with a service principal</span></span>

<span data-ttu-id="f3216-113">Os principais de serviço são contas não interativas do Azure.</span><span class="sxs-lookup"><span data-stu-id="f3216-113">Service principals are non-interactive Azure accounts.</span></span> <span data-ttu-id="f3216-114">Como outras contas de utilizador, as respetivas permissões são geridas com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f3216-114">Like other user accounts, their permissions are managed with Azure Active Directory.</span></span> <span data-ttu-id="f3216-115">Ao conceder a um principal de serviço apenas as permissões de que aquele precisa, os seus scripts de automatização permanecem seguros.</span><span class="sxs-lookup"><span data-stu-id="f3216-115">By granting a service principal only the permissions it needs, your automation scripts stay secure.</span></span>

<span data-ttu-id="f3216-116">Para saber como criar um principal de serviço para utilizar com o Azure PowerShell, veja [Criar um principal de serviço do Azure com o Azure PowerShell](create-azure-service-principal-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="f3216-116">To learn how to create a service principal for use with Azure PowerShell, see [Create an Azure service principal with Azure PowerShell](create-azure-service-principal-azureps.md).</span></span>

<span data-ttu-id="f3216-117">Para iniciar sessão com um principal de serviço, utilize o argumento `-ServicePrincipal` com o cmdlet `Connect-AzureRmAccount`.</span><span class="sxs-lookup"><span data-stu-id="f3216-117">To sign in with a service principal, use the `-ServicePrincipal` argument with the `Connect-AzureRmAccount` cmdlet.</span></span> <span data-ttu-id="f3216-118">Também vai precisar do ID de aplicação do principal de serviço, das credenciais de início de sessão e da associação do ID de inquilino ao principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="f3216-118">You'll also need the service principal's application ID, sign-in credentials, and the tenant ID associate with the service principal.</span></span> <span data-ttu-id="f3216-119">Para obter as credenciais do principal de serviço como o objeto adequado, utilize o cmdlet [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential).</span><span class="sxs-lookup"><span data-stu-id="f3216-119">To get the service principal's credentials as the appropriate object, use the [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) cmdlet.</span></span> <span data-ttu-id="f3216-120">Este cmdlet irá apresentar uma caixa de diálogo para introduzir o ID de utilizador e a palavra-passe do principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="f3216-120">This cmdlet will display a dialog box to enter the service principal user ID and password into.</span></span>

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzureRmAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
```

## <a name="sign-in-using-an-azure-managed-service-identity"></a><span data-ttu-id="f3216-121">Iniciar sessão com uma Identidade de Serviço Gerida do Azure</span><span class="sxs-lookup"><span data-stu-id="f3216-121">Sign in using an Azure Managed Service Identity</span></span>

<span data-ttu-id="f3216-122">As identidades geridas para os recursos do Azure são uma funcionalidade do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f3216-122">Managed identities for Azure resources is a feature of Azure Active Directory.</span></span> <span data-ttu-id="f3216-123">Pode utilizar um principal de serviço da identidade gerida para início de sessão e adquirir um token de acesso só de aplicação para aceder a outros recursos.</span><span class="sxs-lookup"><span data-stu-id="f3216-123">You can use a managed identity service principal for sign-in, and acquire an app-only access token to access other resources.</span></span> <span data-ttu-id="f3216-124">As identidades geridas só estão disponíveis em máquinas virtuais em execução numa cloud do Azure.</span><span class="sxs-lookup"><span data-stu-id="f3216-124">Managed identities are only available on virtual machines running in an Azure cloud.</span></span>

<span data-ttu-id="f3216-125">Para obter mais informações sobre identidades geridas para recursos do Azure, veja [Como utilizar identidades geridas para recursos do Azure numa VM do Azure para adquirir um token de acesso](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).</span><span class="sxs-lookup"><span data-stu-id="f3216-125">For more information about managed identities for Azure resources, see [How to use managed identities for Azure resources on an Azure VM to acquire an access token](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).</span></span>

## <a name="sign-in-as-a-cloud-solution-provider-csp"></a><span data-ttu-id="f3216-126">Iniciar a sessão como um Fornecedor de Soluções Cloud (CSP)</span><span class="sxs-lookup"><span data-stu-id="f3216-126">Sign in as a Cloud Solution Provider (CSP)</span></span>

<span data-ttu-id="f3216-127">Um início de sessão do [Fornecedor de Soluções Cloud (CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/) requer a utilização de `-TenantId`.</span><span class="sxs-lookup"><span data-stu-id="f3216-127">A [Cloud Solution Provider (CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/) sign-in requires the use of `-TenantId`.</span></span> <span data-ttu-id="f3216-128">Normalmente, este parâmetro pode ser fornecido como um ID de inquilino ou um nome de domínio.</span><span class="sxs-lookup"><span data-stu-id="f3216-128">Normally, this parameter can be provided as either a tenant ID or a domain name.</span></span> <span data-ttu-id="f3216-129">No entanto, para o início de sessão de CSP, é preciso fornecer um **ID de inquilino**.</span><span class="sxs-lookup"><span data-stu-id="f3216-129">However, for CSP sign-in, it must be provided a **tenant ID**.</span></span>

```azurepowershell-interactive
Connect-AzureRmAccount -TenantId 'xxxx-xxxx-xxxx-xxxx'
```

## <a name="sign-in-to-another-cloud"></a><span data-ttu-id="f3216-130">Iniciar sessão noutra Cloud</span><span class="sxs-lookup"><span data-stu-id="f3216-130">Sign in to another Cloud</span></span>

<span data-ttu-id="f3216-131">Os serviços cloud do Azure oferecem ambientes em conformidade com regulamentos de processamento de dados regionais.</span><span class="sxs-lookup"><span data-stu-id="f3216-131">Azure cloud services offer environments compliant with regional data-handling regulations.</span></span>
<span data-ttu-id="f3216-132">Para as contas numa cloud regional, defina o ambiente quando iniciar sessão com o argumento `-Environment`.</span><span class="sxs-lookup"><span data-stu-id="f3216-132">For accounts in a regional cloud, set the environment when you sign in with the `-Environment` argument.</span></span>
<span data-ttu-id="f3216-133">Por exemplo, se a sua conta está na cloud da China:</span><span class="sxs-lookup"><span data-stu-id="f3216-133">For example, if your account is in the China cloud:</span></span>

```azurepowershell-interactive
Connect-AzureRmAccount -Environment AzureChinaCloud
```

<span data-ttu-id="f3216-134">O comando seguinte obtém uma lista dos ambientes disponíveis:</span><span class="sxs-lookup"><span data-stu-id="f3216-134">The following command gets a list of available environments:</span></span>

```azurepowershell-interactive
Get-AzureRmEnvironment | Select-Object Name
```

## <a name="learn-more-about-managing-azure-role-based-access"></a><span data-ttu-id="f3216-135">Saiba mais sobre como gerir o acesso baseado em funções do Azure</span><span class="sxs-lookup"><span data-stu-id="f3216-135">Learn more about managing Azure role-based access</span></span>

<span data-ttu-id="f3216-136">Para obter mais informações sobre a gestão de autenticação e de subscrições do Azure, veja [Gerir Contas, Subscrições e Funções Administrativas](/azure/active-directory/role-based-access-control-configure).</span><span class="sxs-lookup"><span data-stu-id="f3216-136">For more information about authentication and subscription management in Azure, see [Manage Accounts, Subscriptions, and Administrative Roles](/azure/active-directory/role-based-access-control-configure).</span></span>

<span data-ttu-id="f3216-137">Cmdlets do Azure PowerShell para a gestão de funções:</span><span class="sxs-lookup"><span data-stu-id="f3216-137">Azure PowerShell cmdlets for role management:</span></span>

* [<span data-ttu-id="f3216-138">Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f3216-138">Get-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/Get-AzureRmRoleAssignment)
* [<span data-ttu-id="f3216-139">Get-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f3216-139">Get-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Get-AzureRmRoleDefinition)
* [<span data-ttu-id="f3216-140">New-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f3216-140">New-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/New-AzureRmRoleAssignment)
* [<span data-ttu-id="f3216-141">New-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f3216-141">New-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/New-AzureRmRoleDefinition)
* [<span data-ttu-id="f3216-142">Remove-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f3216-142">Remove-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleAssignment)
* [<span data-ttu-id="f3216-143">Remove-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f3216-143">Remove-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleDefinition)
* [<span data-ttu-id="f3216-144">Set-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f3216-144">Set-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Set-AzureRmRoleDefinition)
