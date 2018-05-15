---
title: Descrição geral do Azure Stack do PowerShell | Microsoft Docs
description: Descrição geral da instalação e da configuração do Azure Stack do PowerShell.
author: SnehaGunda
manager: Byronr
ms.product: azure-stack
ms.service: powershell
ms.devlang: powershell
ms.topic: reference
ms.author: sngun
ms.manager: byronr
ms.openlocfilehash: f895992b4200f260189b3dbc541452e73a377b00
ms.sourcegitcommit: 37bfbf11fd0967a8e7977c692ab829d286baf88a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/08/2018
---
# <a name="azure-stack-powershell"></a><span data-ttu-id="2fbf7-103">Azure Stack do PowerShell</span><span class="sxs-lookup"><span data-stu-id="2fbf7-103">Azure Stack PowerShell</span></span>

<span data-ttu-id="2fbf7-104">O Azure Stack requer os seguintes dois módulos do PowerShell:</span><span class="sxs-lookup"><span data-stu-id="2fbf7-104">Azure Stack requires the following two PowerShell modules:</span></span>  

1. <span data-ttu-id="2fbf7-105">O módulo**AzureRM** compatível com o Azure Stack que está disponível ao instalar o **2017-03-09-profile** do Perfil da Versão de API.</span><span class="sxs-lookup"><span data-stu-id="2fbf7-105">The Azure Stack compatible **AzureRM** module which is available by installing the **2017-03-09-profile** API Version Profile.</span></span> <span data-ttu-id="2fbf7-106">Os cmdlets instalados através deste perfil podem ser utilizados por utilizadores e operadores do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="2fbf7-106">The cmdlets installed by using this profile can be used by Azure Stack operators and users.</span></span>

2. <span data-ttu-id="2fbf7-107">A versão mais recente é a instalação **1.2.11** do módulo **AzureStack**.</span><span class="sxs-lookup"><span data-stu-id="2fbf7-107">The most current version is the **1.2.11** install of the **AzureStack** module.</span></span> <span data-ttu-id="2fbf7-108">Os cmdlets instalados através deste módulo apenas podem ser utilizados por operadores do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="2fbf7-108">The cmdlets installed by using this module can be used by Azure Stack operators only.</span></span> <span data-ttu-id="2fbf7-109">Os operadores podem realizar operações, tais como gerir ofertas, planos, serviços, quotas, etc., através dos cmdlets do PowerShell fornecidos por este módulo.</span><span class="sxs-lookup"><span data-stu-id="2fbf7-109">Operators can perform operations such as manage offers, plans, services, quotas, etc. by using the PowerShell cmdlets provided by this module.</span></span> <span data-ttu-id="2fbf7-110">Para saber mais sobre os cmdlets do PowerShell disponíveis neste módulo, veja os conteúdos de referência [AzureStackAdmin](https://docs.microsoft.com/powershell/module/azurerm.azurestackadmin/?view=azurestackps-1.2.11#azurerm.azurestackadmin) e [AzureStackStorage](https://docs.microsoft.com/powershell/module/azurerm.azurestackstorage/?view=azurestackps-1.2.11#azurerm.azurestackstorage).</span><span class="sxs-lookup"><span data-stu-id="2fbf7-110">To learn about the PowerShell cmdlets available in this module, see the [AzureStackAdmin](https://docs.microsoft.com/powershell/module/azurerm.azurestackadmin/?view=azurestackps-1.2.11#azurerm.azurestackadmin) and [AzureStackStorage](https://docs.microsoft.com/powershell/module/azurerm.azurestackstorage/?view=azurestackps-1.2.11#azurerm.azurestackstorage) Reference content.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2fbf7-111">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="2fbf7-111">Next Steps</span></span>

* [<span data-ttu-id="2fbf7-112">Instalar o PowerShell para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="2fbf7-112">Install PowerShell for Azure Stack</span></span>](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
* [<span data-ttu-id="2fbf7-113">Configurar o PowerShell para utilização com o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="2fbf7-113">Configure PowerShell for use with Azure Stack</span></span>](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-configure?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
