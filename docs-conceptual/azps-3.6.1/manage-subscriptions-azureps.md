---
title: Gerir subscrições do Azure com o Azure PowerShell
description: Gerir subscrições do Azure com o Azure PowerShell
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 02/04/2019
ms.openlocfilehash: 778fdb463a42b609d3a94c910a2c0f9553ef4eb9
ms.sourcegitcommit: f6fa6543be1e0f6330b1598f01528b2928cc426c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/10/2020
ms.locfileid: "79035860"
---
# <a name="use-multiple-azure-subscriptions"></a>Utilizar várias subscrições do Azure

A maioria dos utilizadores do Azure terão apenas uma única subscrição. No entanto, se fizer parte de várias organizações ou se a sua organização tiver dividido o acesso a determinados recursos entre agrupamentos, pode ter várias subscrições no Azure. A CLI suporta a seleção de uma subscrição tanto a nível global como por comando.

Para obter informações detalhadas sobre subscrições, faturação e gestão de custos, veja a [documentação sobre a gestão da faturação e dos custos](/azure/billing/).

## <a name="tenants-users-and-subscriptions"></a>Inquilinos, utilizadores e subscrições

Poderá surgir alguma confusão sobre a diferença entre inquilinos, utilizadores e subscrições no Azure. Um _inquilino_ é a entidade do Azure Active Directory que abrange uma organização no seu todo. Este inquilino tem, pelo menos, uma _subscrição_ e _utilizador_. Um utilizador é um indivíduo e está associado a apenas um inquilino, a organização a que pertence. Os utilizadores são as contas que iniciam sessão no Azure para criar, gerir e utilizar recursos.
Um utilizador pode ter acesso a várias _subscrições_, que são os contratos com a Microsoft para utilizar serviços cloud, incluindo o Azure. Cada recurso está associado a uma subscrição.

Para saber mais sobre as diferenças entre inquilinos, utilizadores e subscrições, veja o [Azure cloud terminology dictionary (dicionário de terminologia de cloud do Azure)](/azure/azure-glossary-cloud-terminology).  Para saber como adicionar uma nova subscrição ao seu inquilino do Azure Active Directory, veja [How to add an Azure subscription to Azure Active Directory (Como adicionar uma subscrição do Azure ao Azure Active Directory)](/azure/active-directory/active-directory-how-subscriptions-associated-directory).
Para saber como iniciar sessão num inquilino específico, veja [Sign in with Azure PowerShell](/powershell/azure/authenticate-azureps) (Iniciar sessão com o Azure PowerShell).

## <a name="change-the-active-subscription"></a>Alterar a subscrição ativa

No Azure PowerShell, aceder a recursos para uma subscrição exige a alteração da subscrição associada à sua sessão atual do Azure.
Isto é feito ao modificar o contexto da sessão ativa, as informações sobre quais os cmdlets do inquilino, da subscrição e do utilizador devem ser executados.
Para alterar as subscrições, é necessário obter primeiro um objeto de contexto do Azure PowerShell com [Get-AzSubscription](/powershell/module/az.accounts/get-azsubscription) e, em seguida, alterar o contexto atual com [Set-AzContext](/powershell/module/az.accounts/set-azcontext).

O exemplo seguinte mostra como obter uma subscrição no inquilino atualmente ativo e defini-lo como a sessão ativa:

```powershell-interactive
$context = Get-AzSubscription -SubscriptionId ...
Set-AzContext $context
```

Para obter mais informações sobre contextos do Azure PowerShell, incluindo como guardá-los e alternar rapidamente entre os mesmos para utilizar facilmente múltiplas subscrições, veja [Persist credentials with Azure PowerShell contexts](context-persistence.md) (Manter as credenciais nos contextos do Azure PowerShell).
