---
title: Utilizar principais de serviço do Azure com o Azure PowerShell
description: Saiba como criar e utilizar principais de serviço com o Azure PowerShell.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 04/23/2019
ms.openlocfilehash: abb85d3d3f6a20697510447cda2c02b2703ef921
ms.sourcegitcommit: 0356a4694f77eda40eec8c3759b9bb7f28979eb6
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/18/2019
ms.locfileid: "67192806"
---
# <a name="create-an-azure-service-principal-with-azure-powershell"></a><span data-ttu-id="d03d8-103">Criar um principal de serviço do Azure com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="d03d8-103">Create an Azure service principal with Azure PowerShell</span></span>

<span data-ttu-id="d03d8-104">As ferramentas automatizadas que utilizam serviços do Azure devem ter sempre permissões restritas.</span><span class="sxs-lookup"><span data-stu-id="d03d8-104">Automated tools that use Azure services should always have restricted permissions.</span></span> <span data-ttu-id="d03d8-105">Em vez de obrigar as aplicações a iniciarem sessão como um utilizador com privilégios máximos, o Azure disponibiliza principais de serviço.</span><span class="sxs-lookup"><span data-stu-id="d03d8-105">Instead of having applications sign in as a fully privileged user, Azure offers service principals.</span></span>

<span data-ttu-id="d03d8-106">Um principal de serviço do Azure é uma identidade criada para ser utilizada com aplicações, serviços alojados e ferramentas automatizadas para aceder aos recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="d03d8-106">An Azure service principal is an identity created for use with applications, hosted services, and automated tools to access Azure resources.</span></span> <span data-ttu-id="d03d8-107">Este acesso é restringido pelas funções atribuídas ao principal de serviço, o que lhe permite assumir o controlo dos recursos que podem ser acedidos e em que nível.</span><span class="sxs-lookup"><span data-stu-id="d03d8-107">This access is restricted by the roles assigned to the service principal, giving you control over which resources can be accessed and at which level.</span></span> <span data-ttu-id="d03d8-108">Por motivos de segurança, é sempre recomendado utilizar os principais de serviço com ferramentas automatizadas, em vez de permitir que iniciem sessão com uma identidade de utilizador.</span><span class="sxs-lookup"><span data-stu-id="d03d8-108">For security reasons, it's always recommended to use service principals with automated tools rather than allowing them to log in with a user identity.</span></span>

<span data-ttu-id="d03d8-109">Este artigo mostra-lhe os passos para criar, obter informações e repor um principal de serviço com o Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d03d8-109">This article shows you the steps for creating, getting information about, and resetting a service principal with Azure PowerShell.</span></span>

## <a name="create-a-service-principal"></a><span data-ttu-id="d03d8-110">Criar um principal de serviço</span><span class="sxs-lookup"><span data-stu-id="d03d8-110">Create a service principal</span></span>

<span data-ttu-id="d03d8-111">Crie um principal de serviço com o cmdlet [New-AzADServicePrincipal](/powershell/module/Az.Resources/New-AzADServicePrincipal).</span><span class="sxs-lookup"><span data-stu-id="d03d8-111">Create a service principal with the [New-AzADServicePrincipal](/powershell/module/Az.Resources/New-AzADServicePrincipal) cmdlet.</span></span> <span data-ttu-id="d03d8-112">Quando cria um principal de serviço, escolhe o tipo de autenticação de início de sessão que o mesmo utiliza.</span><span class="sxs-lookup"><span data-stu-id="d03d8-112">When creating a service principal, you choose the type of sign-in authentication it uses.</span></span>

> [!NOTE]
>
> <span data-ttu-id="d03d8-113">Se a sua conta não tiver permissão para criar um principal de serviço, o cmdlet `New-AzADServicePrincipal` devolve uma mensagem de erro com a indicação "Privilégios insuficientes para concluir a operação".</span><span class="sxs-lookup"><span data-stu-id="d03d8-113">If your account doesn't have permission to create a service principal, `New-AzADServicePrincipal` will return an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="d03d8-114">Contacte o seu administrador do Azure Active Directory para criar um principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="d03d8-114">Contact your Azure Active Directory admin to create a service principal.</span></span>

