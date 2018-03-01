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
ms.openlocfilehash: f895992b4200f260189b3dbc541452e73a377b00
ms.sourcegitcommit: 8446ae373ac6928871ec8f10d3a4918b4601d5b2
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/27/2018
---
# <a name="azure-stack-powershell"></a>Azure Stack do PowerShell

O Azure Stack requer os seguintes dois módulos do PowerShell:  

1. O módulo**AzureRM** compatível com o Azure Stack que está disponível ao instalar o **2017-03-09-profile** do Perfil da Versão de API. Os cmdlets instalados através deste perfil podem ser utilizados por utilizadores e operadores do Azure Stack.

2. A versão mais recente é a instalação **1.2.11** do módulo **AzureStack**. Os cmdlets instalados através deste módulo apenas podem ser utilizados por operadores do Azure Stack. Os operadores podem realizar operações, tais como gerir ofertas, planos, serviços, quotas, etc., através dos cmdlets do PowerShell fornecidos por este módulo. Para saber mais sobre os cmdlets do PowerShell disponíveis neste módulo, veja os conteúdos de referência [AzureStackAdmin](https://docs.microsoft.com/powershell/module/azurerm.azurestackadmin/?view=azurestackps-1.2.11#azurerm.azurestackadmin) e [AzureStackStorage](https://docs.microsoft.com/powershell/module/azurerm.azurestackstorage/?view=azurestackps-1.2.11#azurerm.azurestackstorage).

## <a name="next-steps"></a>Passos Seguintes

* [Instalar o PowerShell para o Azure Stack](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
* [Configurar o PowerShell para utilização com o Azure Stack](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-configure?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
