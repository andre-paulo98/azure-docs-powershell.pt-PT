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
# <a name="create-an-azure-service-principal-with-azure-powershell"></a>Criar um principal de serviço do Azure com o Azure PowerShell

As ferramentas automatizadas que utilizam serviços do Azure devem ter sempre permissões restritas. Em vez de obrigar as aplicações a iniciarem sessão como um utilizador com privilégios máximos, o Azure disponibiliza principais de serviço.

Um principal de serviço do Azure é uma identidade criada para ser utilizada com aplicações, serviços alojados e ferramentas automatizadas para aceder aos recursos do Azure. Este acesso é restringido pelas funções atribuídas ao principal de serviço, o que lhe permite assumir o controlo dos recursos que podem ser acedidos e em que nível. Por motivos de segurança, é sempre recomendado utilizar os principais de serviço com ferramentas automatizadas, em vez de permitir que iniciem sessão com uma identidade de utilizador.

Este artigo mostra-lhe os passos para criar, obter informações e repor um principal de serviço com o Azure PowerShell.

## <a name="create-a-service-principal"></a>Criar um principal de serviço

Crie um principal de serviço com o cmdlet [New-AzADServicePrincipal](/powershell/module/Az.Resources/New-AzADServicePrincipal). Quando cria um principal de serviço, escolhe o tipo de autenticação de início de sessão que o mesmo utiliza.

> [!NOTE]
>
> Se a sua conta não tiver permissão para criar um principal de serviço, o cmdlet `New-AzADServicePrincipal` devolve uma mensagem de erro com a indicação "Privilégios insuficientes para concluir a operação". Contacte o seu administrador do Azure Active Directory para criar um principal de serviço.

Existem dois tipos de autenticação disponíveis para os principais de serviço: a autenticação baseada em palavra-passe e a autenticação baseada em certificado.

### <a name="password-based-authentication"></a>Autenticação baseada em palavra-passe

Na ausência de outros parâmetros de autenticação, a autenticação baseada em palavra-passe é utilizada e é criada uma palavra-passe aleatória para si. Se estiver interessado na autenticação baseada em palavra-passe, este é o método recomendado.

```azurepowershell-interactive
$sp = New-AzADServicePrincipal -DisplayName ServicePrincipalName
```

