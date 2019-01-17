---
title: Iniciar sessão com o Azure PowerShell
description: Como iniciar sessão com o Azure PowerShell como um utilizador, principal de serviço ou com identidades geridas para recursos do Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/29/2018
ms.openlocfilehash: 80c59a10666c6e3a01e6c33716fce40094fb14be
ms.sourcegitcommit: c6fd0e490fa0e33b8b768b679682a47d8faae1cf
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/16/2019
ms.locfileid: "54342202"
---
# <a name="sign-in-with-azure-powershell"></a><span data-ttu-id="2e446-103">Iniciar sessão com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="2e446-103">Sign in with Azure PowerShell</span></span>

<span data-ttu-id="2e446-104">O Azure PowerShell suporta vários métodos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="2e446-104">Azure PowerShell supports several authentication methods.</span></span> <span data-ttu-id="2e446-105">O [Azure Cloud Shell](/azure/cloud-shell/overview) é a forma mais fácil de começar, uma vez que regista automaticamente o utilizador.</span><span class="sxs-lookup"><span data-stu-id="2e446-105">The easiest way to get started is with [Azure Cloud Shell](/azure/cloud-shell/overview), which automatically logs you in.</span></span> <span data-ttu-id="2e446-106">Com uma instalação local, pode iniciar sessão interativamente através do browser.</span><span class="sxs-lookup"><span data-stu-id="2e446-106">With a local install, you can sign in interactively through your browser.</span></span> <span data-ttu-id="2e446-107">Ao escrever scripts para automatização, a abordagem recomendada é utilizar um [principal de serviço](create-azure-service-principal-azureps.md) com as permissões necessárias.</span><span class="sxs-lookup"><span data-stu-id="2e446-107">When writing scripts for automation, the recommended approach is to use a [service principal](create-azure-service-principal-azureps.md) with the necessary permissions.</span></span> <span data-ttu-id="2e446-108">Ao restringir as permissões de início de sessão tanto quanto possível para o seu caso de utilização, ajuda a manter os recursos do Azure seguros.</span><span class="sxs-lookup"><span data-stu-id="2e446-108">When you restrict sign-in permissions as much as possible for your use case, you help keep your Azure resources secure.</span></span>

<span data-ttu-id="2e446-109">Depois de iniciar sessão, os comandos são executados na sua subscrição predefinida.</span><span class="sxs-lookup"><span data-stu-id="2e446-109">After signing in, commands are run against your default subscription.</span></span> <span data-ttu-id="2e446-110">Para alterar a subscrição ativa para uma sessão, utilize o cmdlet [Set-AzContext](/powershell/module/az.accounts/set-azcontext).</span><span class="sxs-lookup"><span data-stu-id="2e446-110">To change your active subscription for a session, use the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span> <span data-ttu-id="2e446-111">Para alterar a subscrição predefinida utilizada ao iniciar sessão com o Azure PowerShell, utilize [Set-AzDefault](/powershell/module/az.accounts/set-azdefault).</span><span class="sxs-lookup"><span data-stu-id="2e446-111">To change the default subscription used when logging in with Azure PowerShell, use [Set-AzDefault](/powershell/module/az.accounts/set-azdefault).</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="2e446-112">As suas credenciais são partilhadas entre várias sessões do PowerShell, desde que mantenha a sessão iniciada.</span><span class="sxs-lookup"><span data-stu-id="2e446-112">Your credentials are shared among multiple PowerShell sessions as long as you remain signed in.</span></span>
> <span data-ttu-id="2e446-113">Para obter mais informações, veja o artigo sobre [Credenciais Persistentes](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="2e446-113">For more information, see the article on [Persistent Credentials](context-persistence.md).</span></span>

## <a name="sign-in-interactively"></a><span data-ttu-id="2e446-114">Iniciar sessão interativamente</span><span class="sxs-lookup"><span data-stu-id="2e446-114">Sign in interactively</span></span>

<span data-ttu-id="2e446-115">Para iniciar sessão interativamente, utilize o cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).</span><span class="sxs-lookup"><span data-stu-id="2e446-115">To sign in interactively, use the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>

```azurepowershell-interactive
Connect-AzAccount
```

<span data-ttu-id="2e446-116">Quando é executado, este cmdlet apresenta uma cadeia de token.</span><span class="sxs-lookup"><span data-stu-id="2e446-116">When run, this cmdlet will present a token string.</span></span> <span data-ttu-id="2e446-117">Para iniciar sessão, copie esta cadeia e cole-a em https://microsoft.com/devicelogin num browser.</span><span class="sxs-lookup"><span data-stu-id="2e446-117">To sign in, copy this string and paste it into https://microsoft.com/devicelogin in a browser.</span></span> <span data-ttu-id="2e446-118">A sua sessão do PowerShell será autenticada para se ligar ao Azure.</span><span class="sxs-lookup"><span data-stu-id="2e446-118">Your PowerShell session will be authenticated to connect to Azure.</span></span>

