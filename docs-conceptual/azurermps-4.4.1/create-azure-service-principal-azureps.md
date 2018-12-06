---
title: Criar um principal de serviço do Azure com o Azure PowerShell
description: Saiba como criar um principal de serviço para o seu serviço ou aplicação com o Azure PowerShell.
keywords: Azure PowerShell, Azure Active Directory, Azure Active directory, AD, RBAC
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2017
ms.openlocfilehash: 19379a57e2ed369f75b2f02c73c00c1fbe02213e
ms.sourcegitcommit: 93f93b90ef88c2659be95f3acaba514fe9639169
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/05/2018
ms.locfileid: "52828761"
---
# <a name="create-an-azure-service-principal-with-azure-powershell"></a><span data-ttu-id="10fe9-104">Criar um principal de serviço do Azure com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="10fe9-104">Create an Azure service principal with Azure PowerShell</span></span>

<span data-ttu-id="10fe9-105">Se pretender gerir o seu serviço ou aplicação com o Azure PowerShell, deve executá-lo num principal de serviço do Azure Active Directory (AAD) em vez de utilizar as suas próprias credenciais.</span><span class="sxs-lookup"><span data-stu-id="10fe9-105">If you plan to manage your app or service with Azure PowerShell, you should run it under an Azure Active Directory (AAD) service principal, rather than your own credentials.</span></span> <span data-ttu-id="10fe9-106">Este tópico orienta-o ao longo da criação de um principal de segurança com o Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="10fe9-106">This topic steps you through creating a security principal with Azure PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="10fe9-107">Também pode criar um principal de serviço através do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="10fe9-107">You can also create a service principal through the Azure portal.</span></span> <span data-ttu-id="10fe9-108">Leia [Use portal to create Active Directory application and service principal that can access resources](/azure/azure-resource-manager/resource-group-create-service-principal-portal) (Utilizar o portal para criar o principal de serviço e de aplicação do Active Directory que pode aceder a recursos) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="10fe9-108">Read [Use portal to create Active Directory application and service principal that can access resources](/azure/azure-resource-manager/resource-group-create-service-principal-portal) for more details.</span></span>

## <a name="what-is-a-service-principal"></a><span data-ttu-id="10fe9-109">O que é um “principal de serviço”?</span><span class="sxs-lookup"><span data-stu-id="10fe9-109">What is a 'service principal'?</span></span>

<span data-ttu-id="10fe9-110">Um principal de serviço do Azure é uma identidade de segurança utilizada por aplicações e serviços criados por utilizadores e ferramentas de automatização para aceder a recursos do Azure específicos.</span><span class="sxs-lookup"><span data-stu-id="10fe9-110">An Azure service principal is a security identity used by user-created apps, services, and automation tools to access specific Azure resources.</span></span> <span data-ttu-id="10fe9-111">Pense nisso como uma "identidade de utilizador" (nome de utilizador e palavra-passe ou certificado) com uma função específica e permissões fortemente controladas.</span><span class="sxs-lookup"><span data-stu-id="10fe9-111">Think of it as a 'user identity' (username and password or certificate) with a specific role, and tightly controlled permissions.</span></span> <span data-ttu-id="10fe9-112">Só precisa de poder fazer determinadas coisas, ao contrário das identidades de utilizador gerais.</span><span class="sxs-lookup"><span data-stu-id="10fe9-112">It only needs to be able to do specific things, unlike a general user identity.</span></span> <span data-ttu-id="10fe9-113">Melhora a segurança se apenas lhe conceder o nível de permissões mínimo de que precisa para realizar as tarefas de gestão.</span><span class="sxs-lookup"><span data-stu-id="10fe9-113">It improves security if you only grant it the minimum permissions level needed to perform its management tasks.</span></span>

## <a name="verify-your-own-permission-level"></a><span data-ttu-id="10fe9-114">Verificar o seu nível de permissões</span><span class="sxs-lookup"><span data-stu-id="10fe9-114">Verify your own permission level</span></span>

