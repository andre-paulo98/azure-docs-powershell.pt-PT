---
title: Utilizar principais de serviço do Azure com o Azure PowerShell
description: Saiba como criar e utilizar principais de serviço com o Azure PowerShell.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 04/23/2019
ms.openlocfilehash: 4c47d2bac2c63f13ac0ebbccda3e2eed12cd658f
ms.sourcegitcommit: a321ef9d134c684fa24ababcbd898f86b00d9364
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/20/2020
ms.locfileid: "77477785"
---
# <a name="create-an-azure-service-principal-with-azure-powershell"></a><span data-ttu-id="70347-103">Criar um principal de serviço do Azure com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="70347-103">Create an Azure service principal with Azure PowerShell</span></span>

<span data-ttu-id="70347-104">As ferramentas automatizadas que utilizam serviços do Azure devem ter sempre permissões restritas.</span><span class="sxs-lookup"><span data-stu-id="70347-104">Automated tools that use Azure services should always have restricted permissions.</span></span> <span data-ttu-id="70347-105">Em vez de obrigar as aplicações a iniciarem sessão como um utilizador com privilégios máximos, o Azure disponibiliza principais de serviço.</span><span class="sxs-lookup"><span data-stu-id="70347-105">Instead of having applications sign in as a fully privileged user, Azure offers service principals.</span></span>

<span data-ttu-id="70347-106">Um principal de serviço do Azure é uma identidade criada para ser utilizada com aplicações, serviços alojados e ferramentas automatizadas para aceder aos recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="70347-106">An Azure service principal is an identity created for use with applications, hosted services, and automated tools to access Azure resources.</span></span> <span data-ttu-id="70347-107">Este acesso é restringido pelas funções atribuídas ao principal de serviço, o que lhe permite assumir o controlo dos recursos que podem ser acedidos e em que nível.</span><span class="sxs-lookup"><span data-stu-id="70347-107">This access is restricted by the roles assigned to the service principal, giving you control over which resources can be accessed and at which level.</span></span> <span data-ttu-id="70347-108">Por motivos de segurança, é sempre recomendado utilizar os principais de serviço com ferramentas automatizadas, em vez de permitir que iniciem sessão com uma identidade de utilizador.</span><span class="sxs-lookup"><span data-stu-id="70347-108">For security reasons, it's always recommended to use service principals with automated tools rather than allowing them to log in with a user identity.</span></span>

<span data-ttu-id="70347-109">Este artigo mostra-lhe os passos para criar, obter informações e repor um principal de serviço com o Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="70347-109">This article shows you the steps for creating, getting information about, and resetting a service principal with Azure PowerShell.</span></span>

## <a name="create-a-service-principal"></a><span data-ttu-id="70347-110">Criar um principal de serviço</span><span class="sxs-lookup"><span data-stu-id="70347-110">Create a service principal</span></span>

<span data-ttu-id="70347-111">Crie um principal de serviço com o cmdlet [New-AzADServicePrincipal](/powershell/module/Az.Resources/New-AzADServicePrincipal).</span><span class="sxs-lookup"><span data-stu-id="70347-111">Create a service principal with the [New-AzADServicePrincipal](/powershell/module/Az.Resources/New-AzADServicePrincipal) cmdlet.</span></span> <span data-ttu-id="70347-112">Quando cria um principal de serviço, escolhe o tipo de autenticação de início de sessão que o mesmo utiliza.</span><span class="sxs-lookup"><span data-stu-id="70347-112">When creating a service principal, you choose the type of sign-in authentication it uses.</span></span>

> [!NOTE]
>
> <span data-ttu-id="70347-113">Se a sua conta não tiver permissão para criar um principal de serviço, o cmdlet `New-AzADServicePrincipal` devolve uma mensagem de erro com a indicação "Privilégios insuficientes para concluir a operação".</span><span class="sxs-lookup"><span data-stu-id="70347-113">If your account doesn't have permission to create a service principal, `New-AzADServicePrincipal` will return an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="70347-114">Contacte o seu administrador do Azure Active Directory para criar um principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="70347-114">Contact your Azure Active Directory admin to create a service principal.</span></span>

