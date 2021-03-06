---
title: Criar um principal de serviço do Azure com o Azure PowerShell
description: Saiba como criar um principal de serviço para o seu serviço ou aplicação com o Azure PowerShell.
keywords: Azure PowerShell, Azure Active Directory, Azure Active directory, AD, RBAC
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/09/2018
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: 76456b3d0e2a0c000488c0d7518845e5f56f2c75
ms.sourcegitcommit: 8b3126b5c79f453464d90669f0046ba86b7a3424
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/01/2020
ms.locfileid: "89243332"
---
# <a name="create-an-azure-service-principal-with-azure-powershell"></a>Criar um principal de serviço do Azure com o Azure PowerShell

[!INCLUDE [migrate-to-az-banner](../../includes/migrate-to-az-banner.md)]

Se pretender gerir o seu serviço ou aplicação com o Azure PowerShell, deve executá-lo num principal de serviço do Azure Active Directory (AAD) em vez de utilizar as suas próprias credenciais. Este artigo orienta-o ao longo da criação de um principal de segurança com o Azure PowerShell.

> [!NOTE]
> Também pode criar um principal de serviço através do portal do Azure. Leia [Use portal to create Active Directory application and service principal that can access resources](/azure/azure-resource-manager/resource-group-create-service-principal-portal) (Utilizar o portal para criar o principal de serviço e de aplicação do Active Directory que pode aceder a recursos) para obter mais detalhes.

## <a name="what-is-a-service-principal"></a>O que é um “principal de serviço”?

Um principal de serviço do Azure é uma identidade de segurança utilizada por aplicações e serviços criados por utilizadores e ferramentas de automatização para aceder a recursos do Azure específicos. Pense nisso como uma "identidade de utilizador" (nome de utilizador e palavra-passe ou certificado) com uma função específica e permissões fortemente controladas. Um principal de serviço apenas precisa de fazer determinadas coisas, ao contrário das identidades de utilizador gerais. Melhora a segurança se apenas lhe conceder o nível de permissões mínimo de que precisa para realizar as tarefas de gestão.

## <a name="verify-your-own-permission-level"></a>Verificar o seu nível de permissões

Em primeiro lugar, tem de ter permissões suficientes na sua subscrição do Azure e no Azure Active Directory. Tem de poder criar uma aplicação no Active Directory e atribuir uma função ao principal de serviço.

A forma mais fácil de verificar se a sua conta tem permissões adequadas é utilizar o portal. Veja [Verificar as permissões necessárias no portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions).

## <a name="create-a-service-principal-for-your-app"></a>Criar um principal de serviço para a sua aplicação

Quando tiver iniciado sessão na sua conta do Azure, pode criar o principal de serviço. Tem de ter um dos seguintes modos de identificação da sua aplicação implementada:

* O nome exclusivo da aplicação implementada, tal como "MyDemoWebApp" nos exemplos, ou
* o ID da Aplicação, o GUID exclusivo associado à sua aplicação implementada, serviço ou objeto

### <a name="get-information-about-your-application"></a>Obter informações sobre a sua aplicação

O cmdlet `Get-AzureRmADApplication` pode servir para obter informações sobre a aplicação.

```azurepowershell-interactive
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

### <a name="create-a-service-principal-for-your-application"></a>Criar um principal de serviço para a sua aplicação

O cmdlet `New-AzureRmADServicePrincipal` é utilizado para criar o principal de serviço.

```azurepowershell-interactive
$servicePrincipal = New-AzureRmADServicePrincipal -ApplicationId 00c01aaa-1603-49fc-b6df-b78c4e5138b4
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

A partir daqui, pode ou utilizar diretamente a propriedade $servicePrincipal.Secret em Connect-AzureRmAccount (veja "Iniciar sessão com o principal de serviço" abaixo) ou pode converter esta SecureString numa cadeia de carateres de texto simples para utilização posterior:

```azurepowershell-interactive
$BSTR = [System.Runtime.InteropServices.Marshal]::SecureStringToBSTR($servicePrincipal.Secret)
$password = [System.Runtime.InteropServices.Marshal]::PtrToStringAuto($BSTR)
[Runtime.InteropServices.Marshal]::ZeroFreeBSTR($BSTR)
```

### <a name="sign-in-using-the-service-principal"></a>Iniciar sessão com o principal de serviço

Agora pode iniciar sessão como o novo principal de serviço para a sua aplicação com o *appId* que forneceu e a *palavra-passe* que gerada automaticamente. Também vai precisar do ID de Inquilino para o principal de serviço. O ID do Inquilino é apresentado ao iniciar sessão no Azure com as suas credenciais pessoais. Para iniciar sessão com um principal de serviço, utilize os comandos seguintes:

