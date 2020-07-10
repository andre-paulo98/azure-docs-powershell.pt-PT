---
title: Iniciar sessão com o Azure PowerShell
description: Como iniciar sessão com o Azure PowerShell como um utilizador, principal de serviço ou com identidades geridas para recursos do Azure.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 7/7/2020
ms.openlocfilehash: 7ac723202ca9e81c8ef4cba5e844d46b98ba4b67
ms.sourcegitcommit: 7b368a9be1cea2ac4e7d269e1a51529271269a42
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/08/2020
ms.locfileid: "86098785"
---
# <a name="sign-in-with-azure-powershell"></a><span data-ttu-id="524d7-103">Iniciar sessão com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="524d7-103">Sign in with Azure PowerShell</span></span>

<span data-ttu-id="524d7-104">O Azure PowerShell suporta vários métodos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="524d7-104">Azure PowerShell supports several authentication methods.</span></span> <span data-ttu-id="524d7-105">O [Azure Cloud Shell](/azure/cloud-shell/overview) é a forma mais fácil de começar, uma vez que regista automaticamente o utilizador.</span><span class="sxs-lookup"><span data-stu-id="524d7-105">The easiest way to get started is with [Azure Cloud Shell](/azure/cloud-shell/overview), which automatically logs you in.</span></span> <span data-ttu-id="524d7-106">Com uma instalação local, pode iniciar sessão interativamente através do browser.</span><span class="sxs-lookup"><span data-stu-id="524d7-106">With a local install, you can sign in interactively through your browser.</span></span> <span data-ttu-id="524d7-107">Ao escrever scripts para automatização, a abordagem recomendada é utilizar um [principal de serviço](create-azure-service-principal-azureps.md) com as permissões necessárias.</span><span class="sxs-lookup"><span data-stu-id="524d7-107">When writing scripts for automation, the recommended approach is to use a [service principal](create-azure-service-principal-azureps.md) with the necessary permissions.</span></span> <span data-ttu-id="524d7-108">Ao restringir as permissões de início de sessão tanto quanto possível para o seu caso de utilização, ajuda a manter os recursos do Azure seguros.</span><span class="sxs-lookup"><span data-stu-id="524d7-108">When you restrict sign-in permissions as much as possible for your use case, you help keep your Azure resources secure.</span></span>

<span data-ttu-id="524d7-109">Inicialmente, a sua sessão é iniciada na primeira subscrição que o Azure devolve se tiver acesso a mais do que uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="524d7-109">Initially, you're signed into the first subscription Azure returns if you have access to more than one subscription.</span></span> <span data-ttu-id="524d7-110">Os comandos são executados em relação a esta subscrição por predefinição.</span><span class="sxs-lookup"><span data-stu-id="524d7-110">Commands are run against this subscription by default.</span></span> <span data-ttu-id="524d7-111">Para alterar a subscrição ativa para uma sessão, utilize o cmdlet [Set-AzContext](/powershell/module/az.accounts/set-azcontext).</span><span class="sxs-lookup"><span data-stu-id="524d7-111">To change your active subscription for a session, use the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span> <span data-ttu-id="524d7-112">Para alterar a sua subscrição ativa e fazer com que esta persista entre sessões no mesmo sistema, utilize o cmdlet [Select-AzContext](/powershell/module/az.accounts/select-azcontext).</span><span class="sxs-lookup"><span data-stu-id="524d7-112">To change your active subscription and have it persist between sessions on the same system, use the [Select-AzContext](/powershell/module/az.accounts/select-azcontext) cmdlet.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="524d7-113">As suas credenciais são partilhadas entre várias sessões do PowerShell, desde que mantenha a sessão iniciada.</span><span class="sxs-lookup"><span data-stu-id="524d7-113">Your credentials are shared among multiple PowerShell sessions as long as you remain signed in.</span></span>
> <span data-ttu-id="524d7-114">Para obter mais informações, veja o artigo sobre [Credenciais Persistentes](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="524d7-114">For more information, see the article on [Persistent Credentials](context-persistence.md).</span></span>

## <a name="sign-in-interactively"></a><span data-ttu-id="524d7-115">Iniciar sessão interativamente</span><span class="sxs-lookup"><span data-stu-id="524d7-115">Sign in interactively</span></span>

<span data-ttu-id="524d7-116">Para iniciar sessão interativamente, utilize o cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).</span><span class="sxs-lookup"><span data-stu-id="524d7-116">To sign in interactively, use the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>

