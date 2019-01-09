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
ms.sourcegitcommit: 797c18f93aaa495ef005993b2e202d7378588dfa
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/19/2018
ms.locfileid: "53594960"
---
# <a name="create-an-azure-service-principal-with-azure-powershell"></a>Criar um principal de serviço do Azure com o Azure PowerShell

Se pretender gerir o seu serviço ou aplicação com o Azure PowerShell, deve executá-lo num principal de serviço do Azure Active Directory (AAD) em vez de utilizar as suas próprias credenciais. Este artigo orienta-o ao longo da criação de um principal de segurança com o Azure PowerShell.

## <a name="what-is-a-service-principal"></a>O que é um principal de serviço?

Um principal de serviço do Azure é uma identidade de segurança utilizada por aplicações e serviços criados por utilizadores e ferramentas de automatização para aceder a recursos do Azure específicos. Os principais de serviço são permissões específicas atribuídas relacionadas com as tarefas dos mesmos, o que permite um maior controlo de segurança. Não se parecem com uma identidade de utilizador geral, que geralmente tem autorização para fazer qualquer alteração.

## <a name="verify-your-own-permission-level"></a>Verificar o seu nível de permissões

Em primeiro lugar, tem de ter permissões suficientes na sua subscrição do Azure e no Azure Active Directory. Tem de poder criar uma aplicação no Active Directory e atribuir uma função ao principal de serviço.

A forma mais fácil de verificar se a sua conta tem permissões adequadas é utilizar o portal. Veja [Verificar as permissões necessárias no portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions).

## <a name="create-a-service-principal-for-your-app"></a>Criar um principal de serviço para a sua aplicação

Quando tiver iniciado sessão na sua conta do Azure, pode criar o principal de serviço. Tem de ter um dos seguintes modos de identificação da sua aplicação implementada:

* O nome exclusivo da aplicação implementada, tal como "MyDemoWebApp" nos exemplos seguintes
* O ID da Aplicação, o GUID exclusivo associado à aplicação implementada, serviço ou objeto

### <a name="get-information-about-your-application"></a>Obter informações sobre a sua aplicação

O cmdlet `Get-AzADApplication` pode servir para obter informações sobre a aplicação.

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

### <a name="create-a-service-principal-for-your-application"></a>Criar um principal de serviço para a sua aplicação

O cmdlet `New-AzADServicePrincipal` é utilizado para criar o principal de serviço.

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

A partir daqui, pode optar por utilizar diretamente a propriedade `$servicePrincipal.Secret` como um argumento para `Connect-AzAccount` (veja "Iniciar sessão com o principal de serviço") ou pode converter `SecureString` numa cadeia de texto sem formatação:

```azurepowershell-interactive
$BSTR = [System.Runtime.InteropServices.Marshal]::SecureStringToBSTR($servicePrincipal.Secret)
$password = [System.Runtime.InteropServices.Marshal]::PtrToStringAuto($BSTR)
[Runtime.InteropServices.Marshal]::ZeroFreeBSTR($BSTR)
```

### <a name="sign-in-using-the-service-principal"></a>Iniciar sessão com o principal de serviço

Agora, já pode iniciar sessão como o novo principal de serviço da sua aplicação com o `appId` que forneceu e o `password`  
que foi gerado. Também vai precisar do ID de Inquilino para o principal de serviço. O ID do Inquilino é apresentado ao iniciar sessão no Azure com as suas credenciais pessoais. Para iniciar sessão com um principal de serviço, utilize os comandos:

```azurepowershell-interactive
$cred = New-Object System.Management.Automation.PSCredential ("00c01aaa-1603-49fc-b6df-b78c4e5138b4", $servicePrincipal.Secret)
Connect-AzAccount -Credential $cred -ServicePrincipal -TenantId XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```

Depois de iniciar sessão com êxito, verá o resultado da seguinte forma:

```output
Environment           : AzureCloud
Account               : 00c01aaa-1603-49fc-b6df-b78c4e5138b4
TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
SubscriptionId        :
SubscriptionName      :
CurrentStorageAccount :
```

Parabéns! Pode utilizar estas credenciais para executar a aplicação. Em seguida, tem de ajustar as permissões do principal de serviço.

## <a name="managing-roles"></a>Gerir funções