```azurepowershell-interactive
$cred = New-Object System.Management.Automation.PSCredential ("00c01aaa-1603-49fc-b6df-b78c4e5138b4", $servicePrincipal.Secret)
Connect-AzureRmAccount -Credential $cred -ServicePrincipal -TenantId XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
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

* [Get-AzureRmRoleAssignment](/powershell/module/azurerm.resources/get-azurermroleassignment)
* [New-AzureRmRoleAssignment](/powershell/module/azurerm.resources/new-azurermroleassignment)
* [Remove-AzureRmRoleAssignment](/powershell/module/azurerm.resources/remove-azurermroleassignment)

A função predefinida dos principais de serviço é **Contribuinte**. Pode não ser a melhor opção consoante o âmbito das interações da sua aplicação com os serviços do Azure, dadas as suas amplas permissões.
A função **Leitor** é mais restritiva e é uma boa escolha para aplicações só de leitura. Pode ver detalhes de permissões específicas de funções ou criar permissões personalizadas através do portal do Azure.

Neste exemplo, adicionámos a função **Leitor** ao exemplo anterior e eliminámos a função **Contribuinte**:

```azurepowershell-interactive
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

```azurepowershell-interactive
Remove-AzureRmRoleAssignment -ResourceGroupName myRG -ObjectId 698138e7-d7b6-4738-a866-b4e3081a69e4 -RoleDefinitionName Contributor
```

Para ver as funções atuais atribuídas:

```azurepowershell-interactive
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

Outros cmdlets do Azure PowerShell para gestão de funções:

* [Get-AzureRmRoleDefinition](/powershell/module/azurerm.resources/Get-AzureRmRoleDefinition)
* [New-AzureRmRoleDefinition](/powershell/module/azurerm.resources/New-AzureRmRoleDefinition)
* [Remove-AzureRmRoleDefinition](/powershell/module/azurerm.resources/Remove-AzureRmRoleDefinition)
* [Set-AzureRmRoleDefinition](/powershell/module/azurerm.resources/Set-AzureRmRoleDefinition)

## <a name="change-the-credentials-of-the-security-principal"></a>Alterar as credenciais do principal de segurança

Rever as permissões e atualizar a palavra-passe regularmente é uma boa prática de segurança. Também pode ser útil gerir e modificar as credenciais de segurança à medida que a sua aplicação sofre alterações. Por exemplo, podemos alterar a palavra-passe do principal de serviço ao criar uma nova palavra-passe e ao remover a antiga.

### <a name="add-a-new-password-for-the-service-principal"></a>Adicionar uma nova palavra-passe para o principal de serviço

```azurepowershell-interactive
New-AzureRmADSpCredential -ServicePrincipalName http://MyDemoWebApp
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
Get-AzureRmADSpCredential -ServicePrincipalName http://MyDemoWebApp
```

```output
StartDate           EndDate             KeyId                                Type
---------           -------             -----                                ----
3/8/2017 5:58:24 PM 3/8/2018 5:58:24 PM 6f801c3e-6fcd-42b9-be8e-320b17ba1d36 Password
5/5/2016 4:55:27 PM 5/5/2017 4:55:27 PM ca9d4846-4972-4c70-b6f5-a4effa60b9bc Password
```

### <a name="remove-the-old-password-from-the-service-principal"></a>Remover a palavra-passe antiga do principal de serviço

```azurepowershell-interactive
Remove-AzureRmADSpCredential -ServicePrincipalName http://MyDemoWebApp -KeyId ca9d4846-4972-4c70-b6f5-a4effa60b9bc
```

```output
Confirm
Are you sure you want to remove credential with keyId '6f801c3e-6fcd-42b9-be8e-320b17ba1d36' for
service principal objectId '698138e7-d7b6-4738-a866-b4e3081a69e4'.
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

### <a name="verify-the-list-of-credentials-for-the-service-principal"></a>Verificar a lista de credenciais para o principal de serviço

```azurepowershell-interactive
Get-AzureRmADSpCredential -ServicePrincipalName http://MyDemoWebApp
```

```output
StartDate           EndDate             KeyId                                Type
---------           -------             -----                                ----
3/8/2017 5:58:24 PM 3/8/2018 5:58:24 PM 6f801c3e-6fcd-42b9-be8e-320b17ba1d36 Password
```

### <a name="get-information-about-the-service-principal"></a>Obter informações sobre o principal de serviço

```azurepowershell-interactive
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