```azurepowershell-interactive
Connect-AzAccount
```

<span data-ttu-id="524d7-117">Quando é executado a partir da versão 6 e versões superiores do PowerShell, este cmdlet apresenta uma cadeia de token.</span><span class="sxs-lookup"><span data-stu-id="524d7-117">When run from PowerShell version 6 and higher, this cmdlet presents a token string.</span></span> <span data-ttu-id="524d7-118">Para iniciar sessão, copie esta cadeia e cole-a em [microsoft.com/devicelogin](https://microsoft.com/devicelogin) num browser.</span><span class="sxs-lookup"><span data-stu-id="524d7-118">To sign in, copy this string and paste it into [microsoft.com/devicelogin](https://microsoft.com/devicelogin) in a web browser.</span></span> <span data-ttu-id="524d7-119">A sua sessão do PowerShell será autenticada para se ligar ao Azure.</span><span class="sxs-lookup"><span data-stu-id="524d7-119">Your PowerShell session will be authenticated to connect to Azure.</span></span> <span data-ttu-id="524d7-120">Pode especificar o parâmetro `UseDeviceAuthentication` para receber uma cadeia de token no Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="524d7-120">You can specify the `UseDeviceAuthentication` parameter to receive a token string on Windows PowerShell.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="524d7-121">A autorização de credenciais Nome de Utilizador/Palavra-passe foi removida no Azure PowerShell devido a alterações na implementação de autorizações do Active Directory e a preocupações relacionadas com segurança.</span><span class="sxs-lookup"><span data-stu-id="524d7-121">Username/password credential authorization has been removed in Azure PowerShell due to changes in Active Directory authorization implementations and security concerns.</span></span> <span data-ttu-id="524d7-122">Se utiliza a autorização de credenciais para fins de automatização, [crie um principal de serviço](create-azure-service-principal-azureps.md) como alternativa.</span><span class="sxs-lookup"><span data-stu-id="524d7-122">If you use credential authorization for automation purposes, instead [create a service principal](create-azure-service-principal-azureps.md).</span></span>

<span data-ttu-id="524d7-123">Utilize o cmdlet [Get-AzContext](/powershell/module/az.accounts/get-azcontext) para armazenar o seu ID de inquilino numa variável que irá ser utilizada nas duas secções seguintes deste artigo.</span><span class="sxs-lookup"><span data-stu-id="524d7-123">Use the [Get-AzContext](/powershell/module/az.accounts/get-azcontext) cmdlet to store your tenant ID in a variable to be used in the next two sections of this article.</span></span>

```azurepowershell-interactive
$tenantId = (Get-AzContext).Tenant.Id
```

## <a name="sign-in-with-a-service-principal"></a><span data-ttu-id="524d7-124">Iniciar sessão com um principal de serviço<a name="sp-signin"/></span><span class="sxs-lookup"><span data-stu-id="524d7-124">Sign in with a service principal <a name="sp-signin"/></span></span>

<span data-ttu-id="524d7-125">Os principais de serviço são contas não interativas do Azure.</span><span class="sxs-lookup"><span data-stu-id="524d7-125">Service principals are non-interactive Azure accounts.</span></span> <span data-ttu-id="524d7-126">Como outras contas de utilizador, as respetivas permissões são geridas com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="524d7-126">Like other user accounts, their permissions are managed with Azure Active Directory.</span></span> <span data-ttu-id="524d7-127">Ao conceder a um principal de serviço apenas as permissões de que aquele precisa, os seus scripts de automatização permanecem seguros.</span><span class="sxs-lookup"><span data-stu-id="524d7-127">By granting a service principal only the permissions it needs, your automation scripts stay secure.</span></span>

<span data-ttu-id="524d7-128">Para saber como criar um principal de serviço para utilizar com o Azure PowerShell, veja [Criar um principal de serviço do Azure com o Azure PowerShell](create-azure-service-principal-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="524d7-128">To learn how to create a service principal for use with Azure PowerShell, see [Create an Azure service principal with Azure PowerShell](create-azure-service-principal-azureps.md).</span></span>

<span data-ttu-id="524d7-129">Para iniciar sessão com um principal de serviço, utilize o argumento `-ServicePrincipal` com o cmdlet `Connect-AzAccount`.</span><span class="sxs-lookup"><span data-stu-id="524d7-129">To sign in with a service principal, use the `-ServicePrincipal` argument with the `Connect-AzAccount` cmdlet.</span></span> <span data-ttu-id="524d7-130">Também vai precisar do ID de aplicação do principal de serviço, das credenciais de início de sessão e da associação do ID de inquilino ao principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="524d7-130">You'll also need the service principal's application ID, sign-in credentials, and the tenant ID associate with the service principal.</span></span> <span data-ttu-id="524d7-131">A forma como inicia sessão com um principal de serviço depende do facto de este estar configurado para a autenticação baseada em palavra-passe ou baseada em certificado.</span><span class="sxs-lookup"><span data-stu-id="524d7-131">How you sign in with a service principal depends on whether it's configured for password-based or certificate-based authentication.</span></span>

### <a name="password-based-authentication"></a><span data-ttu-id="524d7-132">Autenticação baseada em palavra-passe</span><span class="sxs-lookup"><span data-stu-id="524d7-132">Password-based authentication</span></span>

<span data-ttu-id="524d7-133">Crie um principal de serviço que irá ser utilizado nos exemplos desta secção.</span><span class="sxs-lookup"><span data-stu-id="524d7-133">Create a service principal to be used in the examples in this section.</span></span> <span data-ttu-id="524d7-134">Para mais informações sobre como criar principais de serviço, consulte [Criar um principal de serviço do Azure com o Azure PowerShell](/powershell/azure/create-azure-service-principal-azureps).</span><span class="sxs-lookup"><span data-stu-id="524d7-134">For more information on creating service principals, see [Create an Azure service principal with Azure PowerShell](/powershell/azure/create-azure-service-principal-azureps).</span></span>

```azurepowershell-interactive
$sp = New-AzADServicePrincipal -DisplayName ServicePrincipalName
```

<span data-ttu-id="524d7-135">Para obter as credenciais do principal de serviço como o objeto adequado, utilize o cmdlet [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential).</span><span class="sxs-lookup"><span data-stu-id="524d7-135">To get the service principal's credentials as the appropriate object, use the [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) cmdlet.</span></span> <span data-ttu-id="524d7-136">Este cmdlet apresenta um pedido de nome de utilizador e palavra-passe.</span><span class="sxs-lookup"><span data-stu-id="524d7-136">This cmdlet presents a prompt for a username and password.</span></span> <span data-ttu-id="524d7-137">Utilize o `applicationID` do principal de serviço para o nome de utilizador e converta o respetivo `secret` em texto simples para a palavra-passe.</span><span class="sxs-lookup"><span data-stu-id="524d7-137">Use the service principal's `applicationID` for the username and convert its `secret` to plain text for the password.</span></span>

```azurepowershell-interactive
# Retrieve the plain text password for use with `Get-Credential` in the next command.
$sp.secret | ConvertFrom-SecureString -AsPlainText

$pscredential = Get-Credential -UserName $sp.ApplicationId
Connect-AzAccount -ServicePrincipal -Credential $pscredential -Tenant $tenantId
```

<span data-ttu-id="524d7-138">Para cenários de automatização, tem de criar as credenciais a partir de um `applicationId` e um `secret` do principal de serviço:</span><span class="sxs-lookup"><span data-stu-id="524d7-138">For automation scenarios, you need to create credentials from a service principal's `applicationId` and `secret`:</span></span>

```azurepowershell-interactive
$pscredential = New-Object -TypeName System.Management.Automation.PSCredential($sp.ApplicationId, $sp.Secret)
Connect-AzAccount -ServicePrincipal -Credential $pscredential -Tenant $tenantId
```

<span data-ttu-id="524d7-139">Certifique-se de que utiliza boas práticas de armazenamento de palavras-passe quando automatizar as ligações do principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="524d7-139">Make sure that you use good password storage practices when automating service principal connections.</span></span>

### <a name="certificate-based-authentication"></a><span data-ttu-id="524d7-140">Autenticação baseada em certificado</span><span class="sxs-lookup"><span data-stu-id="524d7-140">Certificate-based authentication</span></span>

<span data-ttu-id="524d7-141">A autenticação baseada em certificado precisa que o Azure PowerShell tenha a capacidade de obter informações de um arquivo de certificados local com base num thumbprint do certificado.</span><span class="sxs-lookup"><span data-stu-id="524d7-141">Certificate-based authentication requires that Azure PowerShell can retrieve information from a local certificate store based on a certificate thumbprint.</span></span>

```azurepowershell-interactive
Connect-AzAccount -ApplicationId $appId -Tenant $tenantId -CertificateThumbprint <thumbprint>
```

<span data-ttu-id="524d7-142">Ao utilizar um principal de serviço em vez de uma aplicação registada, adicione o argumento `-ServicePrincipal` e forneça o ID da Aplicação do principal de serviço como o valor do parâmetro `-ApplicationId`.</span><span class="sxs-lookup"><span data-stu-id="524d7-142">When using a service principal instead of a registered application, add the `-ServicePrincipal` argument and provide the service principal's Application ID as the `-ApplicationId` parameter's value.</span></span>

```azurepowershell-interactive
Connect-AzAccount -ServicePrincipal -ApplicationId $servicePrincipalId -Tenant $tenantId -CertificateThumbprint <thumbprint>
```

<span data-ttu-id="524d7-143">No PowerShell 5.1, o arquivo de certificados pode ser gerido e inspecionado com o módulo de [PKI](/powershell/module/pkiclient).</span><span class="sxs-lookup"><span data-stu-id="524d7-143">In PowerShell 5.1, the certificate store can be managed and inspected with the [PKI](/powershell/module/pkiclient) module.</span></span> <span data-ttu-id="524d7-144">No PowerShell Core 6.x e versões posteriores, o processo é mais complexo.</span><span class="sxs-lookup"><span data-stu-id="524d7-144">For PowerShell Core 6.x and later, the process is more complicated.</span></span> <span data-ttu-id="524d7-145">Os scripts que se seguem mostram como importar um certificado existente para o arquivo de certificados acessível ao PowerShell.</span><span class="sxs-lookup"><span data-stu-id="524d7-145">The following scripts show you how to import an existing certificate into the certificate store accessible by PowerShell.</span></span>

#### <a name="import-a-certificate-in-powershell-51"></a><span data-ttu-id="524d7-146">Importar um certificado no PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="524d7-146">Import a certificate in PowerShell 5.1</span></span>

```azurepowershell-interactive
# Import a PFX
$credentials = Get-Credential -Message "Provide PFX private key password"
Import-PfxCertificate -FilePath <path to certificate> -Password $credentials.Password -CertStoreLocation cert:\CurrentUser\My
```

#### <a name="import-a-certificate-in-powershell-core-6x-and-later"></a><span data-ttu-id="524d7-147">Importar um certificado no PowerShell Core 6.x e versões posteriores</span><span class="sxs-lookup"><span data-stu-id="524d7-147">Import a certificate in PowerShell Core 6.x and later</span></span>

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

## <a name="sign-in-using-a-managed-identity"></a><span data-ttu-id="524d7-148">Iniciar sessão com uma identidade gerida</span><span class="sxs-lookup"><span data-stu-id="524d7-148">Sign in using a managed identity</span></span>

<span data-ttu-id="524d7-149">As identidades geridas são uma funcionalidade do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="524d7-149">Managed identities are a feature of Azure Active Directory.</span></span> <span data-ttu-id="524d7-150">As identidades geridas são principais de serviço atribuídos aos recursos que são executados no Azure.</span><span class="sxs-lookup"><span data-stu-id="524d7-150">Managed identities are service principals assigned to resources that run in Azure.</span></span> <span data-ttu-id="524d7-151">Pode utilizar um principal de serviço da identidade gerida para início de sessão e adquirir um token de acesso só de aplicação para aceder a outros recursos.</span><span class="sxs-lookup"><span data-stu-id="524d7-151">You can use a managed identity service principal for sign-in, and acquire an app-only access token to access other resources.</span></span> <span data-ttu-id="524d7-152">As identidades geridas só estão disponíveis em recursos em execução numa cloud do Azure.</span><span class="sxs-lookup"><span data-stu-id="524d7-152">Managed identities are only available on resources running in an Azure cloud.</span></span>

<span data-ttu-id="524d7-153">A ligação deste exemplo é estabelecida através da identidade gerida do ambiente anfitrião.</span><span class="sxs-lookup"><span data-stu-id="524d7-153">This example connects using the managed identity of the host environment.</span></span> <span data-ttu-id="524d7-154">Por exemplo, se for executado numa VirtualMachine com uma Identidade de Serviço Gerida atribuída, permite ao código iniciar sessão com essa identidade atribuída.</span><span class="sxs-lookup"><span data-stu-id="524d7-154">For example, if executed on a VirtualMachine with an assigned Managed Service Identity, this allows the code to sign in using that assigned identity.</span></span>

```azurepowershell-interactive
 Connect-AzAccount -Identity
```

## <a name="sign-in-with-a-non-default-tenant-or-as-a-cloud-solution-provider-csp"></a><span data-ttu-id="524d7-155">Iniciar sessão com um inquilino não predefinido ou como um Fornecedor de Soluções Cloud (CSP)</span><span class="sxs-lookup"><span data-stu-id="524d7-155">Sign in with a non-default tenant or as a Cloud Solution Provider (CSP)</span></span>

<span data-ttu-id="524d7-156">Se a sua conta estiver associada a mais do que um inquilino, o início de sessão requer a especificação do parâmetro `-Tenant` durante a ligação.</span><span class="sxs-lookup"><span data-stu-id="524d7-156">If your account is associated with more than one tenant, sign-in requires the `-Tenant` parameter to be specified when connecting.</span></span> <span data-ttu-id="524d7-157">Este parâmetro funciona com qualquer método de início de sessão.</span><span class="sxs-lookup"><span data-stu-id="524d7-157">This parameter works with any sign-in method.</span></span> <span data-ttu-id="524d7-158">Quando iniciar sessão, o valor deste parâmetro pode ser o ID de objeto do Azure do inquilino (ID de Inquilino) ou o nome de domínio completamente qualificado do inquilino.</span><span class="sxs-lookup"><span data-stu-id="524d7-158">When logging in, this parameter value can either be the Azure object ID of the tenant (Tenant ID) or the fully qualified domain name of the tenant.</span></span>

<span data-ttu-id="524d7-159">Se for um [Fornecedor de Soluções Cloud (CSP)](https://azure.microsoft.com/offers/ms-azr-0145p/), o valor `-Tenant`**tem** de ser um ID de inquilino.</span><span class="sxs-lookup"><span data-stu-id="524d7-159">If you're a [Cloud Solution Provider (CSP)](https://azure.microsoft.com/offers/ms-azr-0145p/), the `-Tenant` value **must** be a tenant ID.</span></span>

```azurepowershell-interactive
Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
```

## <a name="sign-in-to-another-cloud"></a><span data-ttu-id="524d7-160">Iniciar sessão noutra Cloud</span><span class="sxs-lookup"><span data-stu-id="524d7-160">Sign in to another Cloud</span></span>

<span data-ttu-id="524d7-161">Os serviços cloud do Azure oferecem ambientes em conformidade com as leis de processamento de dados regionais.</span><span class="sxs-lookup"><span data-stu-id="524d7-161">Azure cloud services offer environments compliant with regional data-handling laws.</span></span> <span data-ttu-id="524d7-162">Para as contas numa cloud regional, defina o ambiente quando iniciar sessão com o argumento `-Environment`.</span><span class="sxs-lookup"><span data-stu-id="524d7-162">For accounts in a regional cloud, set the environment when you sign in with the `-Environment` argument.</span></span> <span data-ttu-id="524d7-163">Este parâmetro funciona com qualquer método de início de sessão.</span><span class="sxs-lookup"><span data-stu-id="524d7-163">This parameter works with any sign-in method.</span></span> <span data-ttu-id="524d7-164">Por exemplo, se a sua conta está na cloud da China:</span><span class="sxs-lookup"><span data-stu-id="524d7-164">For example, if your account is in the China cloud:</span></span>

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

<span data-ttu-id="524d7-165">O comando seguinte obtém uma lista dos ambientes disponíveis:</span><span class="sxs-lookup"><span data-stu-id="524d7-165">The following command gets a list of available environments:</span></span>

```azurepowershell-interactive
Get-AzEnvironment | Select-Object -Property Name
```
