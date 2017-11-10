---
title: "Descrição geral do Azure Stack do PowerShell | Microsoft Docs"
description: "Descrição geral da instalação e da configuração do Azure Stack do PowerShell."
author: SnehaGunda
manager: Byronr
ms.product: azure-stack
ms.service: powershell
ms.devlang: powershell
ms.topic: reference
ms.author: sngun
ms.manager: byronr
ms.openlocfilehash: 49980b361c580a1a00f07c2002241e71f2c0b654
ms.sourcegitcommit: df44d5d9874b55455ec745f1846e06a4b3266d13
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/06/2017
---
# <a name="azure-stack-powershell"></a>Azure Stack do PowerShell

O Azure Stack requer os seguintes dois módulos do PowerShell:  

1. O módulo**AzureRM** compatível com o Azure Stack que está disponível ao instalar o **2017-03-09-profile** do Perfil da Versão de API. Os cmdlets instalados através deste perfil podem ser utilizados por utilizadores e operadores do Azure Stack.

2. A versão mais recente é a instalação **1.2.11** do módulo **AzureStack**. Os cmdlets instalados através deste módulo apenas podem ser utilizados por operadores do Azure Stack. Os operadores podem realizar operações, tais como gerir ofertas, planos, serviços, quotas, etc., através dos cmdlets do PowerShell fornecidos por este módulo. Para saber mais sobre os cmdlets do PowerShell disponíveis neste módulo, veja os conteúdos de referência [AzureStackAdmin](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackadmin/?view=azurestackps-1.2.11#azurerm.azurestackadmin) e [AzureStackStorage](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackstorage/?view=azurestackps-1.2.11#azurerm.azurestackstorage).

## <a name="next-steps"></a>Passos Seguintes

* [Instalar o PowerShell para o Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
* [Configurar o PowerShell para utilização com o Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-configure?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