<span data-ttu-id="d03d8-115">Existem dois tipos de autenticação disponíveis para os principais de serviço: a autenticação baseada em palavra-passe e a autenticação baseada em certificado.</span><span class="sxs-lookup"><span data-stu-id="d03d8-115">There are two types of authentication available for service principals: Password-based authentication, and certificate-based authentication.</span></span>

### <a name="password-based-authentication"></a><span data-ttu-id="d03d8-116">Autenticação baseada em palavra-passe</span><span class="sxs-lookup"><span data-stu-id="d03d8-116">Password-based authentication</span></span>

<span data-ttu-id="d03d8-117">Na ausência de outros parâmetros de autenticação, a autenticação baseada em palavra-passe é utilizada e é criada uma palavra-passe aleatória para si.</span><span class="sxs-lookup"><span data-stu-id="d03d8-117">Without any other authentication parameters, password-based authentication is used and a random password created for you.</span></span> <span data-ttu-id="d03d8-118">Se estiver interessado na autenticação baseada em palavra-passe, este é o método recomendado.</span><span class="sxs-lookup"><span data-stu-id="d03d8-118">If you want password-based authentication, this method is recommended.</span></span>

```azurepowershell-interactive
$sp = New-AzADServicePrincipal -DisplayName ServicePrincipalName
```

<span data-ttu-id="d03d8-119">O objeto devolvido contém o membro `Secret`, ou seja, uma `SecureString` que contém a palavra-passe gerada.</span><span class="sxs-lookup"><span data-stu-id="d03d8-119">The returned object contains the `Secret` member, which is a `SecureString` containing the generated password.</span></span> <span data-ttu-id="d03d8-120">Certifique-se de que armazena este valor num local seguro para efetuar a autenticação com o principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="d03d8-120">Make sure that you store this value somewhere secure to authenticate with the service principal.</span></span> <span data-ttu-id="d03d8-121">O respetivo valor __não será__ apresentado na saída da consola.</span><span class="sxs-lookup"><span data-stu-id="d03d8-121">Its value __won't__ be displayed in the console output.</span></span> <span data-ttu-id="d03d8-122">Se perder a palavra-passe, [reponha as credenciais do principal de serviço](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="d03d8-122">If you lose the password, [reset the service principal credentials](#reset-credentials).</span></span> 

<span data-ttu-id="d03d8-123">Para as palavras-passe fornecidas pelo utilizador, o argumento `-PasswordCredential` aceita objetos `Microsoft.Azure.Commands.ActiveDirectory.PSADPasswordCredential`.</span><span class="sxs-lookup"><span data-stu-id="d03d8-123">For user-supplied passwords, the `-PasswordCredential` argument takes `Microsoft.Azure.Commands.ActiveDirectory.PSADPasswordCredential` objects.</span></span> <span data-ttu-id="d03d8-124">Estes objetos têm de ter uma `StartDate` e uma `EndDate` válidas, bem como aceitar uma `Password` com texto desencriptado.</span><span class="sxs-lookup"><span data-stu-id="d03d8-124">These objects must have a valid `StartDate` and `EndDate`, and take a plaintext `Password`.</span></span> <span data-ttu-id="d03d8-125">Quando criar uma palavra-passe, certifique-se de que segue as [regras e restrições de palavra-passe do Azure Active Directory](/azure/active-directory/active-directory-passwords-policy).</span><span class="sxs-lookup"><span data-stu-id="d03d8-125">When creating a password, make sure you follow the [Azure Active Directory password rules and restrictions](/azure/active-directory/active-directory-passwords-policy).</span></span> <span data-ttu-id="d03d8-126">Não utilize uma palavra-passe fraca nem reutilize uma palavra-passe.</span><span class="sxs-lookup"><span data-stu-id="d03d8-126">Don't use a weak password or reuse a password.</span></span>

```azurepowershell-interactive
Import-Module Az.Resources # Imports the PSADPasswordCredential object
$credentials = New-Object Microsoft.Azure.Commands.ActiveDirectory.PSADPasswordCredential -Property @{ StartDate=Get-Date; EndDate=Get-Date -Year 2024; Password=<Choose a strong password>}
$sp = New-AzAdServicePrincipal -DisplayName ServicePrincipalName -PasswordCredential $credentials
```

