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
ms.openlocfilehash: 2a03697e0f3e80d63c48f2dc5615f6c99b9ef716
ms.sourcegitcommit: 226527be7cb647acfe2ea9ab151185053ab3c6db
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/29/2017
---
# <a name="azure-stack-powershell"></a>Azure Stack do PowerShell 

O Azure Stack requer os seguintes dois módulos do PowerShell:  

1. O módulo**AzureRM** compatível com o Azure Stack que está disponível ao instalar o **2017-03-09-profile** do Perfil da Versão de API. Os cmdlets instalados utilizando este perfil podem ser utilizados por administradores da cloud do Azure Stack e pelos inquilinos. Para saber mais sobre os cmdlets do PowerShell que estão disponíveis neste perfil, veja o conteúdo de referência do PowerShell para a [versão 1.2.9 do módulo do AzureRM](https://docs.microsoft.com/en-us/powershell/azure/overview?view=azurermps-1.2.9).  

2. Versão **1.2.9** módulo do **AzureStack**. Os cmdlets instalados utilizando este módulo apenas podem ser utilizados por administradores da cloud do Azure Stack. Os administrador pode efetuar operações, tais como gerir ofertas, planos, serviços, quotas, etc., utilizando os cmdlets do PowerShell fornecidos por este módulo. Para saber mais sobre os cmdlets do PowerShell disponíveis neste módulo, veja os conteúdos de referência [AzureStackAdmin](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackadmin/?view=azurestackps-1.2.9#azurerm.azurestackadmin) e [AzureStackStorage](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackstorage/?view=azurestackps-1.2.9#azurerm.azurestackstorage).

## <a name="next-steps"></a>Passos Seguintes

* [Instalar o PowerShell para o Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
* [Configurar o PowerShell para utilização com o Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-configure?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)