<span data-ttu-id="70347-115">Existem dois tipos de autenticação disponíveis para os principais de serviço: a autenticação baseada em palavra-passe e a autenticação baseada em certificado.</span><span class="sxs-lookup"><span data-stu-id="70347-115">There are two types of authentication available for service principals: Password-based authentication, and certificate-based authentication.</span></span>

### <a name="password-based-authentication"></a><span data-ttu-id="70347-116">Autenticação baseada em palavra-passe</span><span class="sxs-lookup"><span data-stu-id="70347-116">Password-based authentication</span></span>

<span data-ttu-id="70347-117">Na ausência de outros parâmetros de autenticação, a autenticação baseada em palavra-passe é utilizada e é criada uma palavra-passe aleatória para si.</span><span class="sxs-lookup"><span data-stu-id="70347-117">Without any other authentication parameters, password-based authentication is used and a random password created for you.</span></span> <span data-ttu-id="70347-118">Se estiver interessado na autenticação baseada em palavra-passe, este é o método recomendado.</span><span class="sxs-lookup"><span data-stu-id="70347-118">If you want password-based authentication, this method is recommended.</span></span>

```azurepowershell-interactive
$sp = New-AzADServicePrincipal -DisplayName ServicePrincipalName
```

<span data-ttu-id="70347-119">O objeto devolvido contém o membro `Secret`, ou seja, uma `SecureString` que contém a palavra-passe gerada.</span><span class="sxs-lookup"><span data-stu-id="70347-119">The returned object contains the `Secret` member, which is a `SecureString` containing the generated password.</span></span> <span data-ttu-id="70347-120">Certifique-se de que armazena este valor num local seguro para efetuar a autenticação com o principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="70347-120">Make sure that you store this value somewhere secure to authenticate with the service principal.</span></span> <span data-ttu-id="70347-121">O respetivo valor __não será__ apresentado na saída da consola.</span><span class="sxs-lookup"><span data-stu-id="70347-121">Its value __won't__ be displayed in the console output.</span></span> <span data-ttu-id="70347-122">Se perder a palavra-passe, [reponha as credenciais do principal de serviço](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="70347-122">If you lose the password, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="70347-123">O código seguinte permitirá exportar o segredo:</span><span class="sxs-lookup"><span data-stu-id="70347-123">The following code will allow you to export the secret:</span></span>

```azurepowershell-interactive
$BSTR = [System.Runtime.InteropServices.Marshal]::SecureStringToBSTR($sp.Secret)
$UnsecureSecret = [System.Runtime.InteropServices.Marshal]::PtrToStringAuto($BSTR)
```

<span data-ttu-id="70347-124">Para as palavras-passe fornecidas pelo utilizador, o argumento `-PasswordCredential` aceita objetos `Microsoft.Azure.Commands.ActiveDirectory.PSADPasswordCredential`.</span><span class="sxs-lookup"><span data-stu-id="70347-124">For user-supplied passwords, the `-PasswordCredential` argument takes `Microsoft.Azure.Commands.ActiveDirectory.PSADPasswordCredential` objects.</span></span> <span data-ttu-id="70347-125">Estes objetos têm de ter uma `StartDate` e uma `EndDate` válidas, bem como aceitar uma `Password` com texto desencriptado.</span><span class="sxs-lookup"><span data-stu-id="70347-125">These objects must have a valid `StartDate` and `EndDate`, and take a plaintext `Password`.</span></span> <span data-ttu-id="70347-126">Quando criar uma palavra-passe, certifique-se de que segue as [regras e restrições de palavra-passe do Azure Active Directory](/azure/active-directory/active-directory-passwords-policy).</span><span class="sxs-lookup"><span data-stu-id="70347-126">When creating a password, make sure you follow the [Azure Active Directory password rules and restrictions](/azure/active-directory/active-directory-passwords-policy).</span></span> <span data-ttu-id="70347-127">Não utilize uma palavra-passe fraca nem reutilize uma palavra-passe.</span><span class="sxs-lookup"><span data-stu-id="70347-127">Don't use a weak password or reuse a password.</span></span>

