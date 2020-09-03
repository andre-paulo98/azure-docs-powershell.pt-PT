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
ms.locfileid: "89239388"
---
# <a name="frequently-asked-questions-about-azure-powershell"></a>Perguntas mais frequentes sobre o Azure PowerShell

## <a name="what-is-azure-powershell"></a>O que é o Azure PowerShell?

O Azure PowerShell é um conjunto de cmdlets que lhe permite gerir os recursos do Azure diretamente com o PowerShell. Em dezembro de 2018, o módulo Az do PowerShell entrou em disponibilidade geral. É agora o módulo do PowerShell recomendado para interagir com o Azure. Para saber mais sobre o módulo Az do PowerShell, veja [Apresentação do novo módulo Az do Azure PowerShell](/powershell/azure/new-azureps-module-az).

## <a name="how-do-i-disable-breaking-change-warning-messages-in-azure-powershell"></a>Como desativo mensagens de aviso de alteração interruptiva no Azure PowerShell?

Para suprimir as mensagens de aviso de alteração interruptiva no Azure PowerShell, terá de definir a variável de ambiente `SuppressAzurePowerShellBreakingChangeWarnings` como `true`.

```azurepowershell
Set-Item -Path Env:\SuppressAzurePowerShellBreakingChangeWarnings -Value $true
```
