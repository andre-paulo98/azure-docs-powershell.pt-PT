---
title: Iniciar sessão com o Azure PowerShell
description: Como iniciar sessão com o Azure PowerShell como um utilizador, principal de serviço ou com identidades geridas para recursos do Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/04/2019
ms.openlocfilehash: 614cce77deb4390ea158a48ae2d48b7b983224f2
ms.sourcegitcommit: 2d0c3ffaa5246f680784fa7e15b0d2536c27ff80
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/07/2020
ms.locfileid: "75720923"
---
# <a name="sign-in-with-azure-powershell"></a><span data-ttu-id="32c47-103">Iniciar sessão com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="32c47-103">Sign in with Azure PowerShell</span></span>

<span data-ttu-id="32c47-104">O Azure PowerShell suporta vários métodos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="32c47-104">Azure PowerShell supports several authentication methods.</span></span> <span data-ttu-id="32c47-105">O [Azure Cloud Shell](/azure/cloud-shell/overview) é a forma mais fácil de começar, uma vez que regista automaticamente o utilizador.</span><span class="sxs-lookup"><span data-stu-id="32c47-105">The easiest way to get started is with [Azure Cloud Shell](/azure/cloud-shell/overview), which automatically logs you in.</span></span> <span data-ttu-id="32c47-106">Com uma instalação local, pode iniciar sessão interativamente através do browser.</span><span class="sxs-lookup"><span data-stu-id="32c47-106">With a local install, you can sign in interactively through your browser.</span></span> <span data-ttu-id="32c47-107">Ao escrever scripts para automatização, a abordagem recomendada é utilizar um [principal de serviço](create-azure-service-principal-azureps.md) com as permissões necessárias.</span><span class="sxs-lookup"><span data-stu-id="32c47-107">When writing scripts for automation, the recommended approach is to use a [service principal](create-azure-service-principal-azureps.md) with the necessary permissions.</span></span> <span data-ttu-id="32c47-108">Ao restringir as permissões de início de sessão tanto quanto possível para o seu caso de utilização, ajuda a manter os recursos do Azure seguros.</span><span class="sxs-lookup"><span data-stu-id="32c47-108">When you restrict sign-in permissions as much as possible for your use case, you help keep your Azure resources secure.</span></span>

<span data-ttu-id="32c47-109">Depois de iniciar sessão, os comandos são executados na sua subscrição predefinida.</span><span class="sxs-lookup"><span data-stu-id="32c47-109">After signing in, commands are run against your default subscription.</span></span> <span data-ttu-id="32c47-110">Para alterar a subscrição ativa para uma sessão, utilize o cmdlet [Set-AzContext](/powershell/module/az.accounts/set-azcontext).</span><span class="sxs-lookup"><span data-stu-id="32c47-110">To change your active subscription for a session, use the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span> <span data-ttu-id="32c47-111">Para alterar a subscrição predefinida utilizada ao iniciar sessão com o Azure PowerShell, utilize [Set-AzDefault](/powershell/module/az.accounts/set-azdefault).</span><span class="sxs-lookup"><span data-stu-id="32c47-111">To change the default subscription used when logging in with Azure PowerShell, use [Set-AzDefault](/powershell/module/az.accounts/set-azdefault).</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="32c47-112">As suas credenciais são partilhadas entre várias sessões do PowerShell, desde que mantenha a sessão iniciada.</span><span class="sxs-lookup"><span data-stu-id="32c47-112">Your credentials are shared among multiple PowerShell sessions as long as you remain signed in.</span></span>
> <span data-ttu-id="32c47-113">Para obter mais informações, veja o artigo sobre [Credenciais Persistentes](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="32c47-113">For more information, see the article on [Persistent Credentials](context-persistence.md).</span></span>

## <a name="sign-in-interactively"></a><span data-ttu-id="32c47-114">Iniciar sessão interativamente</span><span class="sxs-lookup"><span data-stu-id="32c47-114">Sign in interactively</span></span>

<span data-ttu-id="32c47-115">Para iniciar sessão interativamente, utilize o cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).</span><span class="sxs-lookup"><span data-stu-id="32c47-115">To sign in interactively, use the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>