```azurepowershell-interactive
Import-Module Az.Resources # Imports the PSADPasswordCredential object
$credentials = New-Object Microsoft.Azure.Commands.ActiveDirectory.PSADPasswordCredential -Property @{ StartDate=Get-Date; EndDate=Get-Date -Year 2024; Password=<Choose a strong password>}
$sp = New-AzAdServicePrincipal -DisplayName ServicePrincipalName -PasswordCredential $credentials
```

<span data-ttu-id="70347-128">O objeto devolvido a partir de `New-AzADServicePrincipal` contém os membros `Id` e `DisplayName`, que podem ser utilizados para iniciar sessão com o principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="70347-128">The object returned from `New-AzADServicePrincipal` contains the `Id` and `DisplayName` members, either of which can be used for sign in with the service principal.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="70347-129">Iniciar sessão com um principal de serviço necessita do ID de inquilino no qual o principal de serviço foi criado.</span><span class="sxs-lookup"><span data-stu-id="70347-129">Signing in with a service principal requires the tenant ID which the service principal was created under.</span></span> <span data-ttu-id="70347-130">Para obter o inquilino que estava ativo quando o principal de serviço foi criado, execute o seguinte comando __imediatamente após__ a criação do principal de serviço:</span><span class="sxs-lookup"><span data-stu-id="70347-130">To get the active tenant when the service principal was created, run the following command __immediately after__ service principal creation:</span></span>
>
> ```azurepowershell-interactive
> (Get-AzContext).Tenant.Id
> ```

### <a name="certificate-based-authentication"></a><span data-ttu-id="70347-131">Autenticação baseada em certificado</span><span class="sxs-lookup"><span data-stu-id="70347-131">Certificate-based authentication</span></span>

<span data-ttu-id="70347-132">Os principais de serviço que utilizam a autenticação baseada em certificado são criados com o parâmetro `-CertValue`.</span><span class="sxs-lookup"><span data-stu-id="70347-132">Service principals using certificate-based authentication are created with the `-CertValue` parameter.</span></span> <span data-ttu-id="70347-133">Este parâmetro aceita uma cadeia ASCII codificada em base64 do certificado público.</span><span class="sxs-lookup"><span data-stu-id="70347-133">This parameter takes a base64-encoded ASCII string of the public certificate.</span></span> <span data-ttu-id="70347-134">Isto é representado por um ficheiro PEM, ou por um CRT ou CER codificado em texto.</span><span class="sxs-lookup"><span data-stu-id="70347-134">This is represented by a PEM file, or a text-encoded CRT or CER.</span></span> <span data-ttu-id="70347-135">Não são suportadas codificações binárias do certificado público.</span><span class="sxs-lookup"><span data-stu-id="70347-135">Binary encodings of the public certificate aren't supported.</span></span> <span data-ttu-id="70347-136">Estas instruções partem do princípio de que já tem um certificado disponível.</span><span class="sxs-lookup"><span data-stu-id="70347-136">These instructions assume that you already have a certificate available.</span></span>

```azurepowershell-interactive
$cert = <public certificate as base64-encoded string>
$sp = New-AzADServicePrincipal -DisplayName ServicePrincipalName -CertValue $cert
```

<span data-ttu-id="70347-137">Também pode utilizar o parâmetro `-KeyCredential`, que aceita objetos `PSADKeyCredential`.</span><span class="sxs-lookup"><span data-stu-id="70347-137">You can also use the `-KeyCredential` parameter, which takes `PSADKeyCredential` objects.</span></span> <span data-ttu-id="70347-138">Estes objetos têm de ter uma `StartDate` e uma `EndDate` válidas, e têm de ter o membro `CertValue` definido como uma cadeia ASCII codificada em base64 do certificado público.</span><span class="sxs-lookup"><span data-stu-id="70347-138">These objects must have a valid `StartDate`, `EndDate`, and have the `CertValue` member set to a base64-encoded ASCII string of the public certificate.</span></span>

```azurepowershell-interactive
$cert = <public certificate as base64-encoded string>
$credentials = New-Object Microsoft.Azure.Commands.ActiveDirectory.PSADKeyCredential -Property @{ StartDate=Get-Date; EndDate=Get-Date -Year 2024; KeyId=New-Guid; CertValue=$cert}
$sp = New-AzADServicePrincipal -DisplayName ServicePrincipalName -KeyCredential $credentials
```