<span data-ttu-id="10fe9-115">Em primeiro lugar, tem de ter permissões suficientes na sua subscrição do Azure e no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="10fe9-115">First, you must have sufficient permissions in both your Azure Active Directory and your Azure subscription.</span></span> <span data-ttu-id="10fe9-116">Mais concretamente, tem de poder criar uma aplicação no Active Directory e atribuir uma função ao principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="10fe9-116">Specifically, you must be able to create an app in the Active Directory, and assign a role to the service principal.</span></span>

<span data-ttu-id="10fe9-117">A forma mais fácil de verificar se a sua conta tem permissões adequadas é utilizar o portal.</span><span class="sxs-lookup"><span data-stu-id="10fe9-117">The easiest way to check whether your account has adequate permissions is through the portal.</span></span> <span data-ttu-id="10fe9-118">Veja [Verificar as permissões necessárias no portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions).</span><span class="sxs-lookup"><span data-stu-id="10fe9-118">See [Check required permission in portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions).</span></span>

## <a name="create-a-service-principal-for-your-app"></a><span data-ttu-id="10fe9-119">Criar um principal de serviço para a sua aplicação</span><span class="sxs-lookup"><span data-stu-id="10fe9-119">Create a service principal for your app</span></span>

<span data-ttu-id="10fe9-120">Quando tiver iniciado sessão na sua conta do Azure, pode criar o principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="10fe9-120">Once you are signed into your Azure account, you can create the service principal.</span></span> <span data-ttu-id="10fe9-121">Tem de ter um dos seguintes modos de identificação da sua aplicação implementada:</span><span class="sxs-lookup"><span data-stu-id="10fe9-121">You must have one of the following ways to identify your deployed app:</span></span>

* <span data-ttu-id="10fe9-122">O nome exclusivo da aplicação implementada, tal como "MyDemoWebApp" nos exemplos, ou</span><span class="sxs-lookup"><span data-stu-id="10fe9-122">The unique name of your deployed app, such as "MyDemoWebApp" in the following examples, or</span></span>
* <span data-ttu-id="10fe9-123">o ID da Aplicação, o GUID exclusivo associado à sua aplicação implementada, serviço ou objeto</span><span class="sxs-lookup"><span data-stu-id="10fe9-123">the Application ID, the unique GUID associated with your deployed app, service, or object</span></span>

### <a name="get-information-about-your-application"></a><span data-ttu-id="10fe9-124">Obter informações sobre a sua aplicação</span><span class="sxs-lookup"><span data-stu-id="10fe9-124">Get information about your application</span></span>

<span data-ttu-id="10fe9-125">O cmdlet `Get-AzureRmADApplication` pode ser utilizado para detetar informações sobre a aplicação.</span><span class="sxs-lookup"><span data-stu-id="10fe9-125">The `Get-AzureRmADApplication` cmdlet can be used to discover information about your application.</span></span>