## <a name="sign-in-with-credentials"></a><span data-ttu-id="2e446-119">Iniciar sessão com credenciais</span><span class="sxs-lookup"><span data-stu-id="2e446-119">Sign in with credentials</span></span>

<span data-ttu-id="2e446-120">Também pode iniciar sessão com um objeto `PSCredential` autorizado para ligar ao Azure.</span><span class="sxs-lookup"><span data-stu-id="2e446-120">You can also sign in with a `PSCredential` object authorized to connect to Azure.</span></span>
<span data-ttu-id="2e446-121">A maneira mais fácil de obter um objeto de credencial é com o cmdlet [Get-Credential](/powershell/module/Microsoft.PowerShell.Security/Get-Credential).</span><span class="sxs-lookup"><span data-stu-id="2e446-121">The easiest way to get a credential object is with the [Get-Credential](/powershell/module/Microsoft.PowerShell.Security/Get-Credential) cmdlet.</span></span> <span data-ttu-id="2e446-122">Quando é executado, este cmdlet vai solicitar-lhe um par de credenciais nome de utilizador/palavra-passe.</span><span class="sxs-lookup"><span data-stu-id="2e446-122">When run, this cmdlet will prompt you for a username/password credential pair.</span></span>

> [!Note]
> <span data-ttu-id="2e446-123">Esta abordagem não funciona em contas Microsoft nem em contas que tenham a autenticação multifator ativada.</span><span class="sxs-lookup"><span data-stu-id="2e446-123">This approach doesn't work with Microsoft accounts or accounts that have two-factor authentication enabled.</span></span>

```azurepowershell-interactive
$creds = Get-Credential
Connect-AzAccount -Credential $creds
```

## <a name="sign-in-with-a-service-principal"></a><span data-ttu-id="2e446-124">Iniciar sessão com um principal de serviço</span><span class="sxs-lookup"><span data-stu-id="2e446-124">Sign in with a service principal</span></span>

<span data-ttu-id="2e446-125">Os principais de serviço são contas não interativas do Azure.</span><span class="sxs-lookup"><span data-stu-id="2e446-125">Service principals are non-interactive Azure accounts.</span></span> <span data-ttu-id="2e446-126">Como outras contas de utilizador, as respetivas permissões são geridas com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2e446-126">Like other user accounts, their permissions are managed with Azure Active Directory.</span></span> <span data-ttu-id="2e446-127">Ao conceder a um principal de serviço apenas as permissões de que aquele precisa, os seus scripts de automatização permanecem seguros.</span><span class="sxs-lookup"><span data-stu-id="2e446-127">By granting a service principal only the permissions it needs, your automation scripts stay secure.</span></span>