<span data-ttu-id="70347-139">O objeto devolvido a partir de `New-AzADServicePrincipal` contém os membros `Id` e `DisplayName`, que podem ser utilizados para iniciar sessão com o principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="70347-139">The object returned from `New-AzADServicePrincipal` contains the `Id` and `DisplayName` members, either of which can be used for sign in with the service principal.</span></span> <span data-ttu-id="70347-140">Os clientes que iniciam sessão com o principal de serviço também precisam de acesso à chave privada do certificado.</span><span class="sxs-lookup"><span data-stu-id="70347-140">Clients which sign in with the service principal also need access to the certificate's private key.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="70347-141">O início de sessão com um principal de serviço requer o ID de inquilino no qual o principal de serviço foi criado.</span><span class="sxs-lookup"><span data-stu-id="70347-141">Signing in with a service principal requires the tenant ID which the service principal was created under.</span></span> <span data-ttu-id="70347-142">Para obter o inquilino que estava ativo quando o principal de serviço foi criado, execute o seguinte comando __imediatamente após__ a criação do principal de serviço:</span><span class="sxs-lookup"><span data-stu-id="70347-142">To get the active tenant when the service principal was created, run the following command __immediately after__ service principal creation:</span></span>
>
> ```azurepowershell-interactive
> (Get-AzContext).Tenant.Id
> ```

## <a name="get-an-existing-service-principal"></a><span data-ttu-id="70347-143">Obter um principal de serviço existente</span><span class="sxs-lookup"><span data-stu-id="70347-143">Get an existing service principal</span></span>

<span data-ttu-id="70347-144">É possível obter uma lista de principais de serviço do inquilino atualmente ativo com [Get-AzADServicePrincipal](/powershell/module/az.resources/get-azadserviceprincipal).</span><span class="sxs-lookup"><span data-stu-id="70347-144">A list of service principals for the currently active tenant can be retrieved with [Get-AzADServicePrincipal](/powershell/module/az.resources/get-azadserviceprincipal).</span></span> <span data-ttu-id="70347-145">Por predefinição, este comando devolve __todos__ os principais de serviço de um inquilino, pelo que a devolução dos resultados pode ser muito demorada para as organizações de grande dimensão.</span><span class="sxs-lookup"><span data-stu-id="70347-145">By default this command returns __all__ service principals in a tenant, so for large organizations, it may take a long time to return results.</span></span> <span data-ttu-id="70347-146">Em alternativa, recomenda-se a utilização de um dos argumentos de filtragem opcionais do lado do servidor:</span><span class="sxs-lookup"><span data-stu-id="70347-146">Instead, using one of the optional server-side filtering arguments is recommended:</span></span>

* <span data-ttu-id="70347-147">`-DisplayNameBeginsWith` pede principais de serviço que tenham um _prefixo_ correspondente ao valor fornecido.</span><span class="sxs-lookup"><span data-stu-id="70347-147">`-DisplayNameBeginsWith` requests service principals that have a _prefix_ that match the provided value.</span></span> <span data-ttu-id="70347-148">O nome a apresentar de um principal de serviço é o valor definido com `-DisplayName` durante a criação.</span><span class="sxs-lookup"><span data-stu-id="70347-148">The display name of a service principal is the value set with `-DisplayName` during creation.</span></span>
* <span data-ttu-id="70347-149">`-DisplayName` pede uma _correspondência exata_ de um nome do principal do serviço.</span><span class="sxs-lookup"><span data-stu-id="70347-149">`-DisplayName` requests an _exact match_ of a service principal name.</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="70347-150">Gerir funções de principais de serviço</span><span class="sxs-lookup"><span data-stu-id="70347-150">Manage service principal roles</span></span>

<span data-ttu-id="70347-151">O Azure PowerShell dispõe dos seguintes cmdlets para gerir as atribuições de funções:</span><span class="sxs-lookup"><span data-stu-id="70347-151">Azure PowerShell has the following cmdlets to manage role assignments:</span></span>

