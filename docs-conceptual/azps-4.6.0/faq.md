---
title: Perguntas Frequentes (FAQ)
description: Perguntas Mais Frequentes sobre o Azure PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 08/17/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: b436f00ccef779464a555cd787a9ab0adcc970ce
ms.sourcegitcommit: 8b3126b5c79f453464d90669f0046ba86b7a3424
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/01/2020
ms.locfileid: "89244488"
---
# <a name="frequently-asked-questions-about-azure-powershell"></a><span data-ttu-id="b2013-103">Perguntas mais frequentes sobre o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="b2013-103">Frequently asked questions about Azure PowerShell</span></span>

## <a name="what-is-azure-powershell"></a><span data-ttu-id="b2013-104">O que é o Azure PowerShell?</span><span class="sxs-lookup"><span data-stu-id="b2013-104">What is Azure PowerShell?</span></span>

<span data-ttu-id="b2013-105">O Azure PowerShell é um conjunto de cmdlets que lhe permite gerir os recursos do Azure diretamente com o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b2013-105">Azure PowerShell is a set of cmdlets that allows you to manage Azure resources directly with PowerShell.</span></span> <span data-ttu-id="b2013-106">Em dezembro de 2018, o módulo Az do PowerShell entrou em disponibilidade geral.</span><span class="sxs-lookup"><span data-stu-id="b2013-106">In December 2018, the Az PowerShell module became generally available.</span></span> <span data-ttu-id="b2013-107">É agora o módulo do PowerShell recomendado para interagir com o Azure.</span><span class="sxs-lookup"><span data-stu-id="b2013-107">It's now the recommended PowerShell module for interacting with Azure.</span></span> <span data-ttu-id="b2013-108">Para saber mais sobre o módulo Az do PowerShell, veja [Apresentação do novo módulo Az do Azure PowerShell](/powershell/azure/new-azureps-module-az).</span><span class="sxs-lookup"><span data-stu-id="b2013-108">To learn more about the Az PowerShell module, see [Introducing the new Azure PowerShell Az module](/powershell/azure/new-azureps-module-az).</span></span>

## <a name="how-do-i-disable-breaking-change-warning-messages-in-azure-powershell"></a><span data-ttu-id="b2013-109">Como desativo mensagens de aviso de alteração interruptiva no Azure PowerShell?</span><span class="sxs-lookup"><span data-stu-id="b2013-109">How do I disable breaking change warning messages in Azure PowerShell?</span></span>

<span data-ttu-id="b2013-110">Para suprimir as mensagens de aviso de alteração interruptiva no Azure PowerShell, terá de definir a variável de ambiente `SuppressAzurePowerShellBreakingChangeWarnings` como `true`.</span><span class="sxs-lookup"><span data-stu-id="b2013-110">To suppress the breaking change warning messages in Azure PowerShell, you'll need to set the environment variable `SuppressAzurePowerShellBreakingChangeWarnings` to `true`.</span></span>

```azurepowershell
Set-Item -Path Env:\SuppressAzurePowerShellBreakingChangeWarnings -Value $true
```
