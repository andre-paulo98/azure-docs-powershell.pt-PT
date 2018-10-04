---
title: Iniciar sessão com o Azure PowerShell
description: Como iniciar sessão com o Azure PowerShell como um utilizador, principal de serviço ou com identidades geridas para recursos do Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/09/2018
ms.openlocfilehash: 2a118e1aa8b6755ef5769f44429427d22532780d
ms.sourcegitcommit: 6c38e86e16da99f65cd183c63e34f7176b121ab8
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/04/2018
ms.locfileid: "47425249"
---
# <a name="sign-in-with-azure-powershell"></a><span data-ttu-id="85022-103">Iniciar sessão com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="85022-103">Sign in with Azure PowerShell</span></span>

<span data-ttu-id="85022-104">O Azure PowerShell suporta vários métodos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="85022-104">Azure PowerShell supports several authentication methods.</span></span> <span data-ttu-id="85022-105">A forma mais simples de começar é iniciar sessão interativamente na linha de comandos.</span><span class="sxs-lookup"><span data-stu-id="85022-105">The simplest way to get started is to sign in interactively at the command line.</span></span>

## <a name="sign-in-interactively"></a><span data-ttu-id="85022-106">Iniciar sessão interativamente</span><span class="sxs-lookup"><span data-stu-id="85022-106">Sign in interactively</span></span>

<span data-ttu-id="85022-107">Para iniciar sessão interativamente, utilize o cmdlet [Connect-AzureRmAccount](/powershell/module/azurerm.profile/connect-azurermaccount).</span><span class="sxs-lookup"><span data-stu-id="85022-107">To sign in interactively, use the [Connect-AzureRmAccount](/powershell/module/azurerm.profile/connect-azurermaccount) cmdlet.</span></span>

```azurepowershell
Connect-AzureRmAccount
```