<span data-ttu-id="d03d8-127">O objeto devolvido a partir de `New-AzADServicePrincipal` contém os membros `Id` e `DisplayName`, que podem ser utilizados para iniciar sessão com o principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="d03d8-127">The object returned from `New-AzADServicePrincipal` contains the `Id` and `DisplayName` members, either of which can be used for sign in with the service principal.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="d03d8-128">Iniciar sessão com um principal de serviço necessita do ID de inquilino no qual o principal de serviço foi criado.</span><span class="sxs-lookup"><span data-stu-id="d03d8-128">Signing in with a service principal requires the tenant ID which the service principal was created under.</span></span> <span data-ttu-id="d03d8-129">Para obter o inquilino que estava ativo quando o principal de serviço foi criado, execute o seguinte comando __imediatamente após__ a criação do principal de serviço:</span><span class="sxs-lookup"><span data-stu-id="d03d8-129">To get the active tenant when the service principal was created, run the following command __immediately after__ service principal creation:</span></span>
>
> ```azurepowershell-interactive
> (Get-AzContext).Tenant.Id
> ```

### <a name="certificate-based-authentication"></a><span data-ttu-id="d03d8-130">Autenticação baseada em certificado</span><span class="sxs-lookup"><span data-stu-id="d03d8-130">Certificate-based authentication</span></span>

<span data-ttu-id="d03d8-131">Os principais de serviço que utilizam a autenticação baseada em certificado são criados com o parâmetro `-CertValue`.</span><span class="sxs-lookup"><span data-stu-id="d03d8-131">Service principals using certificate-based authentication are created with the `-CertValue` parameter.</span></span> <span data-ttu-id="d03d8-132">Este parâmetro aceita uma cadeia ASCII codificada em base64 do certificado público.</span><span class="sxs-lookup"><span data-stu-id="d03d8-132">This parameter takes a base64-encoded ASCII string of the public certificate.</span></span> <span data-ttu-id="d03d8-133">Isto é representado por um ficheiro PEM, ou por um CRT ou CER codificado em texto.</span><span class="sxs-lookup"><span data-stu-id="d03d8-133">This is represented by a PEM file, or a text-encoded CRT or CER.</span></span> <span data-ttu-id="d03d8-134">Não são suportadas codificações binárias do certificado público.</span><span class="sxs-lookup"><span data-stu-id="d03d8-134">Binary encodings of the public certificate aren't supported.</span></span> <span data-ttu-id="d03d8-135">Estas instruções partem do princípio de que já tem um certificado disponível.</span><span class="sxs-lookup"><span data-stu-id="d03d8-135">These instructions assume that you already have a certificate available.</span></span>

```azurepowershell-interactive
$cert = <public certificate as base64-encoded string>
$sp = New-AzADServicePrincipal -DisplayName ServicePrincipalName -CertValue $cert
```

<span data-ttu-id="d03d8-136">Também pode utilizar o parâmetro `-KeyCredential`, que aceita objetos `PSADKeyCredential`.</span><span class="sxs-lookup"><span data-stu-id="d03d8-136">You can also use the `-KeyCredential` parameter, which takes `PSADKeyCredential` objects.</span></span> <span data-ttu-id="d03d8-137">Estes objetos têm de ter uma `StartDate` e uma `EndDate` válidas, e têm de ter o membro `CertValue` definido como uma cadeia ASCII codificada em base64 do certificado público.</span><span class="sxs-lookup"><span data-stu-id="d03d8-137">These objects must have a valid `StartDate`, `EndDate`, and have the `CertValue` member set to a base64-encoded ASCII string of the public certificate.</span></span>

```azurepowershell-interactive
$cert = <public certificate as base64-encoded string>
$credentials = New-Object Microsoft.Azure.Commands.ActiveDirectory.PSADKeyCredential -Property @{ StartDate=Get-Date; EndDate=Get-Date -Year 2024; KeyId=New-Guid; CertValue=$cert}
$sp = New-AzADServicePrincipal -DisplayName ServicePrincipalName -KeyCredential $credentials
```

