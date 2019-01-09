---
title: Iniciar sessão com o Azure PowerShell
description: Como iniciar sessão com o Azure PowerShell como um utilizador, principal de serviço ou com identidades geridas para recursos do Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/29/2018
ms.openlocfilehash: 8b085720aeabe26c1293ece193e050b31f99a693
ms.sourcegitcommit: ae81b08a45d8729fc8d40156422e3eb2e94de8c7
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/27/2018
ms.locfileid: "53786684"
---
# <a name="sign-in-with-azure-powershell"></a>Iniciar sessão com o Azure PowerShell

O Azure PowerShell suporta vários métodos de autenticação. A forma mais simples de começar é iniciar sessão interativamente na linha de comandos.

## <a name="sign-in-interactively"></a>Iniciar sessão interativamente

Para iniciar sessão interativamente, utilize o cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).

```azurepowershell-interactive
Connect-AzAccount
```

Quando é executado, este cmdlet apresenta uma cadeia de token. Para iniciar sessão, copie essa cadeia e cole-a em https://microsoft.com/devicelogin num browser. A sua sessão do PowerShell é autenticada para se ligar ao Azure. Esta autenticação tem a duração da sessão atual do PowerShell.

> [!IMPORTANT]
>
> As suas credenciais são partilhadas entre várias sessões do PowerShell, desde que mantenha a sessão iniciada.
> Para obter mais informações, veja o artigo sobre [Credenciais Persistentes](context-persistence.md).

## <a name="sign-in-with-a-service-principal"></a>Iniciar sessão com um principal de serviço

Os principais de serviço são contas não interativas do Azure. Como outras contas de utilizador, as respetivas permissões são geridas com o Azure Active Directory. Ao conceder a um principal de serviço apenas as permissões de que aquele precisa, os seus scripts de automatização permanecem seguros.

Para saber como criar um principal de serviço para utilizar com o Azure PowerShell, veja [Criar um principal de serviço do Azure com o Azure PowerShell](create-azure-service-principal-azureps.md).

Para iniciar sessão com um principal de serviço, utilize o argumento `-ServicePrincipal` com o cmdlet `Connect-AzAccount`. Também vai precisar do ID de aplicação do principal de serviço, das credenciais de início de sessão e da associação do ID de inquilino ao principal de serviço. Para obter as credenciais do principal de serviço como o objeto adequado, utilize o cmdlet [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential). Este cmdlet vai apresentar uma linha de comandos para o ID e a palavra-passe de utilizador do principal de serviço.

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
```

## <a name="sign-in-using-an-azure-managed-service-identity"></a>Iniciar sessão com uma Identidade de Serviço Gerida do Azure

As identidades geridas para os recursos do Azure são uma funcionalidade do Azure Active Directory. Pode utilizar um principal de serviço da identidade gerida para início de sessão e adquirir um token de acesso só de aplicação para aceder a outros recursos. As identidades geridas só estão disponíveis em máquinas virtuais em execução numa cloud do Azure.

Para obter mais informações sobre identidades geridas para recursos do Azure, veja [Como utilizar identidades geridas para recursos do Azure numa VM do Azure para adquirir um token de acesso](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).

## <a name="sign-in-as-a-cloud-solution-provider-csp"></a>Iniciar a sessão como um Fornecedor de Soluções Cloud (CSP)

Um início de sessão do [Fornecedor de Soluções Cloud (CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/) requer a utilização de `-TenantId`. Normalmente, este parâmetro pode ser fornecido como um ID de inquilino ou um nome de domínio. No entanto, para o início de sessão de CSP, é preciso fornecer um **ID de inquilino**.

```azurepowershell-interactive
Connect-AzAccount -TenantId 'xxxx-xxxx-xxxx-xxxx'
```

## <a name="sign-in-to-another-cloud"></a>Iniciar sessão noutra Cloud

Os serviços cloud do Azure oferecem ambientes em conformidade com regulamentos de processamento de dados regionais.
Para as contas numa cloud regional, defina o ambiente quando iniciar sessão com o argumento `-Environment`.
Por exemplo, se a sua conta está na cloud da China:

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

O comando seguinte obtém uma lista dos ambientes disponíveis:

```azurepowershell-interactive
Get-AzEnvironment | Select-Object Name
```

## <a name="learn-more-about-managing-azure-role-based-access"></a>Saiba mais sobre como gerir o acesso baseado em funções do Azure

Para obter mais informações sobre a gestão de autenticação e de subscrições do Azure, veja [Gerir Contas, Subscrições e Funções Administrativas](/azure/active-directory/role-based-access-control-configure).

Cmdlets do Azure PowerShell para a gestão de funções:

* [Get-AzRoleAssignment](/powershell/module/az.Resources/Get-azRoleAssignment)
* [Get-AzRoleDefinition](/powershell/module/az.Resources/Get-azRoleDefinition)
* [New-AzRoleAssignment](/powershell/module/az.Resources/New-azRoleAssignment)
* [New-AzRoleDefinition](/powershell/module/az.Resources/New-azRoleDefinition)
* [Remove-AzRoleAssignment](/powershell/module/az.Resources/Remove-azRoleAssignment)
* [Remove-AzRoleDefinition](/powershell/module/az.Resources/Remove-azRoleDefinition)
* [Set-AzRoleDefinition](/powershell/module/az.Resources/Set-azRoleDefinition)
