---
title: Registo de alterações do Azure PowerShell | Microsoft Docs
description: Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente.
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: 04f89e8d47d0825d46cb1b8817efbcc0cafa0acd
ms.sourcegitcommit: 37bfbf11fd0967a8e7977c692ab829d286baf88a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/08/2018
---
# <a name="release-notes"></a>Notas de versão

Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.

## <a name="version-380"></a>Versão 3.8.0
* Computação
  - Correção de erros nos cmdlets Get-*, para permitir a obtenção de várias páginas de dados (mais de 120 itens)
* DataLakeAnalytics
  - Correção da ajuda de alguns comandos para ter o texto e os exemplos adequados.
* DataLakeStore
  - Adição de suporte relativo à parte inicial e final ao cmdlet `Get-AzureRMDataLakeStoreItemContent`. Isto permite a apresentação das linhas delimitadas por nova linha N inicial ou N final.
* HDInsight
  - Foi adicionado suporte para o tipo de cluster RServer
    + O tamanho da VM Edgenode pode ser especificado para o cluster RServer em New-AzureRmHDInsightCluster ou New-AzureRmHDInsightClusterConfig
    + RServer é agora uma opção de configuração em Add-AzureRmHDInsightConfigValues. Permite definir o sinalizador de RStudio para indicar que a instalação do R Studio deve ser executada.
* LogicApp
  - Os cmdlets Set-AzureRmIntegrationAccountSchema e Set-AzureRmIntegrationAccountMap foram corrigidos para o problema de contentlink (content e contentlink estavam definidos, o que resultava numa falha de atualização).
* Rede
  - Foi adicionado suporte para novas funcionalidades de firewall da aplicação Web aos Gateways de Aplicação
    + New-AzureRmApplicationGatewayFirewallDisabledRuleGroupConfig adicionado
    + Get-AzureRmApplicationGatewayAvailableWafRuleSets (Alias: List-AzureRmApplicationGatewayAvailableWafRuleSets) adicionado
    + New-AzureRmApplicationGatewayWebApplicationFirewallConfiguration atualizado: parâmetro adicionado -RuleSetType -RuleSetVersion e -DisabledRuleGroups
    + Set-AzureRmApplicationGatewayWebApplicationFirewallConfiguration atualizado: parâmetro adicionado -RuleSetType -RuleSetVersion e -DisabledRuleGroups
  - Foi adicionado suporte para políticas IPSec às Ligações de Gateway de Rede Virtual
  - New-AzureRmIpsecPolicy adicionado
  - New-AzureRmVirtualNetworkGatewayConnection atualizado: parâmetro adicionado -IpsecPolicies e -UsePolicyBasedTrafficSelectors
* Perfil
  - *Obsoleto*: o nome de Save-AzureRmProfile foi mudado para Save-AzureRmContext; existe um alias para o nome antigo do cmdlet; o alias será removido na próxima versão.
  - *Obsoleto*: o nome de Select-AzureRmProfile foi mudado para Import-AzureRmContext; existe um alias para o nome antigo do cmdlet; o alias será removido na próxima versão.
  - Os tipos de saída PSAzureContext e PSAzureProfile dos cmdlets de perfil vão ser alterados na próxima versão.
  - O cmdlet Save-AzureRmContext não terá qualquer OutputType na próxima versão.
  - Correção de erro no código comum do cmdlet para utilizar o algoritmo compatível com FIPS para hashes de dados: https://github.com/Azure/azure-powershell/issues/3651
* SQL
  - Correções de erros no Cmdlets de Grupo de Ativação Pós-falha do Azure
  - Correção para a consulta de operações
  - Correção do valor GracePeriodWithDataLossHour ao definir FailoverPolicy como Manual
* TrafficManager
  - Suporte para o método de encaminhamento de tráfego Geográfico
    + Novo valor 'Geographic' para o parâmetro TrafficRoutingMethod de New-AzureRmTrafficManagerProfile
    + Novo parâmetro GeoMapping para New-AzureRmTrafficManagerEndpoint e Add-AzureRmTrafficManagerEndpointConfig
    + Correção da tubagem para Get-AzureRmTrafficManagerProfile quando devolve um conjunto de perfis
* ServiceManagement
  - Restart-AzureVM: parâmetro InitiateMaintenance adicionado para executar a manutenção durante o reinício da VM.
  - Get-AzureVM: campo de Estado de Manutenção adicionado.
  - Novos cmdlets adicionados para suportar a atualização do cofre dos Serviços de Recuperação
    + Test-AzureRecoveryServicesVaultUpgrade
    + Invoke-AzureRecoveryServicesVaultUpgrade