<span data-ttu-id="d03d8-138">O objeto devolvido a partir de `New-AzADServicePrincipal` contém os membros `Id` e `DisplayName`, que podem ser utilizados para iniciar sessão com o principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="d03d8-138">The object returned from `New-AzADServicePrincipal` contains the `Id` and `DisplayName` members, either of which can be used for sign in with the service principal.</span></span> <span data-ttu-id="d03d8-139">Os clientes que iniciam sessão com o principal de serviço também precisam de acesso à chave privada do certificado.</span><span class="sxs-lookup"><span data-stu-id="d03d8-139">Clients which sign in with the service principal also need access to the certificate's private key.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="d03d8-140">Iniciar sessão com um principal de serviço necessita do ID de inquilino no qual o principal de serviço foi criado.</span><span class="sxs-lookup"><span data-stu-id="d03d8-140">Signing in with a service principal requires the tenant ID which the service principal was created under.</span></span> <span data-ttu-id="d03d8-141">Para obter o inquilino que estava ativo quando o principal de serviço foi criado, execute o seguinte comando __imediatamente após__ a criação do principal de serviço:</span><span class="sxs-lookup"><span data-stu-id="d03d8-141">To get the active tenant when the service principal was created, run the following command __immediately after__ service principal creation:</span></span>
>
> ```azurepowershell-interactive
> (Get-AzContext).Tenant.Id
> ```

## <a name="get-an-existing-service-principal"></a><span data-ttu-id="d03d8-142">Obter um principal de serviço existente</span><span class="sxs-lookup"><span data-stu-id="d03d8-142">Get an existing service principal</span></span>

<span data-ttu-id="d03d8-143">É possível obter uma lista de principais de serviço do inquilino atualmente ativo com [Get-AzADServicePrincipal](/powershell/module/az.resources/get-azadserviceprincipal).</span><span class="sxs-lookup"><span data-stu-id="d03d8-143">A list of service principals for the currently active tenant can be retrieved with [Get-AzADServicePrincipal](/powershell/module/az.resources/get-azadserviceprincipal).</span></span> <span data-ttu-id="d03d8-144">Por predefinição, este comando devolve __todos__ os principais de serviço de um inquilino, pelo que a devolução dos resultados pode ser muito demorada para as organizações de grande dimensão.</span><span class="sxs-lookup"><span data-stu-id="d03d8-144">By default this command returns __all__ service principals in a tenant, so for large organizations, it may take a long time to return results.</span></span> <span data-ttu-id="d03d8-145">Em alternativa, recomenda-se a utilização de um dos argumentos de filtragem opcionais do lado do servidor:</span><span class="sxs-lookup"><span data-stu-id="d03d8-145">Instead, using one of the optional server-side filtering arguments is recommended:</span></span>

* <span data-ttu-id="d03d8-146">`-DisplayNameBeginsWith` pede principais de serviço que tenham um _prefixo_ correspondente ao valor fornecido.</span><span class="sxs-lookup"><span data-stu-id="d03d8-146">`-DisplayNameBeginsWith` requests service principals that have a _prefix_ that match the provided value.</span></span> <span data-ttu-id="d03d8-147">O nome a apresentar de um principal de serviço é o valor definido com `-DisplayName` durante a criação.</span><span class="sxs-lookup"><span data-stu-id="d03d8-147">The display name of a service principal is the value set with `-DisplayName` during creation.</span></span>
* <span data-ttu-id="d03d8-148">`-DisplayName` pede uma _correspondência exata_ de um nome do principal do serviço.</span><span class="sxs-lookup"><span data-stu-id="d03d8-148">`-DisplayName` requests an _exact match_ of a service principal name.</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="d03d8-149">Gerir funções de principais de serviço</span><span class="sxs-lookup"><span data-stu-id="d03d8-149">Manage service principal roles</span></span>

<span data-ttu-id="d03d8-150">O Azure PowerShell dispõe dos seguintes cmdlets para gerir as atribuições de funções:</span><span class="sxs-lookup"><span data-stu-id="d03d8-150">Azure PowerShell has the following cmdlets to manage role assignments:</span></span>

