---
title: Criar um principal de serviço do Azure com o Azure PowerShell
description: Saiba como criar um principal de serviço para o seu serviço ou aplicação com o Azure PowerShell.
keywords: Azure PowerShell, Azure Active Directory, Azure Active directory, AD, RBAC
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: 3e1c5ad280bdb29ce479dd0a478d0ed58237f969
ms.sourcegitcommit: c6fd0e490fa0e33b8b768b679682a47d8faae1cf
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/16/2019
ms.locfileid: "54342199"
---
# <a name="create-an-azure-service-principal-with-azure-powershell"></a><span data-ttu-id="2ad22-104">Criar um principal de serviço do Azure com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="2ad22-104">Create an Azure service principal with Azure PowerShell</span></span>

<span data-ttu-id="2ad22-105">Se pretender gerir o seu serviço ou aplicação com o Azure PowerShell, deve executá-lo num principal de serviço do Azure Active Directory (AAD) em vez de utilizar as suas próprias credenciais.</span><span class="sxs-lookup"><span data-stu-id="2ad22-105">If you plan to manage your app or service with Azure PowerShell, you should run it under an Azure Active Directory (AAD) service principal, rather than your own credentials.</span></span> <span data-ttu-id="2ad22-106">Este artigo orienta-o ao longo da criação de um principal de segurança com o Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2ad22-106">This article steps you through creating a security principal with Azure PowerShell.</span></span>

## <a name="what-is-a-service-principal"></a><span data-ttu-id="2ad22-107">O que é um principal de serviço?</span><span class="sxs-lookup"><span data-stu-id="2ad22-107">What is a service principal?</span></span>

<span data-ttu-id="2ad22-108">Um principal de serviço do Azure é uma identidade de segurança utilizada por aplicações e serviços criados por utilizadores e ferramentas de automatização para aceder a recursos do Azure específicos.</span><span class="sxs-lookup"><span data-stu-id="2ad22-108">An Azure service principal is a security identity used by user-created apps, services, and automation tools to access specific Azure resources.</span></span> <span data-ttu-id="2ad22-109">Os principais de serviço são permissões específicas atribuídas relacionadas com as tarefas dos mesmos, o que permite um maior controlo de segurança.</span><span class="sxs-lookup"><span data-stu-id="2ad22-109">Service principals are assigned specific permissions related to their tasks, giving you better security control.</span></span> <span data-ttu-id="2ad22-110">Não se parecem com uma identidade de utilizador geral, que geralmente tem autorização para fazer qualquer alteração.</span><span class="sxs-lookup"><span data-stu-id="2ad22-110">This is unlike a general user identity, which is usually authorized to make any changes.</span></span>

## <a name="verify-your-own-permission-level"></a><span data-ttu-id="2ad22-111">Verificar o seu nível de permissões</span><span class="sxs-lookup"><span data-stu-id="2ad22-111">Verify your own permission level</span></span>

<span data-ttu-id="2ad22-112">Em primeiro lugar, tem de ter permissões suficientes na sua subscrição do Azure e no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2ad22-112">First, you must have sufficient permissions in both your Azure Active Directory and your Azure subscription.</span></span> <span data-ttu-id="2ad22-113">Tem de poder criar uma aplicação no Active Directory e atribuir uma função ao principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="2ad22-113">You must be able to create an app in the Active Directory and assign a role to the service principal.</span></span>

<span data-ttu-id="2ad22-114">A forma mais fácil de verificar se a sua conta tem permissões adequadas é utilizar o portal.</span><span class="sxs-lookup"><span data-stu-id="2ad22-114">The easiest way to check whether your account has the right permissions is through the portal.</span></span> <span data-ttu-id="2ad22-115">Veja [Verificar as permissões necessárias no portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions).</span><span class="sxs-lookup"><span data-stu-id="2ad22-115">See [Check required permission in portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions).</span></span>

## <a name="create-a-service-principal-for-your-app"></a><span data-ttu-id="2ad22-116">Criar um principal de serviço para a sua aplicação</span><span class="sxs-lookup"><span data-stu-id="2ad22-116">Create a service principal for your app</span></span>

<span data-ttu-id="2ad22-117">Quando tiver iniciado sessão na sua conta do Azure, pode criar o principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="2ad22-117">Once signed in to your Azure account, you can create the service principal.</span></span> <span data-ttu-id="2ad22-118">Tem de ter um dos seguintes modos de identificação da sua aplicação implementada:</span><span class="sxs-lookup"><span data-stu-id="2ad22-118">You must have one of the following ways to identify your deployed app:</span></span>