O objeto devolvido contém o membro `Secret`, ou seja, uma `SecureString` que contém a palavra-passe gerada. Certifique-se de que armazena este valor num local seguro para efetuar a autenticação com o principal de serviço. O respetivo valor __não será__ apresentado na saída da consola. Se perder a palavra-passe, [reponha as credenciais do principal de serviço](#reset-credentials). 

Para as palavras-passe fornecidas pelo utilizador, o argumento `-PasswordCredential` aceita objetos `Microsoft.Azure.Commands.ActiveDirectory.PSADPasswordCredential`. Estes objetos têm de ter uma `StartDate` e uma `EndDate` válidas, bem como aceitar uma `Password` com texto desencriptado. Quando criar uma palavra-passe, certifique-se de que segue as [regras e restrições de palavra-passe do Azure Active Directory](/azure/active-directory/active-directory-passwords-policy). Não utilize uma palavra-passe fraca nem reutilize uma palavra-passe.

```azurepowershell-interactive
Import-Module Az.Resources # Imports the PSADPasswordCredential object
$credentials = New-Object Microsoft.Azure.Commands.ActiveDirectory.PSADPasswordCredential -Property @{ StartDate=Get-Date; EndDate=Get-Date -Year 2024; Password=<Choose a strong password>}
$sp = New-AzAdServicePrincipal -DisplayName ServicePrincipalName -PasswordCredential $credentials
```

O objeto devolvido a partir de `New-AzADServicePrincipal` contém os membros `Id` e `DisplayName`, que podem ser utilizados para iniciar sessão com o principal de serviço.

> [!IMPORTANT]
>
> Iniciar sessão com um principal de serviço necessita do ID de inquilino no qual o principal de serviço foi criado. Para obter o inquilino que estava ativo quando o principal de serviço foi criado, execute o seguinte comando __imediatamente após__ a criação do principal de serviço:
>
> ```azurepowershell-interactive
> (Get-AzContext).Tenant.Id
> ```

### <a name="certificate-based-authentication"></a>Autenticação baseada em certificado

Os principais de serviço que utilizam a autenticação baseada em certificado são criados com o parâmetro `-CertValue`. Este parâmetro aceita uma cadeia ASCII codificada em base64 do certificado público. Isto é representado por um ficheiro PEM, ou por um CRT ou CER codificado em texto. Não são suportadas codificações binárias do certificado público. Estas instruções partem do princípio de que já tem um certificado disponível.

```azurepowershell-interactive
$cert = <public certificate as base64-encoded string>
$sp = New-AzADServicePrincipal -DisplayName ServicePrincipalName -CertValue $cert
```

Também pode utilizar o parâmetro `-KeyCredential`, que aceita objetos `PSADKeyCredential`. Estes objetos têm de ter uma `StartDate` e uma `EndDate` válidas, e têm de ter o membro `CertValue` definido como uma cadeia ASCII codificada em base64 do certificado público.

```azurepowershell-interactive
$cert = <public certificate as base64-encoded string>
$credentials = New-Object Microsoft.Azure.Commands.ActiveDirectory.PSADKeyCredential -Property @{ StartDate=Get-Date; EndDate=Get-Date -Year 2024; KeyId=New-Guid; CertValue=$cert}
$sp = New-AzADServicePrincipal -DisplayName ServicePrincipalName -KeyCredential $credentials
```

O objeto devolvido a partir de `New-AzADServicePrincipal` contém os membros `Id` e `DisplayName`, que podem ser utilizados para iniciar sessão com o principal de serviço. Os clientes que iniciam sessão com o principal de serviço também precisam de acesso à chave privada do certificado.

> [!IMPORTANT]
>
> Iniciar sessão com um principal de serviço necessita do ID de inquilino no qual o principal de serviço foi criado. Para obter o inquilino que estava ativo quando o principal de serviço foi criado, execute o seguinte comando __imediatamente após__ a criação do principal de serviço:
>
> ```azurepowershell-interactive
> (Get-AzContext).Tenant.Id
> ```

## <a name="get-an-existing-service-principal"></a>Obter um principal de serviço existente

É possível obter uma lista de principais de serviço do inquilino atualmente ativo com [Get-AzADServicePrincipal](/powershell/module/az.resources/get-azadserviceprincipal). Por predefinição, este comando devolve __todos__ os principais de serviço de um inquilino, pelo que a devolução dos resultados pode ser muito demorada para as organizações de grande dimensão. Em alternativa, recomenda-se a utilização de um dos argumentos de filtragem opcionais do lado do servidor:

* `-DisplayNameBeginsWith` pede principais de serviço que tenham um _prefixo_ correspondente ao valor fornecido. O nome a apresentar de um principal de serviço é o valor definido com `-DisplayName` durante a criação.
* `-DisplayName` pede uma _correspondência exata_ de um nome do principal do serviço.

## <a name="manage-service-principal-roles"></a>Gerir funções de principais de serviço

O Azure PowerShell dispõe dos seguintes cmdlets para gerir as atribuições de funções:

* [Get-AzRoleAssignment](/powershell/module/az.resources/get-azroleassignment)
* [New-AzRoleAssignment](/powershell/module/az.resources/new-azroleassignment)
* [Remove-AzRoleAssignment](/powershell/module/az.resources/remove-azroleassignment)

A função predefinida dos principais de serviço é **Contribuinte**. Esta função tem permissões completas para ler e escrever numa conta do Azure. A função **Leitor** é mais restritiva, com acesso só de leitura.  Para obter mais informações sobre o Controlo de Acesso Baseado em Funções (RBAC) e as funções, veja [RBAC: Funções incorporadas](/azure/active-directory/role-based-access-built-in-roles).

Este exemplo adiciona a função **Leitor** e remove a função **Contribuidor**:

```azurepowershell-interactive
New-AzRoleAssignment -ApplicationId <service principal application ID> -RoleDefinitionName "Reader"
Remove-AzRoleAssignment -ApplicationId <service principal application ID> -RoleDefinitionName "Contributor"
```

> [!IMPORTANT]
> Os cmdlets de atribuição de funções não aceitam o ID do objeto do principal de serviço. Aceitam o ID da aplicação associada, gerado no momento da criação. Para obter o ID da aplicação de um principal de serviço, utilize `Get-AzADServicePrincipal`.

> [!NOTE]
> Se a sua conta não tiver permissão para atribuir uma função, ser-lhe-á apresentada uma mensagem de erro com a indicação de que a sua conta "não tem autorização para realizar a ação 'Microsoft.Authorization/roleAssignments/write'". Contacte o administrador do Azure Active Directory para gerir funções.

Adicionar uma função _não_ restringe as permissões atribuídas anteriormente. Quando restringir as permissões de um principal de serviço, a função __Contribuidor__ deve ser removida.

As alterações podem ser verificadas ao listar as funções atribuídas:

```azurepowershell-interactive
Get-AzRoleAssignment -ServicePrincipalName ServicePrincipalName
```

## <a name="sign-in-using-a-service-principal"></a>Iniciar sessão com um principal de serviço

Teste as credenciais e permissões do novo principal de serviço iniciando sessão. Para iniciar sessão com um principal de serviço, precisa do valor `applicationId` associado ao mesmo, bem como do inquilino em que foi criado.

Para iniciar sessão com um principal de serviço através de uma palavra-passe:

```azurepowershell-interactive
# Use the application ID as the username, and the secret as password
$credentials = Get-Credential
Connect-AzAccount -ServicePrincipal -Credential $credentials -Tenant <tenant ID> 
```

A autenticação baseada em certificado precisa que o Azure PowerShell tenha a capacidade de obter informações de um arquivo de certificados local com base num thumbprint do certificado.

```azurepowershell-interactive
Connect-AzAccount -ServicePrincipal -TenantId $tenantId -CertificateThumbprint <thumbprint>
```

Para obter instruções sobre como importar um certificado para um arquivo de credenciais acessível ao PowerShell, veja [Sign in with Azure PowerShell](authenticate-azureps.md#sp-signin) (Iniciar sessão com o Azure PowerShell)

## <a name="reset-credentials"></a>Repor credenciais

Se se esquecer das credenciais de um principal de serviço, utilize [New-AzADSpCredential](/powershell/module/az.resources/new-azadspcredential) para adicionar uma credencial nova. Este cmdlet aceita os mesmos tipos e argumentos de credencial que `New-AzADServicePrincipal`. Na ausência de argumentos de credencial, é criada uma nova `PasswordCredential` com uma palavra-passe aleatória.

> [!IMPORTANT]
> Antes de atribuir credenciais novas, convém remover as credenciais existentes para evitar iniciar sessão com as mesmas. Para tal, utilize o cmdlet [Remove-AzADSpCredential](/powershell/module/az.resources/remove-azadspcredential):
>
> ```azurepowershell-interactive
> Remove-AzADSpCredential -DisplayName ServicePrincipalName
> ```

```azurepowershell-interactive
$newCredential = New-AzADSpCredential -ServicePrincipalName ServicePrincipalName
```