> [!NOTE]
> O Controlo de Acesso Baseado em Funções (RBAC) do Azure é um modelo para definir e gerir funções para principais de utilizador e serviço. As funções têm conjuntos de permissões associadas às mesmas, que determinam os recursos que o principal pode ler, aceder, escrever ou gerir. Para obter mais informações sobre RBAC e funções, veja [RBAC: Funções incorporadas](/azure/active-directory/role-based-access-built-in-roles).

O Azure PowerShell disponibiliza os cmdlets seguintes para gerir atribuições de funções:

* [Get-AzRoleAssignment](/powershell/module/az.resources/get-azroleassignment)
* [New-AzRoleAssignment](/powershell/module/az.resources/new-azroleassignment)
* [Remove-AzRoleAssignment](/powershell/module/az.resources/remove-azroleassignment)

A função predefinida dos principais de serviço é **Contribuinte**. Pode não ser a melhor opção consoante o âmbito das interações da sua aplicação com os serviços do Azure, dadas as suas amplas permissões.
A função **Leitor** é mais restritiva e é uma boa escolha para aplicações só de leitura. Pode ver detalhes de permissões específicas de funções ou criar permissões personalizadas através do portal do Azure.

Neste exemplo, adicionámos a função **Leitor** ao exemplo anterior e eliminámos a função **Contribuinte**:

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

Para ver as funções atuais atribuídas:

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

Outros cmdlets do Azure PowerShell para gestão de funções:

* [Get-AzRoleDefinition](/powershell/module/az.resources/Get-azRoleDefinition)
* [New-AzRoleDefinition](/powershell/module/az.resources/New-azRoleDefinition)
* [Remove-AzRoleDefinition](/powershell/module/az.resources/Remove-azRoleDefinition)
* [Set-AzRoleDefinition](/powershell/module/az.resources/Set-azRoleDefinition)

## <a name="change-the-credentials-of-the-security-principal"></a>Alterar as credenciais do principal de segurança

Rever as permissões e atualizar a palavra-passe regularmente é uma boa prática de segurança. Também pode ser útil gerir e modificar as credenciais de segurança à medida que a sua aplicação sofre alterações. Por exemplo, podemos alterar a palavra-passe do principal de serviço ao criar uma nova palavra-passe e ao remover a antiga.

### <a name="add-a-new-password-for-the-service-principal"></a>Adicionar uma nova palavra-passe para o principal de serviço

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

### <a name="get-a-list-of-credentials-for-the-service-principal"></a>Obter uma lista de credenciais para o principal de serviço

```azurepowershell-interactive
Get-AzADSpCredential -ServicePrincipalName http://MyDemoWebApp
```

```output
StartDate           EndDate             KeyId                                Type
---------           -------             -----                                ----
3/8/2017 5:58:24 PM 3/8/2018 5:58:24 PM 6f801c3e-6fcd-42b9-be8e-320b17ba1d36 Password
5/5/2016 4:55:27 PM 5/5/2017 4:55:27 PM ca9d4846-4972-4c70-b6f5-a4effa60b9bc Password
```

### <a name="remove-the-old-password-from-the-service-principal"></a>Remover a palavra-passe antiga do principal de serviço

```azurepowershell-interactive
Remove-AzADSpCredential -ServicePrincipalName http://MyDemoWebApp -KeyId ca9d4846-4972-4c70-b6f5-a4effa60b9bc
```

```output
Confirm
Are you sure you want to remove credential with keyId '6f801c3e-6fcd-42b9-be8e-320b17ba1d36' for
service principal objectId '698138e7-d7b6-4738-a866-b4e3081a69e4'.
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

### <a name="verify-the-list-of-credentials-for-the-service-principal"></a>Verificar a lista de credenciais para o principal de serviço

```azurepowershell-interactive
Get-AzADSpCredential -ServicePrincipalName http://MyDemoWebApp
```

```output
StartDate           EndDate             KeyId                                Type
---------           -------             -----                                ----
3/8/2017 5:58:24 PM 3/8/2018 5:58:24 PM 6f801c3e-6fcd-42b9-be8e-320b17ba1d36 Password
```

### <a name="get-information-about-the-service-principal"></a>Obter informações sobre o principal de serviço

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
