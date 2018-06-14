---
title: Iniciar sessão com o Azure PowerShell
description: Iniciar sessão com o Azure PowerShell
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2017
ms.openlocfilehash: f2a9247d442229b7323e5a9195c7257e45d58e56
ms.sourcegitcommit: c98e3a21037ebd82936828bcb544eed902b24212
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/08/2018
ms.locfileid: "34854346"
---
# <a name="log-in-with-azure-powershell"></a>Iniciar sessão com o Azure PowerShell

O Azure PowerShell suporta vários métodos de início de sessão. A forma mais simples de começar é iniciar sessão interativamente na linha de comandos.

## <a name="interactive-log-in"></a>Início de sessão interativo

1. Digite `Login-AzureRmAccount`. Obterá uma caixa de diálogo a solicitar as suas credenciais do Azure.

2. Escreva o endereço de e-mail e a palavra-passe associados à sua conta. O Azure autentica e guarda as informações das credenciais e, em seguida, fecha a janela.

## <a name="log-in-with-a-service-principal"></a>Iniciar sessão com um principal de serviço

Os principais de serviço proporcionam uma forma de criar contas não interativas que pode ser utilizar para manipular recursos. Os principais de serviço são como contas de utilizador às quais pode aplicar regras com o Azure Active Directory. Ao conceder as permissões mínimas necessárias para um principal de serviço, pode garantir que os seus scripts de automatização estão ainda mais protegidos.

1. Se ainda não tiver um principal de serviço, [crie-o](create-azure-service-principal-azureps.md).

2. Inicie sessão com o principal de serviço.

    ```powershell
    Login-AzureRmAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
    ```

    Para obter o seu T, inicie sessão interativamente e obtenha o TenantId da sua subscrição.

    ```powershell
    Get-AzureRmSubscription
    ```

    ```
    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Production Subscription
    CurrentStorageAccount :
    ```

### <a name="log-in-using-an-azure-vm-managed-service-identity"></a>Iniciar sessão com uma Identidade do Serviço Gerido de VM do Azure

Identidade do Serviço Gerido (MSI) é uma funcionalidade de pré-visualização do Azure Active Directory. Pode utilizar um principal de serviço do MSI para início de sessão e adquirir um token de acesso só de aplicação para aceder a outros recursos.

Para obter mais informações sobre o MSI, veja [Como utilizar uma Identidade do Serviço Gerido de VM (MSI) do Azure para início de sessão e aquisição de token](/azure/active-directory/msi-how-to-get-access-token-using-msi).

## <a name="log-in-to-another-cloud"></a>Inicie sessão noutra Cloud

Os serviços cloud do Azure fornecem diferentes ambientes que aderem aos regulamentos de processamento de dados de várias administrações públicas. Se a sua conta do Azure é de uma das clouds de administração pública, tem de especificar o ambiente quando iniciar sessão. Por exemplo, se a sua conta está na cloud da China, inicia sessão com o seguinte comando:

```powershell
Login-AzureRmAccount -EnvironmentName AzureChinaCloud
```

Utilize o seguinte comando para obter uma lista de ambientes disponíveis:

```powershell
Get-AzureRmEnvironment | Select-Object Name
```

```
Name
----
AzureCloud
AzureChinaCloud
AzureUSGovernment
AzureGermanCloud
```

## <a name="learn-more-about-managing-azure-role-based-access"></a>Saiba mais sobre como gerir o acesso baseado em funções do Azure

Para obter mais informações sobre a gestão de autenticação e de subscrições do Azure, veja [Gerir Contas, Subscrições e Funções Administrativas](/azure/active-directory/role-based-access-control-configure).

Cmdlets do Azure PowerShell para gestão de funções

* [Get-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/Get-AzureRmRoleAssignment)
* [Get-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/Get-AzureRmRoleDefinition)
* [New-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/New-AzureRmRoleAssignment)
* [New-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/New-AzureRmRoleDefinition)
* [Remove-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleAssignment)
* [Remove-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleDefinition)
* [Set-AzureRmRoleDefinition](/powershell/moduel/AzureRM.Resources/Set-AzureRmRoleDefinition)