<span data-ttu-id="85022-108">Quando é executado, este cmdlet apresenta uma caixa de diálogo que lhe pede para indicar o endereço de e-mail e a palavra-passe associados à sua conta do Azure.</span><span class="sxs-lookup"><span data-stu-id="85022-108">When run, this cmdlet will bring up a dialog box prompting you for your email address and password associated with your Azure account.</span></span> <span data-ttu-id="85022-109">Esta autenticação tem a duração da sessão atual do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="85022-109">This authentication lasts for the current PowerShell session.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="85022-110">A partir do Azure PowerShell 6.3.0, as suas credenciais são partilhadas entre várias sessões do PowerShell, desde que mantenha sessão iniciada no Windows.</span><span class="sxs-lookup"><span data-stu-id="85022-110">As of Azure PowerShell 6.3.0, your credentials are shared among multiple PowerShell sessions as long as you remain signed in to Windows.</span></span> <span data-ttu-id="85022-111">Para obter mais informações, veja o artigo sobre [Credenciais Persistentes](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="85022-111">For more information, see the article on [Persistent Credentials](context-persistence.md).</span></span>

## <a name="sign-in-with-a-service-principal"></a><span data-ttu-id="85022-112">Iniciar sessão com um principal de serviço</span><span class="sxs-lookup"><span data-stu-id="85022-112">Sign in with a service principal</span></span>

<span data-ttu-id="85022-113">Os principais de serviço são contas não interativas do Azure.</span><span class="sxs-lookup"><span data-stu-id="85022-113">Service principals are non-interactive Azure accounts.</span></span> <span data-ttu-id="85022-114">Como outras contas de utilizador, as respetivas permissões são geridas com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="85022-114">Like other user accounts, their permissions are managed with Azure Active Directory.</span></span> <span data-ttu-id="85022-115">Ao conceder a um principal de serviço apenas as permissões de que aquele precisa, os seus scripts de automatização permanecem seguros.</span><span class="sxs-lookup"><span data-stu-id="85022-115">By granting a service principal only the permissions it needs, your automation scripts stay secure.</span></span>

<span data-ttu-id="85022-116">Para saber como criar um principal de serviço para utilizar com o Azure PowerShell, veja [Criar um principal de serviço do Azure com o Azure PowerShell](create-azure-service-principal-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="85022-116">To learn how to create a service principal for use with Azure PowerShell, see [Create an Azure service principal with Azure PowerShell](create-azure-service-principal-azureps.md).</span></span>

<span data-ttu-id="85022-117">Para iniciar sessão com um principal de serviço, utilize o argumento `-ServicePrincipal` com o cmdlet `Connect-AzureRmAccount`.</span><span class="sxs-lookup"><span data-stu-id="85022-117">To sign in with a service principal, use the `-ServicePrincipal` argument with the `Connect-AzureRmAccount` cmdlet.</span></span> <span data-ttu-id="85022-118">Também vai precisar do ID de aplicação do principal de serviço, das credenciais de início de sessão e da associação do ID de inquilino ao principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="85022-118">You'll also need the service principal's application ID, sign-in credentials, and the tenant ID associate with the service principal.</span></span> <span data-ttu-id="85022-119">Para obter as credenciais do principal de serviço como o objeto adequado, utilize o cmdlet [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential).</span><span class="sxs-lookup"><span data-stu-id="85022-119">To get the service principal's credentials as the appropriate object, use the [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) cmdlet.</span></span> <span data-ttu-id="85022-120">Este cmdlet irá apresentar uma caixa de diálogo para introduzir o ID de utilizador e a palavra-passe do principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="85022-120">This cmdlet will display a dialog box to enter the service principal user ID and password into.</span></span>

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzureRmAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
```

## <a name="sign-in-using-an-azure-managed-service-identity"></a><span data-ttu-id="85022-121">Iniciar sessão com uma Identidade de Serviço Gerida do Azure</span><span class="sxs-lookup"><span data-stu-id="85022-121">Sign in using an Azure Managed Service Identity</span></span>

<span data-ttu-id="85022-122">As identidades geridas para os recursos do Azure são uma funcionalidade do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="85022-122">Managed identities for Azure resources is a feature of Azure Active Directory.</span></span> <span data-ttu-id="85022-123">Pode utilizar um principal de serviço da identidade gerida para início de sessão e adquirir um token de acesso só de aplicação para aceder a outros recursos.</span><span class="sxs-lookup"><span data-stu-id="85022-123">You can use a managed identity service principal for sign-in, and acquire an app-only access token to access other resources.</span></span> <span data-ttu-id="85022-124">As identidades geridas só estão disponíveis em máquinas virtuais em execução numa cloud do Azure.</span><span class="sxs-lookup"><span data-stu-id="85022-124">Managed identities are only available on virtual machines running in an Azure cloud.</span></span>

<span data-ttu-id="85022-125">Para obter mais informações sobre identidades geridas para recursos do Azure, veja [Como utilizar identidades geridas para recursos do Azure numa VM do Azure para adquirir um token de acesso](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).</span><span class="sxs-lookup"><span data-stu-id="85022-125">For more information about managed identities for Azure resources, see [How to use managed identities for Azure resources on an Azure VM to acquire an access token](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).</span></span>

## <a name="sign-in-to-another-cloud"></a><span data-ttu-id="85022-126">Iniciar sessão noutra Cloud</span><span class="sxs-lookup"><span data-stu-id="85022-126">Sign in to another Cloud</span></span>

<span data-ttu-id="85022-127">Os serviços cloud do Azure oferecem ambientes em conformidade com regulamentos de processamento de dados regionais.</span><span class="sxs-lookup"><span data-stu-id="85022-127">Azure cloud services offer environments compliant with regional data-handling regulations.</span></span>
<span data-ttu-id="85022-128">Para as contas numa cloud regional, defina o ambiente quando iniciar sessão com o argumento `-Environment`.</span><span class="sxs-lookup"><span data-stu-id="85022-128">For accounts in a regional cloud, set the environment when you sign in with the `-Environment` argument.</span></span>
<span data-ttu-id="85022-129">Por exemplo, se a sua conta está na cloud da China:</span><span class="sxs-lookup"><span data-stu-id="85022-129">For example, if your account is in the China cloud:</span></span>

```azurepowershell-interactive
Connect-AzureRmAccount -Environment AzureChinaCloud
```

<span data-ttu-id="85022-130">O comando seguinte obtém uma lista dos ambientes disponíveis:</span><span class="sxs-lookup"><span data-stu-id="85022-130">The following command gets a list of available environments:</span></span>

```azurepowershell-interactive
Get-AzureRmEnvironment | Select-Object Name
```

## <a name="learn-more-about-managing-azure-role-based-access"></a><span data-ttu-id="85022-131">Saiba mais sobre como gerir o acesso baseado em funções do Azure</span><span class="sxs-lookup"><span data-stu-id="85022-131">Learn more about managing Azure role-based access</span></span>

<span data-ttu-id="85022-132">Para obter mais informações sobre a gestão de autenticação e de subscrições do Azure, veja [Gerir Contas, Subscrições e Funções Administrativas](/azure/active-directory/role-based-access-control-configure).</span><span class="sxs-lookup"><span data-stu-id="85022-132">For more information about authentication and subscription management in Azure, see [Manage Accounts, Subscriptions, and Administrative Roles](/azure/active-directory/role-based-access-control-configure).</span></span>

<span data-ttu-id="85022-133">Cmdlets do Azure PowerShell para a gestão de funções:</span><span class="sxs-lookup"><span data-stu-id="85022-133">Azure PowerShell cmdlets for role management:</span></span>

* [<span data-ttu-id="85022-134">Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="85022-134">Get-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/Get-AzureRmRoleAssignment)
* [<span data-ttu-id="85022-135">Get-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="85022-135">Get-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Get-AzureRmRoleDefinition)
* [<span data-ttu-id="85022-136">New-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="85022-136">New-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/New-AzureRmRoleAssignment)
* [<span data-ttu-id="85022-137">New-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="85022-137">New-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/New-AzureRmRoleDefinition)
* [<span data-ttu-id="85022-138">Remove-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="85022-138">Remove-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleAssignment)
* [<span data-ttu-id="85022-139">Remove-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="85022-139">Remove-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleDefinition)
* [<span data-ttu-id="85022-140">Set-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="85022-140">Set-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Set-AzureRmRoleDefinition)
