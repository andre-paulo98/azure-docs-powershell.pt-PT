---
title: Apresentação do módulo do Azure PowerShell Az
description: Apresentação do novo módulo do Azure PowerShell Az, a substituição do módulo AzureRM.
ms.date: 11/07/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: b0f31341d4344bdac5b4d657a1f66acfd9984dda
ms.sourcegitcommit: 4afdba3cd7e1d348876ce59f3503fdcd258f79ab
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/15/2018
ms.locfileid: "51574809"
---
# <a name="introducing-the-new-azure-powershell-az-module"></a>Apresentação do novo módulo do Azure PowerShell Az

A partir de novembro de 2018, o módulo do Azure PowerShell `Az` está disponível para pré-visualização pública completa.
O Az disponibiliza comandos mais curtos, maior estabilidade e suporta Windows, macOS e Linux. O Az também oferece paridade de funcionalidades e um caminho de migração fácil a partir do AzureRM.

O Az utiliza a biblioteca .NET Standard, o que significa que é executada no PowerShell 5.x e no PowerShell 6.x.
Dado que o PowerShell 6.x pode ser executado em Linux, macOS e Windows, o Az está disponível para todas as plataformas.
A utilização do .NET Standard permite-nos unificar a base de código do Azure PowerShell com o mínimo impacto nos utilizadores.

O Az é um módulo novo, pelo que a versão foi reposta. A primeira versão estável será 1.0, mas o módulo tem paridade de funcionalidades com o AzureRm a partir de novembro de 2018.

## <a name="upgrade-to-az"></a>Atualizar para Az

Recomenda-se que os utilizadores atualizem para o novo módulo do `Az`. Para tal:

* [Desinstalar o módulo do Azure PowerShell AzureRM](/powershell/azure/uninstall-azurerm-ps)
* [Instalar o módulo do Azure PowerShell Az](/powershell/azure/install-az-ps)
* Ative o modo de compatibilidade para o AzureRM com `Enable-AzureRMAlias`, enquanto se familiariza com o novo conjunto de comandos.

## <a name="migrate-existing-scripts-to-az"></a>Migrar scripts existentes para o Az

As atualizações importantes podem ser inconvenientes. No entanto, o módulo `Az` tem um modo de compatibilidade para o ajudar a utilizar os scripts existentes enquanto trabalha em atualizações para a nova sintaxe. Utilize o cmdlet `Enable-AzureRmAlias` para ativar o modo de compatibilidade `AzureRM`. Este cmdlet define nomes de cmdlet `AzureRM` como aliases para os novos nomes de cmdlet `Az`.

Os novos nomes de cmdlet foram criados para serem fáceis de aprender. Em vez de utilizar `AzureRm` ou `Azure` em nomes de cmdlet, utilize `Az`. Por exemplo, o comando antigo `New-AzureRmVm` tornou-se `New-AzVm`.

Para obter uma descrição completa do processo de migração, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).

## <a name="the-future-of-support-for-azurerm"></a>O futuro do suporte para o AzureRM

A módulo `AzureRM` atual deixará de receber novos cmdlets ou funcionalidades quando a versão 1.0 `Az` for lançada em dezembro de 2018. No entanto, `AzureRM` ainda é oficialmente mantida e irá obter as correções de erros. Para se manter atualizado com os mais recentes serviços e funcionalidades do Azure, deve trocar para o módulo `Az`.