```azurepowershell-interactive
Connect-AzAccount
```

<span data-ttu-id="32c47-116">Quando é executado, este cmdlet apresenta uma cadeia de token.</span><span class="sxs-lookup"><span data-stu-id="32c47-116">When run, this cmdlet will present a token string.</span></span> <span data-ttu-id="32c47-117">Para iniciar sessão, copie esta cadeia e cole-a em https://microsoft.com/devicelogin num browser.</span><span class="sxs-lookup"><span data-stu-id="32c47-117">To sign in, copy this string and paste it into https://microsoft.com/devicelogin in a browser.</span></span> <span data-ttu-id="32c47-118">A sua sessão do PowerShell será autenticada para se ligar ao Azure.</span><span class="sxs-lookup"><span data-stu-id="32c47-118">Your PowerShell session will be authenticated to connect to Azure.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="32c47-119">A autorização de credenciais Nome de Utilizador/Palavra-passe foi removida no Azure PowerShell devido a alterações na implementação de autorizações do Active Directory e a preocupações relacionadas com segurança.</span><span class="sxs-lookup"><span data-stu-id="32c47-119">Username/password credential authorization has been removed in Azure PowerShell due to changes in Active Directory authorization implementations and security concerns.</span></span>
> <span data-ttu-id="32c47-120">Se utiliza a autorização de credenciais para fins de automatização, [crie um principal de serviço](create-azure-service-principal-azureps.md) como alternativa.</span><span class="sxs-lookup"><span data-stu-id="32c47-120">If you use credential authorization for automation purposes, instead [create a service principal](create-azure-service-principal-azureps.md).</span></span>

## <a name="sign-in-with-a-service-principal-a-namesp-signin"></a><span data-ttu-id="32c47-121">Iniciar sessão com um principal de serviço<a name="sp-signin"/></span><span class="sxs-lookup"><span data-stu-id="32c47-121">Sign in with a service principal <a name="sp-signin"/></span></span>

<span data-ttu-id="32c47-122">Os principais de serviço são contas não interativas do Azure.</span><span class="sxs-lookup"><span data-stu-id="32c47-122">Service principals are non-interactive Azure accounts.</span></span> <span data-ttu-id="32c47-123">Como outras contas de utilizador, as respetivas permissões são geridas com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="32c47-123">Like other user accounts, their permissions are managed with Azure Active Directory.</span></span> <span data-ttu-id="32c47-124">Ao conceder a um principal de serviço apenas as permissões de que aquele precisa, os seus scripts de automatização permanecem seguros.</span><span class="sxs-lookup"><span data-stu-id="32c47-124">By granting a service principal only the permissions it needs, your automation scripts stay secure.</span></span>

