---
title: Iniciar sessão com o Azure PowerShell
description: Como iniciar sessão com o Azure PowerShell como um utilizador, principal de serviço ou com identidades geridas para recursos do Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/29/2018
ms.openlocfilehash: 80c59a10666c6e3a01e6c33716fce40094fb14be
ms.sourcegitcommit: 2054a8f74cd9bf5a50ea7fdfddccaa632c842934
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "56145269"
---
# <a name="sign-in-with-azure-powershell"></a>Iniciar sessão com o Azure PowerShell

O Azure PowerShell suporta vários métodos de autenticação. O [Azure Cloud Shell](/azure/cloud-shell/overview) é a forma mais fácil de começar, uma vez que regista automaticamente o utilizador. Com uma instalação local, pode iniciar sessão interativamente através do browser. Ao escrever scripts para automatização, a abordagem recomendada é utilizar um [principal de serviço](create-azure-service-principal-azureps.md) com as permissões necessárias. Ao restringir as permissões de início de sessão tanto quanto possível para o seu caso de utilização, ajuda a manter os recursos do Azure seguros.

Depois de iniciar sessão, os comandos são executados na sua subscrição predefinida. Para alterar a subscrição ativa para uma sessão, utilize o cmdlet [Set-AzContext](/powershell/module/az.accounts/set-azcontext). Para alterar a subscrição predefinida utilizada ao iniciar sessão com o Azure PowerShell, utilize [Set-AzDefault](/powershell/module/az.accounts/set-azdefault).

> [!IMPORTANT]
>
> As suas credenciais são partilhadas entre várias sessões do PowerShell, desde que mantenha a sessão iniciada.
> Para obter mais informações, veja o artigo sobre [Credenciais Persistentes](context-persistence.md).

## <a name="sign-in-interactively"></a>Iniciar sessão interativamente

Para iniciar sessão interativamente, utilize o cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).

```azurepowershell-interactive
Connect-AzAccount
```

Quando é executado, este cmdlet apresenta uma cadeia de token. Para iniciar sessão, copie esta cadeia e cole-a em https://microsoft.com/devicelogin num browser. A sua sessão do PowerShell será autenticada para se ligar ao Azure.

## <a name="sign-in-with-credentials"></a>Iniciar sessão com credenciais

Também pode iniciar sessão com um objeto `PSCredential` autorizado para ligar ao Azure.
A maneira mais fácil de obter um objeto de credencial é com o cmdlet [Get-Credential](/powershell/module/Microsoft.PowerShell.Security/Get-Credential). Quando é executado, este cmdlet vai solicitar-lhe um par de credenciais nome de utilizador/palavra-passe.

> [!Note]
> Esta abordagem não funciona em contas Microsoft nem em contas que tenham a autenticação multifator ativada.

```azurepowershell-interactive
$creds = Get-Credential
Connect-AzAccount -Credential $creds
```

## <a name="sign-in-with-a-service-principal"></a>Iniciar sessão com um principal de serviço

Os principais de serviço são contas não interativas do Azure. Como outras contas de utilizador, as respetivas permissões são geridas com o Azure Active Directory. Ao conceder a um principal de serviço apenas as permissões de que aquele precisa, os seus scripts de automatização permanecem seguros.

Para saber como criar um principal de serviço para utilizar com o Azure PowerShell, veja [Criar um principal de serviço do Azure com o Azure PowerShell](create-azure-service-principal-azureps.md).

Para iniciar sessão com um principal de serviço, utilize o argumento `-ServicePrincipal` com o cmdlet `Connect-AzAccount`. Também vai precisar do ID de aplicação do principal de serviço, das credenciais de início de sessão e da associação do ID de inquilino ao principal de serviço. Para obter as credenciais do principal de serviço como o objeto adequado, utilize o cmdlet [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential). Este cmdlet vai apresentar uma linha de comandos para o ID e a palavra-passe de utilizador do principal de serviço.

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
```

## <a name="sign-in-using-a-managed-identity"></a>Iniciar sessão com uma identidade gerida 

As identidades geridas são uma funcionalidade do Azure Active Directory. As identidades geridas são principais de serviço atribuídos aos recursos que são executados no Azure. Pode utilizar um principal de serviço da identidade gerida para início de sessão e adquirir um token de acesso só de aplicação para aceder a outros recursos. As identidades geridas só estão disponíveis em recursos em execução numa cloud do Azure.

Para saber mais sobre identidades geridas para recursos do Azure, veja [Como utilizar identidades geridas para recursos do Azure numa VM do Azure para adquirir um token de acesso](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).

## <a name="sign-in-with-a-non-default-tenant-or-as-a-cloud-solution-provider-csp"></a>Iniciar sessão com um inquilino não predefinido ou como um Fornecedor de Soluções Cloud (CSP)

Se a sua conta estiver associada a mais do que um inquilino, o início de sessão requer a utilização do parâmetro `-TenantId` durante a ligação. Este parâmetro irá funcionar com qualquer outro método de início de sessão. Quando iniciar sessão, o valor deste parâmetro pode ser o ID de objeto do Azure do inquilino (ID de Inquilino) ou o nome de domínio completamente qualificado do inquilino.

Se for um [Fornecedor de Soluções Cloud (CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/), o valor `-TenantId` **tem** de ser um ID de inquilino.

```azurepowershell-interactive
Connect-AzAccount -TenantId 'xxxx-xxxx-xxxx-xxxx'
```

## <a name="sign-in-to-another-cloud"></a>Iniciar sessão noutra Cloud

Os serviços cloud do Azure oferecem ambientes em conformidade com as leis de processamento de dados regionais.
Para as contas numa cloud regional, defina o ambiente quando iniciar sessão com o argumento `-Environment`.
Por exemplo, se a sua conta está na cloud da China:

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

O comando seguinte obtém uma lista dos ambientes disponíveis:

```azurepowershell-interactive
Get-AzEnvironment | Select-Object Name
```