* [<span data-ttu-id="d03d8-151">Get-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d03d8-151">Get-AzRoleAssignment</span></span>](/powershell/module/az.resources/get-azroleassignment)
* [<span data-ttu-id="d03d8-152">New-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d03d8-152">New-AzRoleAssignment</span></span>](/powershell/module/az.resources/new-azroleassignment)
* [<span data-ttu-id="d03d8-153">Remove-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d03d8-153">Remove-AzRoleAssignment</span></span>](/powershell/module/az.resources/remove-azroleassignment)

<span data-ttu-id="d03d8-154">A função predefinida dos principais de serviço é **Contribuinte**.</span><span class="sxs-lookup"><span data-stu-id="d03d8-154">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="d03d8-155">Esta função tem permissões completas para ler e escrever numa conta do Azure.</span><span class="sxs-lookup"><span data-stu-id="d03d8-155">This role has full permissions to read and write to an Azure account.</span></span> <span data-ttu-id="d03d8-156">A função **Leitor** é mais restritiva, com acesso só de leitura.</span><span class="sxs-lookup"><span data-stu-id="d03d8-156">The **Reader** role is more restrictive, with read-only access.</span></span>  <span data-ttu-id="d03d8-157">Para obter mais informações sobre o Controlo de Acesso Baseado em Funções (RBAC) e as funções, veja [RBAC: Funções incorporadas](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="d03d8-157">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="d03d8-158">Este exemplo adiciona a função **Leitor** e remove a função **Contribuidor**:</span><span class="sxs-lookup"><span data-stu-id="d03d8-158">This example adds the **Reader** role and removes the **Contributor** one:</span></span>

```azurepowershell-interactive
New-AzRoleAssignment -ApplicationId <service principal application ID> -RoleDefinitionName "Reader"
Remove-AzRoleAssignment -ApplicationId <service principal application ID> -RoleDefinitionName "Contributor"
```

> [!IMPORTANT]
> <span data-ttu-id="d03d8-159">Os cmdlets de atribuição de funções não aceitam o ID do objeto do principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="d03d8-159">Role assignment cmdlets don't take the service principal object ID.</span></span> <span data-ttu-id="d03d8-160">Aceitam o ID da aplicação associada, gerado no momento da criação.</span><span class="sxs-lookup"><span data-stu-id="d03d8-160">They take the associated application ID, which is generated at creation time.</span></span> <span data-ttu-id="d03d8-161">Para obter o ID da aplicação de um principal de serviço, utilize `Get-AzADServicePrincipal`.</span><span class="sxs-lookup"><span data-stu-id="d03d8-161">To get the application ID for a service principal, use `Get-AzADServicePrincipal`.</span></span>

> [!NOTE]
> <span data-ttu-id="d03d8-162">Se a sua conta não tiver permissão para atribuir uma função, ser-lhe-á apresentada uma mensagem de erro com a indicação de que a sua conta "não tem autorização para realizar a ação 'Microsoft.Authorization/roleAssignments/write'". Contacte o administrador do Azure Active Directory para gerir funções.</span><span class="sxs-lookup"><span data-stu-id="d03d8-162">If your account doesn't have permission to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write'." Contact your Azure Active Directory admin to manage roles.</span></span>

<span data-ttu-id="d03d8-163">Adicionar uma função _não_ restringe as permissões atribuídas anteriormente.</span><span class="sxs-lookup"><span data-stu-id="d03d8-163">Adding a role _doesn't_ restrict previously assigned permissions.</span></span> <span data-ttu-id="d03d8-164">Quando restringir as permissões de um principal de serviço, a função __Contribuidor__ deve ser removida.</span><span class="sxs-lookup"><span data-stu-id="d03d8-164">When restricting a service principal's permissions, the __Contributor__ role should be removed.</span></span>

<span data-ttu-id="d03d8-165">As alterações podem ser verificadas ao listar as funções atribuídas:</span><span class="sxs-lookup"><span data-stu-id="d03d8-165">The changes can be verified by listing the assigned roles:</span></span>

```azurepowershell-interactive
Get-AzRoleAssignment -ServicePrincipalName ServicePrincipalName
```

## <a name="sign-in-using-a-service-principal"></a><span data-ttu-id="d03d8-166">Iniciar sessão com um principal de serviço</span><span class="sxs-lookup"><span data-stu-id="d03d8-166">Sign in using a service principal</span></span>

<span data-ttu-id="d03d8-167">Teste as credenciais e permissões do novo principal de serviço iniciando sessão.</span><span class="sxs-lookup"><span data-stu-id="d03d8-167">Test the new service principal's credentials and permissions by signing in.</span></span> <span data-ttu-id="d03d8-168">Para iniciar sessão com um principal de serviço, precisa do valor `applicationId` associado ao mesmo, bem como do inquilino em que foi criado.</span><span class="sxs-lookup"><span data-stu-id="d03d8-168">To sign in with a service principal, you need the `applicationId` value associated with it, and the tenant it was created under.</span></span>

<span data-ttu-id="d03d8-169">Para iniciar sessão com um principal de serviço através de uma palavra-passe:</span><span class="sxs-lookup"><span data-stu-id="d03d8-169">To sign in with a service principal using a password:</span></span>

```azurepowershell-interactive
# Use the application ID as the username, and the secret as password
$credentials = Get-Credential
Connect-AzAccount -ServicePrincipal -Credential $credentials -Tenant <tenant ID> 
```

<span data-ttu-id="d03d8-170">A autenticação baseada em certificado precisa que o Azure PowerShell tenha a capacidade de obter informações de um arquivo de certificados local com base num thumbprint do certificado.</span><span class="sxs-lookup"><span data-stu-id="d03d8-170">Certificate-based authentication requires that Azure PowerShell can retrieve information from a local certificate store based on a certificate thumbprint.</span></span>

```azurepowershell-interactive
Connect-AzAccount -ServicePrincipal -TenantId $tenantId -CertificateThumbprint <thumbprint>
```

<span data-ttu-id="d03d8-171">Para obter instruções sobre como importar um certificado para um arquivo de credenciais acessível ao PowerShell, veja [Sign in with Azure PowerShell](authenticate-azureps.md#sp-signin) (Iniciar sessão com o Azure PowerShell)</span><span class="sxs-lookup"><span data-stu-id="d03d8-171">For instructions on importing a certificate into a credential store accessible by PowerShell, see [Sign in with Azure PowerShell](authenticate-azureps.md#sp-signin)</span></span>

## <a name="reset-credentials"></a><span data-ttu-id="d03d8-172">Repor credenciais</span><span class="sxs-lookup"><span data-stu-id="d03d8-172">Reset credentials</span></span>

<span data-ttu-id="d03d8-173">Se se esquecer das credenciais de um principal de serviço, utilize [New-AzADSpCredential](/powershell/module/az.resources/new-azadspcredential) para adicionar uma credencial nova.</span><span class="sxs-lookup"><span data-stu-id="d03d8-173">If you forget the credentials for a service principal, use [New-AzADSpCredential](/powershell/module/az.resources/new-azadspcredential) to add a new credential.</span></span> <span data-ttu-id="d03d8-174">Este cmdlet aceita os mesmos tipos e argumentos de credencial que `New-AzADServicePrincipal`.</span><span class="sxs-lookup"><span data-stu-id="d03d8-174">This cmdlet takes the same credential arguments and types as `New-AzADServicePrincipal`.</span></span> <span data-ttu-id="d03d8-175">Na ausência de argumentos de credencial, é criada uma nova `PasswordCredential` com uma palavra-passe aleatória.</span><span class="sxs-lookup"><span data-stu-id="d03d8-175">Without any credential arguments, a new `PasswordCredential` with a random password is created.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d03d8-176">Antes de atribuir credenciais novas, convém remover as credenciais existentes para evitar iniciar sessão com as mesmas.</span><span class="sxs-lookup"><span data-stu-id="d03d8-176">Before assigning any new credentials, you may want to remove existing credentials to prevent sign in with them.</span></span> <span data-ttu-id="d03d8-177">Para tal, utilize o cmdlet [Remove-AzADSpCredential](/powershell/module/az.resources/remove-azadspcredential):</span><span class="sxs-lookup"><span data-stu-id="d03d8-177">To do so, use the [Remove-AzADSpCredential](/powershell/module/az.resources/remove-azadspcredential) cmdlet:</span></span>
>
> ```azurepowershell-interactive
> Remove-AzADSpCredential -DisplayName ServicePrincipalName
> ```

```azurepowershell-interactive
$newCredential = New-AzADSpCredential -ServicePrincipalName ServicePrincipalName
```