<span data-ttu-id="32c47-125">Para saber como criar um principal de serviço para utilizar com o Azure PowerShell, veja [Criar um principal de serviço do Azure com o Azure PowerShell](create-azure-service-principal-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="32c47-125">To learn how to create a service principal for use with Azure PowerShell, see [Create an Azure service principal with Azure PowerShell](create-azure-service-principal-azureps.md).</span></span>

<span data-ttu-id="32c47-126">Para iniciar sessão com um principal de serviço, utilize o argumento `-ServicePrincipal` com o cmdlet `Connect-AzAccount`.</span><span class="sxs-lookup"><span data-stu-id="32c47-126">To sign in with a service principal, use the `-ServicePrincipal` argument with the `Connect-AzAccount` cmdlet.</span></span> <span data-ttu-id="32c47-127">Também vai precisar do ID de aplicação do principal de serviço, das credenciais de início de sessão e da associação do ID de inquilino ao principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="32c47-127">You'll also need the service principal's application ID, sign-in credentials, and the tenant ID associate with the service principal.</span></span> <span data-ttu-id="32c47-128">A forma como inicia sessão com um principal de serviço irá depender do facto de este estar configurado para a autenticação baseada em palavra-passe ou baseada em certificado.</span><span class="sxs-lookup"><span data-stu-id="32c47-128">How you sign in with a service principal will depend on whether it's configured for password-based or certificate-based authentication.</span></span>

### <a name="password-based-authentication"></a><span data-ttu-id="32c47-129">Autenticação baseada em palavra-passe</span><span class="sxs-lookup"><span data-stu-id="32c47-129">Password-based authentication</span></span>

<span data-ttu-id="32c47-130">Para obter as credenciais do principal de serviço como o objeto adequado, utilize o cmdlet [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential).</span><span class="sxs-lookup"><span data-stu-id="32c47-130">To get the service principal's credentials as the appropriate object, use the [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) cmdlet.</span></span> <span data-ttu-id="32c47-131">Este cmdlet vai apresentar um pedido de nome de utilizador e palavra-passe.</span><span class="sxs-lookup"><span data-stu-id="32c47-131">This cmdlet will present a prompt for a username and password.</span></span> <span data-ttu-id="32c47-132">Utilize o ID do principal de serviço para o nome de utilizador.</span><span class="sxs-lookup"><span data-stu-id="32c47-132">Use the service principal ID for the username.</span></span>

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzAccount -ServicePrincipal -Credential $pscredential -Tenant $tenantId
```

<span data-ttu-id="32c47-133">Para cenários de automatização, tem de criar as credenciais a partir de um nome de utilizador e de uma cadeia segura:</span><span class="sxs-lookup"><span data-stu-id="32c47-133">For automation scenarios, you need to create credentials from a user name and secure string:</span></span>

```azurepowershell-interactive
$passwd = ConvertTo-SecureString <use a secure password here> -AsPlainText -Force
$pscredential = New-Object System.Management.Automation.PSCredential('service principal name/id', $passwd)
Connect-AzAccount -ServicePrincipal -Credential $pscredential -Tenant $tenantId
```

<span data-ttu-id="32c47-134">Certifique-se de que utiliza boas práticas de armazenamento de palavras-passe quando automatizar as ligações do principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="32c47-134">Make sure that you use good password storage practices when automating service principal connections.</span></span>

### <a name="certificate-based-authentication"></a><span data-ttu-id="32c47-135">Autenticação baseada em certificado</span><span class="sxs-lookup"><span data-stu-id="32c47-135">Certificate-based authentication</span></span>

<span data-ttu-id="32c47-136">A autenticação baseada em certificado precisa que o Azure PowerShell tenha a capacidade de obter informações de um arquivo de certificados local com base num thumbprint do certificado.</span><span class="sxs-lookup"><span data-stu-id="32c47-136">Certificate-based authentication requires that Azure PowerShell can retrieve information from a local certificate store based on a certificate thumbprint.</span></span>

```azurepowershell-interactive
Connect-AzAccount -ApplicationId $appId -Tenant $tenantId -CertificateThumbprint <thumbprint>
```

<span data-ttu-id="32c47-137">Ao utilizar um principal de serviço em vez de uma aplicação registada, adicione o argumento `-ServicePrincipal` e forneça o ID do principal de serviço como o valor do parâmetro `-ApplicationId`.</span><span class="sxs-lookup"><span data-stu-id="32c47-137">When using a service principal instead of a registered application, add the `-ServicePrincipal` argument and provide the service principal's ID as the `-ApplicationId` parameter's value.</span></span>

```azurepowershell-interactive
Connect-AzAccount -ServicePrincipal -ApplicationId $servicePrincipalId -Tenant $tenantId -CertificateThumbprint <thumbprint>
```

<span data-ttu-id="32c47-138">No PowerShell 5.1, o arquivo de certificados pode ser gerido e inspecionado com o módulo de [PKI](/powershell/module/pkiclient).</span><span class="sxs-lookup"><span data-stu-id="32c47-138">In PowerShell 5.1, the certificate store can be managed and inspected with the [PKI](/powershell/module/pkiclient) module.</span></span> <span data-ttu-id="32c47-139">No PowerShell Core 6.x e versões posteriores, o processo é mais complexo.</span><span class="sxs-lookup"><span data-stu-id="32c47-139">For PowerShell Core 6.x and later, the process is more complicated.</span></span> <span data-ttu-id="32c47-140">Os scripts que se seguem mostram como importar um certificado existente para o arquivo de certificados acessível ao PowerShell.</span><span class="sxs-lookup"><span data-stu-id="32c47-140">The following scripts show you how to import an existing certificate into the certificate store accessible by PowerShell.</span></span>

#### <a name="import-a-certificate-in-powershell-51"></a><span data-ttu-id="32c47-141">Importar um certificado no PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="32c47-141">Import a certificate in PowerShell 5.1</span></span>

```azurepowershell-interactive
# Import a PFX
$credentials = Get-Credential -Message "Provide PFX private key password"
Import-PfxCertificate -FilePath <path to certificate> -Password $credentials.Password -CertStoreLocation cert:\CurrentUser\My
```

#### <a name="import-a-certificate-in-powershell-core-6x-and-later"></a><span data-ttu-id="32c47-142">Importar um certificado no PowerShell Core 6.x e versões posteriores</span><span class="sxs-lookup"><span data-stu-id="32c47-142">Import a certificate in PowerShell Core 6.x and later</span></span>

```azurepowershell-interactive
# Import a PFX
$storeName = [System.Security.Cryptography.X509Certificates.StoreName]::My 
$storeLocation = [System.Security.Cryptography.X509Certificates.StoreLocation]::CurrentUser 
$store = [System.Security.Cryptography.X509Certificates.X509Store]::new($storeName, $storeLocation) 
$certPath = <path to certificate>
$credentials = Get-Credential -Message "Provide PFX private key password"
$flag = [System.Security.Cryptography.X509Certificates.X509KeyStorageFlags]::Exportable 
$certificate = [System.Security.Cryptography.X509Certificates.X509Certificate2]::new($certPath, $credentials.Password, $flag) 
$store.Open([System.Security.Cryptography.X509Certificates.OpenFlags]::ReadWrite) 
$store.Add($Certificate) 
$store.Close()
```

## <a name="sign-in-using-a-managed-identity"></a><span data-ttu-id="32c47-143">Iniciar sessão com uma identidade gerida</span><span class="sxs-lookup"><span data-stu-id="32c47-143">Sign in using a managed identity</span></span>

<span data-ttu-id="32c47-144">As identidades geridas são uma funcionalidade do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="32c47-144">Managed identities are a feature of Azure Active Directory.</span></span> <span data-ttu-id="32c47-145">As identidades geridas são principais de serviço atribuídos aos recursos que são executados no Azure.</span><span class="sxs-lookup"><span data-stu-id="32c47-145">Managed identities are service principals assigned to resources that run in Azure.</span></span> <span data-ttu-id="32c47-146">Pode utilizar um principal de serviço da identidade gerida para início de sessão e adquirir um token de acesso só de aplicação para aceder a outros recursos.</span><span class="sxs-lookup"><span data-stu-id="32c47-146">You can use a managed identity service principal for sign-in, and acquire an app-only access token to access other resources.</span></span> <span data-ttu-id="32c47-147">As identidades geridas só estão disponíveis em recursos em execução numa cloud do Azure.</span><span class="sxs-lookup"><span data-stu-id="32c47-147">Managed identities are only available on resources running in an Azure cloud.</span></span>

<span data-ttu-id="32c47-148">Este comando liga-se através da identidade gerida do ambiente anfitrião.</span><span class="sxs-lookup"><span data-stu-id="32c47-148">This command connects using the managed identity of the host environment.</span></span> <span data-ttu-id="32c47-149">Por exemplo, se for executado numa VirtualMachine com uma Identidade de Serviço Gerida atribuída, permite ao código iniciar sessão com essa identidade atribuída.</span><span class="sxs-lookup"><span data-stu-id="32c47-149">For example, if executed on a VirtualMachine with an assigned Managed Service Identity, this allows the code to sign in using that assigned identity.</span></span>

```azurepowershell-interactive
 Connect-AzAccount -Identity 
```

## <a name="sign-in-with-a-non-default-tenant-or-as-a-cloud-solution-provider-csp"></a><span data-ttu-id="32c47-150">Iniciar sessão com um inquilino não predefinido ou como um Fornecedor de Soluções Cloud (CSP)</span><span class="sxs-lookup"><span data-stu-id="32c47-150">Sign in with a non-default tenant or as a Cloud Solution Provider (CSP)</span></span>

<span data-ttu-id="32c47-151">Se a sua conta estiver associada a mais do que um inquilino, o início de sessão requer a utilização do parâmetro `-Tenant` durante a ligação.</span><span class="sxs-lookup"><span data-stu-id="32c47-151">If your account is associated with more than one tenant, sign-in requires the use of the `-Tenant` parameter when connecting.</span></span> <span data-ttu-id="32c47-152">Este parâmetro irá funcionar com qualquer método de início de sessão.</span><span class="sxs-lookup"><span data-stu-id="32c47-152">This parameter will work with any sign-in method.</span></span> <span data-ttu-id="32c47-153">Quando iniciar sessão, o valor deste parâmetro pode ser o ID de objeto do Azure do inquilino (ID de Inquilino) ou o nome de domínio completamente qualificado do inquilino.</span><span class="sxs-lookup"><span data-stu-id="32c47-153">When logging in, this parameter value can either be the Azure object ID of the tenant (Tenant ID) or the fully qualified domain name of the tenant.</span></span>

<span data-ttu-id="32c47-154">Se for um [Fornecedor de Soluções Cloud (CSP)](https://azure.microsoft.com/offers/ms-azr-0145p/), o valor `-Tenant`**tem** de ser um ID de inquilino.</span><span class="sxs-lookup"><span data-stu-id="32c47-154">If you're a [Cloud Solution Provider (CSP)](https://azure.microsoft.com/offers/ms-azr-0145p/), the `-Tenant` value **must** be a tenant ID.</span></span>

```azurepowershell-interactive
Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
```

## <a name="sign-in-to-another-cloud"></a><span data-ttu-id="32c47-155">Iniciar sessão noutra Cloud</span><span class="sxs-lookup"><span data-stu-id="32c47-155">Sign in to another Cloud</span></span>

<span data-ttu-id="32c47-156">Os serviços cloud do Azure oferecem ambientes em conformidade com as leis de processamento de dados regionais.</span><span class="sxs-lookup"><span data-stu-id="32c47-156">Azure cloud services offer environments compliant with regional data-handling laws.</span></span>
<span data-ttu-id="32c47-157">Para as contas numa cloud regional, defina o ambiente quando iniciar sessão com o argumento `-Environment`.</span><span class="sxs-lookup"><span data-stu-id="32c47-157">For accounts in a regional cloud, set the environment when you sign in with the `-Environment` argument.</span></span>
<span data-ttu-id="32c47-158">Este parâmetro irá funcionar com qualquer método de início de sessão.</span><span class="sxs-lookup"><span data-stu-id="32c47-158">This parameter will work with any sign-in method.</span></span> <span data-ttu-id="32c47-159">Por exemplo, se a sua conta está na cloud da China:</span><span class="sxs-lookup"><span data-stu-id="32c47-159">For example, if your account is in the China cloud:</span></span>

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

<span data-ttu-id="32c47-160">O comando seguinte obtém uma lista dos ambientes disponíveis:</span><span class="sxs-lookup"><span data-stu-id="32c47-160">The following command gets a list of available environments:</span></span>

```azurepowershell-interactive
Get-AzEnvironment | Select-Object Name
```