* <span data-ttu-id="2ad22-119">O nome exclusivo da aplicação implementada, tal como "MyDemoWebApp" nos exemplos seguintes</span><span class="sxs-lookup"><span data-stu-id="2ad22-119">The unique name of your deployed app, such as "MyDemoWebApp" in the following examples</span></span>
* <span data-ttu-id="2ad22-120">O ID da Aplicação, o GUID exclusivo associado à aplicação implementada, serviço ou objeto</span><span class="sxs-lookup"><span data-stu-id="2ad22-120">The Application ID, the unique GUID associated with your deployed app, service, or object</span></span>

### <a name="get-information-about-your-application"></a><span data-ttu-id="2ad22-121">Obter informações sobre a sua aplicação</span><span class="sxs-lookup"><span data-stu-id="2ad22-121">Get information about your application</span></span>

<span data-ttu-id="2ad22-122">O cmdlet `Get-AzADApplication` pode servir para obter informações sobre a aplicação.</span><span class="sxs-lookup"><span data-stu-id="2ad22-122">The `Get-AzADApplication` cmdlet can be used to get information about your application.</span></span>

```azurepowershell-interactive
$app = Get-AzADApplication -DisplayNameStartWith MyDemoWebApp
$app
```

```output
DisplayName             : MyDemoWebApp
ObjectId                : 775f64cd-0ec8-4b9b-b69a-8b8946022d9f
IdentifierUris          : {http://MyDemoWebApp}
HomePage                : http://www.contoso.com
Type                    : Application
ApplicationId           : 00c01aaa-1603-49fc-b6df-b78c4e5138b4
AvailableToOtherTenants : False
AppPermissions          :
ReplyUrls               : {}
```

### <a name="create-a-service-principal-for-your-application"></a><span data-ttu-id="2ad22-123">Criar um principal de serviço para a sua aplicação</span><span class="sxs-lookup"><span data-stu-id="2ad22-123">Create a service principal for your application</span></span>

<span data-ttu-id="2ad22-124">O cmdlet `New-AzADServicePrincipal` é utilizado para criar o principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="2ad22-124">The `New-AzADServicePrincipal` cmdlet is used to create the service principal.</span></span>

```azurepowershell-interactive
$servicePrincipal = New-AzADServicePrincipal -ApplicationId 00c01aaa-1603-49fc-b6df-b78c4e5138b4
```

```output
Secret                : System.Security.SecureString
ServicePrincipalNames : {00c01aaa-1603-49fc-b6df-b78c4e5138b4, http://MyDemoWebApp}
ApplicationId         : 00c01aaa-1603-49fc-b6df-b78c4e5138b4
DisplayName           : MyDemoWebApp
Id                    : 698138e7-d7b6-4738-a866-b4e3081a69e4
AdfsId                :
Type                  : ServicePrincipal
```

<span data-ttu-id="2ad22-125">A partir daqui, pode optar por utilizar diretamente a propriedade `$servicePrincipal.Secret` como um argumento para `Connect-AzAccount` (veja "Iniciar sessão com o principal de serviço") ou pode converter `SecureString` numa cadeia de texto sem formatação:</span><span class="sxs-lookup"><span data-stu-id="2ad22-125">From here, you can either directly use the `$servicePrincipal.Secret` property as an argument to `Connect-AzAccount` (see "Sign in using the service principal"), or you can convert this `SecureString` to a plain text string:</span></span>

```azurepowershell-interactive
$BSTR = [System.Runtime.InteropServices.Marshal]::SecureStringToBSTR($servicePrincipal.Secret)
$password = [System.Runtime.InteropServices.Marshal]::PtrToStringAuto($BSTR)
[Runtime.InteropServices.Marshal]::ZeroFreeBSTR($BSTR)
```

### <a name="sign-in-using-the-service-principal"></a><span data-ttu-id="2ad22-126">Iniciar sessão com o principal de serviço</span><span class="sxs-lookup"><span data-stu-id="2ad22-126">Sign in using the service principal</span></span>