* [<span data-ttu-id="70347-152">Get-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="70347-152">Get-AzRoleAssignment</span></span>](/powershell/module/az.resources/get-azroleassignment)
* [<span data-ttu-id="70347-153">New-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="70347-153">New-AzRoleAssignment</span></span>](/powershell/module/az.resources/new-azroleassignment)
* [<span data-ttu-id="70347-154">Remove-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="70347-154">Remove-AzRoleAssignment</span></span>](/powershell/module/az.resources/remove-azroleassignment)

<span data-ttu-id="70347-155">A função predefinida dos principais de serviço é **Contribuinte**.</span><span class="sxs-lookup"><span data-stu-id="70347-155">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="70347-156">Esta função tem permissões completas para ler e escrever numa conta do Azure.</span><span class="sxs-lookup"><span data-stu-id="70347-156">This role has full permissions to read and write to an Azure account.</span></span> <span data-ttu-id="70347-157">A função **Leitor** é mais restritiva, com acesso só de leitura.</span><span class="sxs-lookup"><span data-stu-id="70347-157">The **Reader** role is more restrictive, with read-only access.</span></span>  <span data-ttu-id="70347-158">Para obter mais informações sobre o Controlo de Acesso Baseado em Funções (RBAC) e as funções, veja [RBAC: Funções incorporadas](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="70347-158">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="70347-159">Este exemplo adiciona a função **Leitor** e remove a função **Contribuidor**:</span><span class="sxs-lookup"><span data-stu-id="70347-159">This example adds the **Reader** role and removes the **Contributor** one:</span></span>

```azurepowershell-interactive
New-AzRoleAssignment -ApplicationId <service principal application ID> -RoleDefinitionName "Reader"
Remove-AzRoleAssignment -ApplicationId <service principal application ID> -RoleDefinitionName "Contributor"
```

> [!IMPORTANT]
> <span data-ttu-id="70347-160">Os cmdlets de atribuição de funções não aceitam o ID do objeto do principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="70347-160">Role assignment cmdlets don't take the service principal object ID.</span></span> <span data-ttu-id="70347-161">Aceitam o ID da aplicação associada, gerado no momento da criação.</span><span class="sxs-lookup"><span data-stu-id="70347-161">They take the associated application ID, which is generated at creation time.</span></span> <span data-ttu-id="70347-162">Para obter o ID da aplicação de um principal de serviço, utilize `Get-AzADServicePrincipal`.</span><span class="sxs-lookup"><span data-stu-id="70347-162">To get the application ID for a service principal, use `Get-AzADServicePrincipal`.</span></span>

> [!NOTE]
> <span data-ttu-id="70347-163">Se a sua conta não tiver permissão para atribuir uma função, ser-lhe-á apresentada uma mensagem de erro com a indicação de que a sua conta "não tem autorização para realizar a ação 'Microsoft.Authorization/roleAssignments/write'". Contacte o administrador do Azure Active Directory para gerir funções.</span><span class="sxs-lookup"><span data-stu-id="70347-163">If your account doesn't have permission to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write'." Contact your Azure Active Directory admin to manage roles.</span></span>

<span data-ttu-id="70347-164">Adicionar uma função _não_ restringe as permissões atribuídas anteriormente.</span><span class="sxs-lookup"><span data-stu-id="70347-164">Adding a role _doesn't_ restrict previously assigned permissions.</span></span> <span data-ttu-id="70347-165">Quando restringir as permissões de um principal de serviço, a função __Contribuidor__ deve ser removida.</span><span class="sxs-lookup"><span data-stu-id="70347-165">When restricting a service principal's permissions, the __Contributor__ role should be removed.</span></span>

<span data-ttu-id="70347-166">As alterações podem ser verificadas ao listar as funções atribuídas:</span><span class="sxs-lookup"><span data-stu-id="70347-166">The changes can be verified by listing the assigned roles:</span></span>

```azurepowershell-interactive
Get-AzRoleAssignment -ServicePrincipalName ServicePrincipalName
```

## <a name="sign-in-using-a-service-principal"></a><span data-ttu-id="70347-167">Iniciar sessão com um principal de serviço</span><span class="sxs-lookup"><span data-stu-id="70347-167">Sign in using a service principal</span></span>

<span data-ttu-id="70347-168">Teste as credenciais e permissões do novo principal de serviço iniciando sessão.</span><span class="sxs-lookup"><span data-stu-id="70347-168">Test the new service principal's credentials and permissions by signing in.</span></span> <span data-ttu-id="70347-169">Para iniciar sessão com um principal de serviço, precisa do valor `applicationId` associado ao mesmo, bem como do inquilino em que foi criado.</span><span class="sxs-lookup"><span data-stu-id="70347-169">To sign in with a service principal, you need the `applicationId` value associated with it, and the tenant it was created under.</span></span>

<span data-ttu-id="70347-170">Para iniciar sessão com um principal de serviço através de uma palavra-passe:</span><span class="sxs-lookup"><span data-stu-id="70347-170">To sign in with a service principal using a password:</span></span>

```azurepowershell-interactive
# Use the application ID as the username, and the secret as password
$credentials = Get-Credential
Connect-AzAccount -ServicePrincipal -Credential $credentials -Tenant <tenant ID> 
```

<span data-ttu-id="70347-171">A autenticação baseada em certificado precisa que o Azure PowerShell tenha a capacidade de obter informações de um arquivo de certificados local com base num thumbprint do certificado.</span><span class="sxs-lookup"><span data-stu-id="70347-171">Certificate-based authentication requires that Azure PowerShell can retrieve information from a local certificate store based on a certificate thumbprint.</span></span>

```azurepowershell-interactive
Connect-AzAccount -ServicePrincipal -Tenant <tenant ID> -CertificateThumbprint <thumbprint>
```

<span data-ttu-id="70347-172">Para obter instruções sobre como importar um certificado para um arquivo de credenciais acessível ao PowerShell, veja [Sign in with Azure PowerShell](authenticate-azureps.md#sp-signin) (Iniciar sessão com o Azure PowerShell)</span><span class="sxs-lookup"><span data-stu-id="70347-172">For instructions on importing a certificate into a credential store accessible by PowerShell, see [Sign in with Azure PowerShell](authenticate-azureps.md#sp-signin)</span></span>

## <a name="reset-credentials"></a><span data-ttu-id="70347-173">Repor credenciais</span><span class="sxs-lookup"><span data-stu-id="70347-173">Reset credentials</span></span>

<span data-ttu-id="70347-174">Se se esquecer das credenciais de um principal de serviço, utilize [New-AzADSpCredential](/powershell/module/az.resources/new-azadspcredential) para adicionar uma credencial nova.</span><span class="sxs-lookup"><span data-stu-id="70347-174">If you forget the credentials for a service principal, use [New-AzADSpCredential](/powershell/module/az.resources/new-azadspcredential) to add a new credential.</span></span> <span data-ttu-id="70347-175">Este cmdlet aceita os mesmos tipos e argumentos de credencial que `New-AzADServicePrincipal`.</span><span class="sxs-lookup"><span data-stu-id="70347-175">This cmdlet takes the same credential arguments and types as `New-AzADServicePrincipal`.</span></span> <span data-ttu-id="70347-176">Na ausência de argumentos de credencial, é criada uma nova `PasswordCredential` com uma palavra-passe aleatória.</span><span class="sxs-lookup"><span data-stu-id="70347-176">Without any credential arguments, a new `PasswordCredential` with a random password is created.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="70347-177">Antes de atribuir credenciais novas, convém remover as credenciais existentes para evitar iniciar sessão com as mesmas.</span><span class="sxs-lookup"><span data-stu-id="70347-177">Before assigning any new credentials, you may want to remove existing credentials to prevent sign in with them.</span></span> <span data-ttu-id="70347-178">Para tal, utilize o cmdlet [Remove-AzADSpCredential](/powershell/module/az.resources/remove-azadspcredential):</span><span class="sxs-lookup"><span data-stu-id="70347-178">To do so, use the [Remove-AzADSpCredential](/powershell/module/az.resources/remove-azadspcredential) cmdlet:</span></span>
>
> ```azurepowershell-interactive
> Remove-AzADSpCredential -DisplayName ServicePrincipalName
> ```

```azurepowershell-interactive
$newCredential = New-AzADSpCredential -ServicePrincipalName ServicePrincipalName
```