<span data-ttu-id="2e446-128">Para saber como criar um principal de serviço para utilizar com o Azure PowerShell, veja [Criar um principal de serviço do Azure com o Azure PowerShell](create-azure-service-principal-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="2e446-128">To learn how to create a service principal for use with Azure PowerShell, see [Create an Azure service principal with Azure PowerShell](create-azure-service-principal-azureps.md).</span></span>

<span data-ttu-id="2e446-129">Para iniciar sessão com um principal de serviço, utilize o argumento `-ServicePrincipal` com o cmdlet `Connect-AzAccount`.</span><span class="sxs-lookup"><span data-stu-id="2e446-129">To sign in with a service principal, use the `-ServicePrincipal` argument with the `Connect-AzAccount` cmdlet.</span></span> <span data-ttu-id="2e446-130">Também vai precisar do ID de aplicação do principal de serviço, das credenciais de início de sessão e da associação do ID de inquilino ao principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="2e446-130">You'll also need the service principal's application ID, sign-in credentials, and the tenant ID associate with the service principal.</span></span> <span data-ttu-id="2e446-131">Para obter as credenciais do principal de serviço como o objeto adequado, utilize o cmdlet [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential).</span><span class="sxs-lookup"><span data-stu-id="2e446-131">To get the service principal's credentials as the appropriate object, use the [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) cmdlet.</span></span> <span data-ttu-id="2e446-132">Este cmdlet vai apresentar uma linha de comandos para o ID e a palavra-passe de utilizador do principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="2e446-132">This cmdlet will present a prompt for the service principal user ID and password.</span></span>

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
```

## <a name="sign-in-using-a-managed-identity"></a><span data-ttu-id="2e446-133">Iniciar sessão com uma identidade gerida</span><span class="sxs-lookup"><span data-stu-id="2e446-133">Sign in using a managed identity</span></span> 

<span data-ttu-id="2e446-134">As identidades geridas são uma funcionalidade do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2e446-134">Managed identities are a feature of Azure Active Directory.</span></span> <span data-ttu-id="2e446-135">As identidades geridas são principais de serviço atribuídos aos recursos que são executados no Azure.</span><span class="sxs-lookup"><span data-stu-id="2e446-135">Managed identities are service principals assigned to resources that run in Azure.</span></span> <span data-ttu-id="2e446-136">Pode utilizar um principal de serviço da identidade gerida para início de sessão e adquirir um token de acesso só de aplicação para aceder a outros recursos.</span><span class="sxs-lookup"><span data-stu-id="2e446-136">You can use a managed identity service principal for sign-in, and acquire an app-only access token to access other resources.</span></span> <span data-ttu-id="2e446-137">As identidades geridas só estão disponíveis em recursos em execução numa cloud do Azure.</span><span class="sxs-lookup"><span data-stu-id="2e446-137">Managed identities are only available on resources running in an Azure cloud.</span></span>

<span data-ttu-id="2e446-138">Para saber mais sobre identidades geridas para recursos do Azure, veja [Como utilizar identidades geridas para recursos do Azure numa VM do Azure para adquirir um token de acesso](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).</span><span class="sxs-lookup"><span data-stu-id="2e446-138">To learn more about managed identities for Azure resources, see [How to use managed identities for Azure resources on an Azure VM to acquire an access token](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).</span></span>

## <a name="sign-in-with-a-non-default-tenant-or-as-a-cloud-solution-provider-csp"></a><span data-ttu-id="2e446-139">Iniciar sessão com um inquilino não predefinido ou como um Fornecedor de Soluções Cloud (CSP)</span><span class="sxs-lookup"><span data-stu-id="2e446-139">Sign in with a non-default tenant or as a Cloud Solution Provider (CSP)</span></span>

<span data-ttu-id="2e446-140">Se a sua conta estiver associada a mais do que um inquilino, o início de sessão requer a utilização do parâmetro `-TenantId` durante a ligação.</span><span class="sxs-lookup"><span data-stu-id="2e446-140">If your account is associated with more than one tenant, sign-in requires the use of the `-TenantId` parameter when connecting.</span></span> <span data-ttu-id="2e446-141">Este parâmetro irá funcionar com qualquer outro método de início de sessão.</span><span class="sxs-lookup"><span data-stu-id="2e446-141">This parameter will work with any other sign-in method.</span></span> <span data-ttu-id="2e446-142">Quando iniciar sessão, o valor deste parâmetro pode ser o ID de objeto do Azure do inquilino (ID de Inquilino) ou o nome de domínio completamente qualificado do inquilino.</span><span class="sxs-lookup"><span data-stu-id="2e446-142">When logging in, this parameter value can either be the Azure object ID of the tenant (Tenant ID) or the fully qualified domain name of the tenant.</span></span>

<span data-ttu-id="2e446-143">Se for um [Fornecedor de Soluções Cloud (CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/), o valor `-TenantId` **tem** de ser um ID de inquilino.</span><span class="sxs-lookup"><span data-stu-id="2e446-143">If you're a [Cloud Solution Provider (CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/), the `-TenantId` value **must** be a tenant ID.</span></span>

```azurepowershell-interactive
Connect-AzAccount -TenantId 'xxxx-xxxx-xxxx-xxxx'
```

## <a name="sign-in-to-another-cloud"></a><span data-ttu-id="2e446-144">Iniciar sessão noutra Cloud</span><span class="sxs-lookup"><span data-stu-id="2e446-144">Sign in to another Cloud</span></span>

<span data-ttu-id="2e446-145">Os serviços cloud do Azure oferecem ambientes em conformidade com as leis de processamento de dados regionais.</span><span class="sxs-lookup"><span data-stu-id="2e446-145">Azure cloud services offer environments compliant with regional data-handling laws.</span></span>
<span data-ttu-id="2e446-146">Para as contas numa cloud regional, defina o ambiente quando iniciar sessão com o argumento `-Environment`.</span><span class="sxs-lookup"><span data-stu-id="2e446-146">For accounts in a regional cloud, set the environment when you sign in with the `-Environment` argument.</span></span>
<span data-ttu-id="2e446-147">Por exemplo, se a sua conta está na cloud da China:</span><span class="sxs-lookup"><span data-stu-id="2e446-147">For example, if your account is in the China cloud:</span></span>

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

<span data-ttu-id="2e446-148">O comando seguinte obtém uma lista dos ambientes disponíveis:</span><span class="sxs-lookup"><span data-stu-id="2e446-148">The following command gets a list of available environments:</span></span>

```azurepowershell-interactive
Get-AzEnvironment | Select-Object Name
```