<span data-ttu-id="2ad22-127">Agora, já pode iniciar sessão como o novo principal de serviço da sua aplicação com o `appId` que forneceu e o `password`</span><span class="sxs-lookup"><span data-stu-id="2ad22-127">You can now sign in as the new service principal for your app using the `appId` you provided and `password` that was</span></span>  
<span data-ttu-id="2ad22-128">que foi gerado.</span><span class="sxs-lookup"><span data-stu-id="2ad22-128">generated.</span></span> <span data-ttu-id="2ad22-129">Também vai precisar do ID de Inquilino para o principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="2ad22-129">You also need the Tenant ID for the service principal.</span></span> <span data-ttu-id="2ad22-130">O ID do Inquilino é apresentado ao iniciar sessão no Azure com as suas credenciais pessoais.</span><span class="sxs-lookup"><span data-stu-id="2ad22-130">Your Tenant ID is displayed when you sign into Azure with your personal credentials.</span></span> <span data-ttu-id="2ad22-131">Para iniciar sessão com um principal de serviço, utilize os comandos:</span><span class="sxs-lookup"><span data-stu-id="2ad22-131">To sign in with a service principal, use the commands:</span></span>

```azurepowershell-interactive
$cred = New-Object System.Management.Automation.PSCredential ("00c01aaa-1603-49fc-b6df-b78c4e5138b4", $servicePrincipal.Secret)
Connect-AzAccount -Credential $cred -ServicePrincipal -TenantId XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```

<span data-ttu-id="2ad22-132">Depois de iniciar sessão com êxito, verá o resultado da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="2ad22-132">After a successful sign-in you see output like:</span></span>

```output
Environment           : AzureCloud
Account               : 00c01aaa-1603-49fc-b6df-b78c4e5138b4
TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
SubscriptionId        :
SubscriptionName      :
CurrentStorageAccount :
```

<span data-ttu-id="2ad22-133">Parabéns!</span><span class="sxs-lookup"><span data-stu-id="2ad22-133">Congratulations!</span></span> <span data-ttu-id="2ad22-134">Pode utilizar estas credenciais para executar a aplicação.</span><span class="sxs-lookup"><span data-stu-id="2ad22-134">You can use these credentials to run your app.</span></span> <span data-ttu-id="2ad22-135">Em seguida, tem de ajustar as permissões do principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="2ad22-135">Next, you need to adjust the permissions of the service principal.</span></span>

## <a name="managing-roles"></a><span data-ttu-id="2ad22-136">Gerir funções</span><span class="sxs-lookup"><span data-stu-id="2ad22-136">Managing roles</span></span>