```powershell-interactive
Get-AzureRmADApplication -DisplayNameStartWith MyDemoWebApp
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

### <a name="create-a-service-principal-for-your-application"></a><span data-ttu-id="10fe9-126">Criar um principal de serviço para a sua aplicação</span><span class="sxs-lookup"><span data-stu-id="10fe9-126">Create a service principal for your application</span></span>

<span data-ttu-id="10fe9-127">O cmdlet `New-AzureRmADServicePrincipal` é utilizado para criar o principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="10fe9-127">The `New-AzureRmADServicePrincipal` cmdlet is used to create the service principal.</span></span>

```powershell-interactive
Add-Type -Assembly System.Web
$password = [System.Web.Security.Membership]::GeneratePassword(16,3)
New-AzureRmADServicePrincipal -ApplicationId 00c01aaa-1603-49fc-b6df-b78c4e5138b4 -Password $password
```

```output
DisplayName                    Type                           ObjectId
-----------                    ----                           --------
MyDemoWebApp                   ServicePrincipal               698138e7-d7b6-4738-a866-b4e3081a69e4
```

### <a name="get-information-about-the-service-principal"></a><span data-ttu-id="10fe9-128">Obter informações sobre o principal de serviço</span><span class="sxs-lookup"><span data-stu-id="10fe9-128">Get information about the service principal</span></span>

```powershell-interactive
$svcprincipal = Get-AzureRmADServicePrincipal -ObjectId 698138e7-d7b6-4738-a866-b4e3081a69e4
$svcprincipal | Select-Object *
```

```output
ServicePrincipalNames : {http://MyDemoWebApp, 00c01aaa-1603-49fc-b6df-b78c4e5138b4}
ApplicationId         : 00c01aaa-1603-49fc-b6df-b78c4e5138b4
DisplayName           : MyDemoWebApp
Id                    : 698138e7-d7b6-4738-a866-b4e3081a69e4
Type                  : ServicePrincipal
```

### <a name="sign-in-using-the-service-principal"></a><span data-ttu-id="10fe9-129">Iniciar sessão com o principal de serviço</span><span class="sxs-lookup"><span data-stu-id="10fe9-129">Sign in using the service principal</span></span>

<span data-ttu-id="10fe9-130">Agora, pode iniciar sessão como o novo principal de serviço da sua aplicação com o *appId* e a *palavra-passe* fornecidos.</span><span class="sxs-lookup"><span data-stu-id="10fe9-130">You can now sign in as the new service principal for your app using the *appId* and *password* you provided.</span></span> <span data-ttu-id="10fe9-131">Tem de fornecer o ID do Inquilino para a sua conta.</span><span class="sxs-lookup"><span data-stu-id="10fe9-131">You need to supply the Tenant Id for your account.</span></span> <span data-ttu-id="10fe9-132">O ID do Inquilino é apresentado ao iniciar sessão no Azure com as suas credenciais pessoais.</span><span class="sxs-lookup"><span data-stu-id="10fe9-132">Your Tenant Id is displayed when you sign into Azure with your personal credentials.</span></span>

```powershell-interactive
$cred = Get-Credential -UserName $svcprincipal.ApplicationId -Message "Enter Password"
Login-AzureRmAccount -Credential $cred -ServicePrincipal -TenantId XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```

<span data-ttu-id="10fe9-133">Execute este comando a partir de uma nova sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="10fe9-133">Run this command from a new PowerShell session.</span></span> <span data-ttu-id="10fe9-134">Após um início de sessão com êxito, vê um resultado como este:</span><span class="sxs-lookup"><span data-stu-id="10fe9-134">After a successfully signing on you see output something like this:</span></span>

```output
Environment           : AzureCloud
Account               : 00c01aaa-1603-49fc-b6df-b78c4e5138b4
TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
SubscriptionId        :
SubscriptionName      :
CurrentStorageAccount :
```

<span data-ttu-id="10fe9-135">Parabéns!</span><span class="sxs-lookup"><span data-stu-id="10fe9-135">Congratulations!</span></span> <span data-ttu-id="10fe9-136">Pode utilizar estas credenciais para executar a aplicação.</span><span class="sxs-lookup"><span data-stu-id="10fe9-136">You can use these credentials to run your app.</span></span> <span data-ttu-id="10fe9-137">Em seguida, tem de ajustar as permissões do principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="10fe9-137">Next, you need to adjust the permissions of the service principal.</span></span>

## <a name="managing-roles"></a><span data-ttu-id="10fe9-138">Gerir funções</span><span class="sxs-lookup"><span data-stu-id="10fe9-138">Managing roles</span></span>

> [!NOTE]
> <span data-ttu-id="10fe9-139">O Controlo de Acesso Baseado em Funções (RBAC) do Azure é um modelo para definir e gerir funções para principais de utilizador e serviço.</span><span class="sxs-lookup"><span data-stu-id="10fe9-139">Azure Role-Based Access Control (RBAC) is a model for defining and managing roles for user and service principals.</span></span> <span data-ttu-id="10fe9-140">As funções têm conjuntos de permissões associadas às mesmas, que determinam os recursos que o principal pode ler, aceder, escrever ou gerir.</span><span class="sxs-lookup"><span data-stu-id="10fe9-140">Roles have sets of permissions associated with them, which determine the resources a principal can read, access, write, or manage.</span></span> <span data-ttu-id="10fe9-141">Para obter mais informações sobre RBAC e funções, veja [RBAC: Funções incorporadas](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="10fe9-141">For more information on RBAC and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="10fe9-142">O Azure PowerShell disponibiliza os cmdlets seguintes para gerir atribuições de funções:</span><span class="sxs-lookup"><span data-stu-id="10fe9-142">Azure PowerShell provides the following cmdlets to manage role assignments:</span></span>

* [<span data-ttu-id="10fe9-143">Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="10fe9-143">Get-AzureRmRoleAssignment</span></span>](/powershell/module/azurerm.resources/get-azurermroleassignment)
* [<span data-ttu-id="10fe9-144">New-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="10fe9-144">New-AzureRmRoleAssignment</span></span>](/powershell/module/azurerm.resources/new-azurermroleassignment)
* [<span data-ttu-id="10fe9-145">Remove-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="10fe9-145">Remove-AzureRmRoleAssignment</span></span>](/powershell/module/azurerm.resources/remove-azurermroleassignment)

<span data-ttu-id="10fe9-146">A função predefinida dos principais de serviço é **Contribuinte**.</span><span class="sxs-lookup"><span data-stu-id="10fe9-146">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="10fe9-147">Pode não ser a melhor opção consoante o âmbito das interações da sua aplicação com os serviços do Azure, dadas as suas amplas permissões.</span><span class="sxs-lookup"><span data-stu-id="10fe9-147">It may not be the best choice depending on the scope of your app's interactions with Azure services, given its broad permissions.</span></span>
<span data-ttu-id="10fe9-148">A função **Leitor** é mais restritiva e é uma boa escolha para aplicações só de leitura.</span><span class="sxs-lookup"><span data-stu-id="10fe9-148">The **Reader** role is more restrictive and can be a good choice for read-only apps.</span></span> <span data-ttu-id="10fe9-149">Pode ver detalhes de permissões específicas de funções ou criar permissões personalizadas através do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="10fe9-149">You can view details on role-specific permissions or create custom ones through the Azure portal.</span></span>

<span data-ttu-id="10fe9-150">Neste exemplo, adicionámos a função **Leitor** ao exemplo anterior e eliminámos a função **Contribuinte**:</span><span class="sxs-lookup"><span data-stu-id="10fe9-150">In this example, we add the **Reader** role to our prior example, and delete the **Contributor** one:</span></span>

```powershell-interactive
New-AzureRmRoleAssignment -ResourceGroupName myRG -ObjectId 698138e7-d7b6-4738-a866-b4e3081a69e4 -RoleDefinitionName Reader
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

```powershell-interactive
Remove-AzureRmRoleAssignment -ResourceGroupName myRG -ObjectId 698138e7-d7b6-4738-a866-b4e3081a69e4 -RoleDefinitionName Contributor
```

<span data-ttu-id="10fe9-151">Para ver as funções atuais atribuídas:</span><span class="sxs-lookup"><span data-stu-id="10fe9-151">To view the current roles assigned:</span></span>

```powershell-interactive
Get-AzureRmRoleAssignment -ResourceGroupName myRG -ObjectId 698138e7-d7b6-4738-a866-b4e3081a69e4
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

<span data-ttu-id="10fe9-152">Outros cmdlets do Azure PowerShell para gestão de funções:</span><span class="sxs-lookup"><span data-stu-id="10fe9-152">Other Azure PowerShell cmdlets for role management:</span></span>

* [<span data-ttu-id="10fe9-153">Get-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="10fe9-153">Get-AzureRmRoleDefinition</span></span>](/powershell/module/azurerm.resources/Get-AzureRmRoleDefinition)
* [<span data-ttu-id="10fe9-154">New-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="10fe9-154">New-AzureRmRoleDefinition</span></span>](/powershell/module/azurerm.resources/New-AzureRmRoleDefinition)
* [<span data-ttu-id="10fe9-155">Remove-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="10fe9-155">Remove-AzureRmRoleDefinition</span></span>](/powershell/module/azurerm.resources/Remove-AzureRmRoleDefinition)
* [<span data-ttu-id="10fe9-156">Set-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="10fe9-156">Set-AzureRmRoleDefinition</span></span>](/powershell/module/azurerm.resources/Set-AzureRmRoleDefinition)

## <a name="change-the-credentials-of-the-security-principal"></a><span data-ttu-id="10fe9-157">Alterar as credenciais do principal de segurança</span><span class="sxs-lookup"><span data-stu-id="10fe9-157">Change the credentials of the security principal</span></span>

<span data-ttu-id="10fe9-158">Rever as permissões e atualizar a palavra-passe regularmente é uma boa prática de segurança.</span><span class="sxs-lookup"><span data-stu-id="10fe9-158">It's a good security practice to review the permissions and update the password regularly.</span></span> <span data-ttu-id="10fe9-159">Também pode ser útil gerir e modificar as credenciais de segurança à medida que a sua aplicação sofre alterações.</span><span class="sxs-lookup"><span data-stu-id="10fe9-159">You may also want to manage and modify the security credentials as your app changes.</span></span> <span data-ttu-id="10fe9-160">Por exemplo, podemos alterar a palavra-passe do principal de serviço ao criar uma nova palavra-passe e ao remover a antiga.</span><span class="sxs-lookup"><span data-stu-id="10fe9-160">For example, we can change the password of the service principal by creating a new password and removing the old one.</span></span>

### <a name="add-a-new-password-for-the-service-principal"></a><span data-ttu-id="10fe9-161">Adicionar uma nova palavra-passe para o principal de serviço</span><span class="sxs-lookup"><span data-stu-id="10fe9-161">Add a new password for the service principal</span></span>

```powershell-interactive
$password = [System.Web.Security.Membership]::GeneratePassword(16,3)
New-AzureRmADSpCredential -ServicePrincipalName http://MyDemoWebApp -Password $password
```

```output
StartDate           EndDate             KeyId                                Type
---------           -------             -----                                ----
3/8/2017 5:58:24 PM 3/8/2018 5:58:24 PM 6f801c3e-6fcd-42b9-be8e-320b17ba1d36 Password
```

### <a name="get-a-list-of-credentials-for-the-service-principal"></a><span data-ttu-id="10fe9-162">Obter uma lista de credenciais para o principal de serviço</span><span class="sxs-lookup"><span data-stu-id="10fe9-162">Get a list of credentials for the service principal</span></span>

```powershell-interactive
Get-AzureRmADSpCredential -ServicePrincipalName http://MyDemoWebApp
```

```output
StartDate           EndDate             KeyId                                Type
---------           -------             -----                                ----
3/8/2017 5:58:24 PM 3/8/2018 5:58:24 PM 6f801c3e-6fcd-42b9-be8e-320b17ba1d36 Password
5/5/2016 4:55:27 PM 5/5/2017 4:55:27 PM ca9d4846-4972-4c70-b6f5-a4effa60b9bc Password
```

### <a name="remove-the-old-password-from-the-service-principal"></a><span data-ttu-id="10fe9-163">Remover a palavra-passe antiga do principal de serviço</span><span class="sxs-lookup"><span data-stu-id="10fe9-163">Remove the old password from the service principal</span></span>

```powershell-interactive
Remove-AzureRmADSpCredential -ServicePrincipalName http://MyDemoWebApp -KeyId ca9d4846-4972-4c70-b6f5-a4effa60b9bc
```

```output
Confirm
Are you sure you want to remove credential with keyId '6f801c3e-6fcd-42b9-be8e-320b17ba1d36' for
service principal objectId '698138e7-d7b6-4738-a866-b4e3081a69e4'.
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

### <a name="verify-the-list-of-credentials-for-the-service-principal"></a><span data-ttu-id="10fe9-164">Verificar a lista de credenciais para o principal de serviço</span><span class="sxs-lookup"><span data-stu-id="10fe9-164">Verify the list of credentials for the service principal</span></span>

```powershell-interactive
Get-AzureRmADSpCredential -ServicePrincipalName http://MyDemoWebApp
```

```output
StartDate           EndDate             KeyId                                Type
---------           -------             -----                                ----
3/8/2017 5:58:24 PM 3/8/2018 5:58:24 PM 6f801c3e-6fcd-42b9-be8e-320b17ba1d36 Password
```
