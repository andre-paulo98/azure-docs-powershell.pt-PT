---
title: Apresentação do módulo do Azure PowerShell Az
description: Apresentação do novo módulo do Azure PowerShell Az, a substituição do módulo AzureRM.
ms.date: 05/20/2020
ms.devlang: powershell
ms.topic: conceptual
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: 29b8fc24c468ad542a109042df552cbd45a9f3b2
ms.sourcegitcommit: 8b3126b5c79f453464d90669f0046ba86b7a3424
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/01/2020
ms.locfileid: "89238817"
---
# <a name="introducing-the-new-azure-powershell-az-module"></a>Apresentação do novo módulo do Azure PowerShell Az

Desde dezembro de 2018, o módulo do Az do Azure PowerShell é uma versão de disponibilidade geral e é agora o módulo indicado do PowerShell para interagir com o Azure. O Az oferece comandos mais curtos, maior estabilidade e suporte para várias plataformas. O Az também tem paridade de funcionalidades com o AzureRM, o que lhe oferece um caminho de migração fácil.

> [!NOTE]
> A versão recomendada do PowerShell para utilização com o Azure PowerShell em todas as plataformas é o PowerShell 7.x e posteriores.

Com o módulo do Az mais recente, o Azure PowerShell funciona bem com o PowerShell 6.x e posterior em todas as plataformas, incluindo Windows, macOS e Linux. Também é compatível com o PowerShell 5.1 no Windows.

O Az é um módulo novo, pelo que a versão foi reposta para 1.0.0.

## <a name="why-a-new-module"></a>Por quê um novo módulo?

As principais atualizações podem ser inconvenientes, pelo que é importante informá-lo das razões que nos levaram a optar por introduzir um novo conjunto de módulos, com novos cmdlets, para interagir com o Azure a partir do PowerShell.

A alteração mais importante e mais significativa é que o PowerShell tem sido um produto compatível com várias plataformas desde o lançamento do [PowerShell](/powershell/scripting/overview), com base na biblioteca do .NET Standard.
Assumimos o compromisso de levar o suporte do Azure a todas as plataformas e, para isso, os módulos do Azure PowerShell tinham de ser atualizados para utilizar o .NET Standard e ser compatíveis com o PowerShell Core. Em vez de introduzirmos alterações complexas ao módulo AzureRM para adicionar este suporte, criámos o módulo Az.

A criação de um novo módulo também permitiu que os nossos engenheiros garantam a consistência da estruturação e da nomenclatura dos cmdlets e dos módulos. Agora, todos os módulos começam com o prefixo `Az.` e todos os cmdlets utilizam a forma _Verbo_-`Az`_Substantivo_. Anteriormente, os nomes dos cmdlets não só eram mais longos, como os nomes tinham mais inconsistências.

O número de módulos também foi reduzido: Alguns módulos que funcionavam com os mesmos serviços foram agregados. Os cmdlets de plano de gestão e de plano de dados estão agora dentro de módulos individuais nos respetivos serviços. Para quem faz a gestão manual das dependências e importações, a tarefa torna-se muito mais simples.

Ao levar a cabo estas alterações importantes que exigiram a criação de um novo módulo do Azure PowerShell, a equipa assumiu o compromisso de tornar a utilização do Azure com os cmdlets do PowerShell mais fácil do que nunca e em mais plataformas do que alguma vez foi antes possível.

## <a name="upgrade-to-az"></a>Atualizar para Az

Para se manter a par das mais recentes funcionalidades do Azure no PowerShell, deve migrar para o módulo Az assim que for possível. Se não estiver pronto para instalar o módulo Az como substituto do AzureRM, tem algumas opções disponíveis para experimentar o Az:

- Utilize um ambiente `PowerShell` com o [Azure Cloud Shell](https://docs.microsoft.com/azure/cloud-shell/overview). O Azure Cloud Shell é um ambiente de shell baseado no browser que é fornecido com o módulo do Az instalado e com os aliases de compatibilidade `Enable-AzureRM` ativados.
- Mantenha o módulo do AzureRM instalado com o PowerShell 5.1 para Windows, mas instale o módulo do Az para o PowerShell 6.x ou posterior. O PowerShell 5.1 para Windows e o PowerShell 6.x utilizam coleções separadas de módulos. Siga as instruções para instalar a [versão mais recente do PowerShell](/powershell/scripting/install/installing-powershell) e, em seguida, [instale o módulo do Az](install-az-ps.md) a partir do PowerShell 6.x ou posterior.

Para atualizar a partir de uma instalação existente do AzureRM:

1. [Desinstalar o módulo do Azure PowerShell AzureRM](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module)
2. [Instalar o módulo do Azure PowerShell Az](install-az-ps.md)
3. **OPCIONAL**: Ative o modo de compatibilidade para adicionar aliases para cmdlets do AzureRM com [Enable-AzureRMAlias](/powershell/module/az.accounts/enable-azurermalias) enquanto se familiariza com o novo conjunto de comandos. Veja a secção seguinte ou [Inicie a migração do AzureRM para o Az](migrate-from-azurerm-to-az.md) para obter mais detalhes.

## <a name="migrate-existing-scripts-to-az"></a>Migrar scripts existentes para o Az

Os novos nomes de cmdlet foram criados para serem fáceis de aprender. Em vez de utilizar `AzureRm` ou `Azure` em nomes de cmdlet, utilize `Az`. Por exemplo, o comando antigo `New-AzureRMVm` tornou-se `New-AzVm`.
Contudo, a migração exige mais do que apenas se familiarizar com os novos nomes dos cmdlets: Existem módulos com nomes alterados, parâmetros e outras alterações importantes.

Temos vários recursos que ajudam a iniciar o processo de migração do AzureRM para o Az:

- [Introdução à migração do AzureRM para o Az](migrate-from-azurerm-to-az.md)
- [Lista completa das alterações interruptivas do AzureRM para o Az 1.0.0](migrate-az-1.0.0.md)
- O cmdlet [Enable-AzureRmAlias](/powershell/module/az.accounts/enable-azurermalias)

O módulo Az tem um modo de compatibilidade para o ajudar a utilizar os scripts existentes enquanto atualiza para a nova sintaxe. O cmdlet [Enable-AzureRmAlias](/powershell/module/az.accounts/enable-azurermalias) ativa um modo de compatibilidade através de aliases, para que possa utilizar scripts existentes com alterações mínimas ao mesmo tempo que faz a migração completa para o Az. Por predefinição, o `Enable-AzureRmAlias` só permite aliases de compatibilidade para a sessão atual do PowerShell. Utilize o respetivo parâmetro `Scope` para persistir os aliases de compatibilidade entre as sessões do PowerShell. Para obter mais informações, veja a [documentação de referência de Enable-AzureRmAlias](/powershell/module/az.accounts/enable-azurermalias).

> [!IMPORTANT]
> Embora os nomes dos cmdlets tenham aliases, poderá continuar a existir parâmetros novos (ou com nome alterado) ou valores de retorno alterados dos cmdlets do Az. Não espere que a ativação dos aliases trate da migração por si! Veja a [lista completa de alterações interruptivas](migrate-az-1.0.0.md) para saber onde os seus scripts poderão precisar de atualizações.

## <a name="continued-support-for-azurerm"></a>Suporte contínuo para o AzureRM

O AzureRM deixará de receber novos cmdlets ou funcionalidades. No entanto, o módulo do AzureRM ainda é oficialmente mantido e receberá correções de erros até dezembro de 2020.