> [!NOTE]
> <span data-ttu-id="2ad22-137">O Controlo de Acesso Baseado em Funções (RBAC) do Azure é um modelo para definir e gerir funções para principais de utilizador e serviço.</span><span class="sxs-lookup"><span data-stu-id="2ad22-137">Azure Role-Based Access Control (RBAC) is a model for defining and managing roles for user and service principals.</span></span> <span data-ttu-id="2ad22-138">As funções têm conjuntos de permissões associadas às mesmas, que determinam os recursos que o principal pode ler, aceder, escrever ou gerir.</span><span class="sxs-lookup"><span data-stu-id="2ad22-138">Roles have sets of permissions associated with them, which determine the resources a principal can read, access, write, or manage.</span></span> <span data-ttu-id="2ad22-139">Para obter mais informações sobre RBAC e funções, veja [RBAC: Funções incorporadas](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="2ad22-139">For more information on RBAC and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="2ad22-140">O Azure PowerShell disponibiliza os cmdlets seguintes para gerir atribuições de funções:</span><span class="sxs-lookup"><span data-stu-id="2ad22-140">Azure PowerShell provides the following cmdlets to manage role assignments:</span></span>

* [<span data-ttu-id="2ad22-141">Get-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="2ad22-141">Get-AzRoleAssignment</span></span>](/powershell/module/az.resources/get-azroleassignment)
* [<span data-ttu-id="2ad22-142">New-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="2ad22-142">New-AzRoleAssignment</span></span>](/powershell/module/az.resources/new-azroleassignment)
* [<span data-ttu-id="2ad22-143">Remove-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="2ad22-143">Remove-AzRoleAssignment</span></span>](/powershell/module/az.resources/remove-azroleassignment)

<span data-ttu-id="2ad22-144">A função predefinida dos principais de serviço é **Contribuinte**.</span><span class="sxs-lookup"><span data-stu-id="2ad22-144">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="2ad22-145">Pode não ser a melhor opção consoante o âmbito das interações da sua aplicação com os serviços do Azure, dadas as suas amplas permissões.</span><span class="sxs-lookup"><span data-stu-id="2ad22-145">It may not be the best choice depending on the scope of your app's interactions with Azure services, given its broad permissions.</span></span>
<span data-ttu-id="2ad22-146">A função **Leitor** é mais restritiva e é uma boa escolha para aplicações só de leitura.</span><span class="sxs-lookup"><span data-stu-id="2ad22-146">The **Reader** role is more restrictive and can be a good choice for read-only apps.</span></span> <span data-ttu-id="2ad22-147">Pode ver detalhes de permissões específicas de funções ou criar permissões personalizadas através do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="2ad22-147">You can view details on role-specific permissions or create custom ones through the Azure portal.</span></span>

<span data-ttu-id="2ad22-148">Neste exemplo, adicionámos a função **Leitor** ao exemplo anterior e eliminámos a função **Contribuinte**:</span><span class="sxs-lookup"><span data-stu-id="2ad22-148">In this example, we add the **Reader** role to our prior example, and delete the **Contributor** one:</span></span>

```azurepowershell-interactive
New-AzRoleAssignment -ResourceGroupName myRG -ObjectId 698138e7-d7b6-4738-a866-b4e3081a69e4 -RoleDefinitionName Reader
```

```output
RoleAssignmentId   : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/myRG/providers/Microsoft.Authorization/roleAssignments/818892f2-d075-46a1-a3a2-3a4e1a12fcd5
Scope              : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/myRG
DisplayName        : MyDemoWebApp
SignInName         :
RoleDefinitionName : Reader
RoleDefinitionId   : b24988ac-6180-42a0-ab88-20f7382dd24c
ObjectId           : 698138e7-d7b6-4738-a866-b4e3081a69e4
ObjectType         : ServicePrincipal
```

```azurepowershell-interactive
Remove-AzRoleAssignment -ResourceGroupName myRG -ObjectId 698138e7-d7b6-4738-a866-b4e3081a69e4 -RoleDefinitionName Contributor
```

<span data-ttu-id="2ad22-149">Para ver as funções atuais atribuídas:</span><span class="sxs-lookup"><span data-stu-id="2ad22-149">To view the current roles assigned:</span></span>

```azurepowershell-interactive
Get-AzRoleAssignment -ResourceGroupName myRG -ObjectId 698138e7-d7b6-4738-a866-b4e3081a69e4
```

```output
RoleAssignmentId   : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/myRG/providers/Microsoft.Authorization/roleAssignments/0906bbd8-9982-4c03-8dae-aeaae8b13f9e
Scope              : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/myRG
DisplayName        : MyDemoWebApp
SignInName         :
RoleDefinitionName : Reader
RoleDefinitionId   : acdd72a7-3385-48ef-bd42-f606fba81ae7
ObjectId           : 698138e7-d7b6-4738-a866-b4e3081a69e4
ObjectType         : ServicePrincipal
```

<span data-ttu-id="2ad22-150">Outros cmdlets do Azure PowerShell para gestão de funções:</span><span class="sxs-lookup"><span data-stu-id="2ad22-150">Other Azure PowerShell cmdlets for role management:</span></span>

* [<span data-ttu-id="2ad22-151">Get-AzRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2ad22-151">Get-AzRoleDefinition</span></span>](/powershell/module/az.resources/Get-azRoleDefinition)
* [<span data-ttu-id="2ad22-152">New-AzRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2ad22-152">New-AzRoleDefinition</span></span>](/powershell/module/az.resources/New-azRoleDefinition)
* [<span data-ttu-id="2ad22-153">Remove-AzRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2ad22-153">Remove-AzRoleDefinition</span></span>](/powershell/module/az.resources/Remove-azRoleDefinition)
* [<span data-ttu-id="2ad22-154">Set-AzRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2ad22-154">Set-AzRoleDefinition</span></span>](/powershell/module/az.resources/Set-azRoleDefinition)

## <a name="change-the-credentials-of-the-security-principal"></a><span data-ttu-id="2ad22-155">Alterar as credenciais do principal de segurança</span><span class="sxs-lookup"><span data-stu-id="2ad22-155">Change the credentials of the security principal</span></span>

<span data-ttu-id="2ad22-156">Rever as permissões e atualizar a palavra-passe regularmente é uma boa prática de segurança.</span><span class="sxs-lookup"><span data-stu-id="2ad22-156">It's a good security practice to review the permissions and update the password regularly.</span></span> <span data-ttu-id="2ad22-157">Também pode ser útil gerir e modificar as credenciais de segurança à medida que a sua aplicação sofre alterações.</span><span class="sxs-lookup"><span data-stu-id="2ad22-157">You may also want to manage and modify the security credentials as your app changes.</span></span> <span data-ttu-id="2ad22-158">Por exemplo, podemos alterar a palavra-passe do principal de serviço ao criar uma nova palavra-passe e ao remover a antiga.</span><span class="sxs-lookup"><span data-stu-id="2ad22-158">For example, we can change the password of the service principal by creating a new password and removing the old one.</span></span>

### <a name="add-a-new-password-for-the-service-principal"></a><span data-ttu-id="2ad22-159">Adicionar uma nova palavra-passe para o principal de serviço</span><span class="sxs-lookup"><span data-stu-id="2ad22-159">Add a new password for the service principal</span></span>

```azurepowershell-interactive
New-AzADSpCredential -ServicePrincipalName http://MyDemoWebApp
```

```output
Secret    : System.Security.SecureString
StartDate : 11/16/2018 12:38:23 AM
EndDate   : 11/16/2019 12:38:23 AM
KeyId     : 6f801c3e-6fcd-42b9-be8e-320b17ba1d36
Type      : Password
```

### <a name="get-a-list-of-credentials-for-the-service-principal"></a><span data-ttu-id="2ad22-160">Obter uma lista de credenciais para o principal de serviço</span><span class="sxs-lookup"><span data-stu-id="2ad22-160">Get a list of credentials for the service principal</span></span>

```azurepowershell-interactive
Get-AzADSpCredential -ServicePrincipalName http://MyDemoWebApp
```

```output
StartDate           EndDate             KeyId                                Type
---------           -------             -----                                ----
3/8/2017 5:58:24 PM 3/8/2018 5:58:24 PM 6f801c3e-6fcd-42b9-be8e-320b17ba1d36 Password
5/5/2016 4:55:27 PM 5/5/2017 4:55:27 PM ca9d4846-4972-4c70-b6f5-a4effa60b9bc Password
```

### <a name="remove-the-old-password-from-the-service-principal"></a><span data-ttu-id="2ad22-161">Remover a palavra-passe antiga do principal de serviço</span><span class="sxs-lookup"><span data-stu-id="2ad22-161">Remove the old password from the service principal</span></span>

```azurepowershell-interactive
Remove-AzADSpCredential -ServicePrincipalName http://MyDemoWebApp -KeyId ca9d4846-4972-4c70-b6f5-a4effa60b9bc
```

```output
Confirm
Are you sure you want to remove credential with keyId '6f801c3e-6fcd-42b9-be8e-320b17ba1d36' for
service principal objectId '698138e7-d7b6-4738-a866-b4e3081a69e4'.
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

### <a name="verify-the-list-of-credentials-for-the-service-principal"></a><span data-ttu-id="2ad22-162">Verificar a lista de credenciais para o principal de serviço</span><span class="sxs-lookup"><span data-stu-id="2ad22-162">Verify the list of credentials for the service principal</span></span>

```azurepowershell-interactive
Get-AzADSpCredential -ServicePrincipalName http://MyDemoWebApp
```

```output
StartDate           EndDate             KeyId                                Type
---------           -------             -----                                ----
3/8/2017 5:58:24 PM 3/8/2018 5:58:24 PM 6f801c3e-6fcd-42b9-be8e-320b17ba1d36 Password
```

### <a name="get-information-about-the-service-principal"></a><span data-ttu-id="2ad22-163">Obter informações sobre o principal de serviço</span><span class="sxs-lookup"><span data-stu-id="2ad22-163">Get information about the service principal</span></span>

```azurepowershell-interactive
$svcprincipal = Get-AzADServicePrincipal -ObjectId 698138e7-d7b6-4738-a866-b4e3081a69e4
$svcprincipal | Select-Object *
```

```output
ServicePrincipalNames : {http://MyDemoWebApp, 00c01aaa-1603-49fc-b6df-b78c4e5138b4}
ApplicationId         : 00c01aaa-1603-49fc-b6df-b78c4e5138b4
DisplayName           : MyDemoWebApp
Id                    : 698138e7-d7b6-4738-a866-b4e3081a69e4
Type                  : ServicePrincipal
```
