---
title: "Registo de alterações do Azure PowerShell | Microsoft Docs"
description: "Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente."
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: 
ms.date: 05/18/2017
ms.openlocfilehash: 0a3f152751fee569d3ac5fba6bcff8c1737f7b8c
ms.sourcegitcommit: 226527be7cb647acfe2ea9ab151185053ab3c6db
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/29/2017
---
# <a name="release-notes"></a>Notas de versão

Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.

## <a name="version-170"></a>Versão 1.7.0

* **Alteração comportamental para os parâmetros -Force, –Confirm e $ConfirmPreference para todos os cmdlets. Estamos a alterar esta implementação para estar em conformidade com as diretrizes do PowerShell. Para a maioria dos cmdlets, isto significa remover o parâmetro Force e ignorar o pedido ShouldProcess; os utilizadores terão de incluir o parâmetro "-Confirm:$false" nos respetivos scripts do PowerShell.** Estas alterações visam os problemas seguintes:
  - Implementação correta da funcionalidade –WhatIf, que permite que um utilizador determine os efeitos de um cmdlet ou script sem fazer alterações reais
  - Controlo sobre pedidos utilizando uma $ConfirmPreference em toda a sessão, de modo a que o utilizador seja avisado com base no impacto de uma alteração potencial (tal como relatado na definição ConfirmImpact no cmdlet)
  - Controlo específico do cmdlet sobre pedidos de confirmação utilizando o parâmetro –Confirm
  - Utilização consistente de ShouldContinue e do parâmetro –Force em todos os cmdlets, para apenas as ações que precisem da confirmação do utilizador devido à natureza especial das alterações (por exemplo, eliminar ficheiros ocultos)
  - Consistência com outros cmdlets do PowerShell, para que o conhecimento de scripting do PowerShell de outros cmdlets seja imediatamente aplicável aos cmdlets do Azure PowerShell.

**Tenha em atenção que agora, para *ignorar automaticamente todos os Pedidos em todas as Circunstâncias*, os cmdlets do Azure PowerShell exigem que o utilizador forneça dois parâmetros:**
```powershell
My-CmdletWithConfirmation –Confirm:$false -Force
```
* Computação do Azure
  - Set-AzureRmVMADDomainExtension
  - Get-AzureRmVMADDomainExtension
  - Parâmetro -Redeploy para Restart-AzureVM
  - Parâmetro -Validate para Move-AzureService, Move-AzureStorageAccount e Move-AzureVirtualNetwork
  - Os parâmetros de nome e versão para cmdlets de extensão são opcionais como antes.
  - New-AzureVM pode obter um tipo de licença a partir do objeto VM.
* Storage do Azure
  - Alteração do Parâmetro de Etiquetas para Etiqueta e adição do alias do parâmetro Etiquetas
    + New-AzureRmStorageAccount
    + Set-AzureRmStorageAccount
* Rede do Azure
  - Novo cmdlet adicionado para Peering de Rede Virtual
* Cache de Redis do Azure
  - Novo cmdlet adicionado para Reset-AzureRmRedisCache
  - Novo cmdlet adicionado para Export-AzureRmRedisCache
  - Novo cmdlet adicionado para Import-AzureRmRedisCache
  - O cmdlet New-AzureRmRedisCache foi modificado para incluir a alteração do parâmetro para vNet
* Cópia de Segurança/Restauro da BD SQL do Azure
  - Cmdlets para a funcionalidade de cópia de segurança LTR (Retenção de Longo Prazo)
  - Get-AzureRmSqlServerBackupLongTermRetentionVault
  - Get-AzureRmSqlDatabaseBackupLongTermRetentionPolicy
  - Set-AzureRmSqlServerBackupLongTermRetentionVault
  - Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy
  - Restore-AzureRmSqlDatabase suporta agora o restauro para um ponto anterior no tempo de uma base de dados eliminada
  - Restore-AzureRmSqlDatabase suporta agora o restauro a partir de uma cópia de segurança de Retenção de Longo Prazo
* Azure LogicApp
  - Foram adicionados cmdlets de contas de Integração de LogicApp.
  - Get-AzureRmIntegrationAccountAgreement
  - Get-AzureRmIntegrationAccountCallbackUrl
  - Get-AzureRmIntegrationAccountCertificate
  - Get-AzureRmIntegrationAccount
  - Get-AzureRmIntegrationAccountMap
  - Get-AzureRmIntegrationAccountPartner
  - Get-AzureRmIntegrationAccountSchema
  - New-AzureRmIntegrationAccountAgreement
  - New-AzureRmIntegrationAccountCertificate
  - New-AzureRmIntegrationAccount
  - New-AzureRmIntegrationAccountMap
  - New-AzureRmIntegrationAccountPartner
  - New-AzureRmIntegrationAccountSchema
  - Remove-AzureRmIntegrationAccountAgreement
  - Remove-AzureRmIntegrationAccountCertificate
  - Remove-AzureRmIntegrationAccount
  - Remove-AzureRmIntegrationAccountMap
  - Remove-AzureRmIntegrationAccountPartner
  - Remove-AzureRmIntegrationAccountSchema
  - Set-AzureRmIntegrationAccountAgreement
  - Set-AzureRmIntegrationAccountCertificate
  - Set-AzureRmIntegrationAccount
  - Set-AzureRmIntegrationAccountMap
  - Set-AzureRmIntegrationAccountPartner
  - Set-AzureRmIntegrationAccountSchema
* Azure Data Lake Store
  - Melhoramento significativo do desempenho do carregamento e da transferência de ficheiros e pastas.
  - Isto inclui uma ligeira alteração aos nomes dos parâmetros para transferência e a inclusão de dois novos parâmetros para carregamento:
    + NumThreads -> PerFileThreadCount, utilizado para indicar o número de threads a utilizar num ficheiro único
    + ConcurrentFileCount, utilizado para indicar o número de ficheiros a carregar/transferir em paralelo para o carregamento/transferência de pastas.
  - Os valores de threading predefinidos visam agora proporcionar um melhor débito geral para a maioria dos tamanhos de ficheiro. Se o desempenho não for o pretendido, os valores acima podem ser modificados para satisfazer os requisitos.
* Azure Data Lake Analytics
  - Get-AzureRMDataLakeAnalyticsDataSource devolve agora todas as origens de dados quando é invocado sem argumentos.
  - Esta alteração também remove o parâmetro de tipo de origem de dados do cmdlet.
  - Esta alteração resulta na devolução de um novo objeto para a operação de lista com as seguintes propriedades:
    + Type, o tipo de origem de dados
    + Name, o nome da origem de dados
    + IsDefault, definido como true se for a origem de dados predefinida para a conta
  - Get-AzureRMDataLakeAnalyticsJob corrigido para lista para determinados valores de desvio de data e hora ao filtrar em submittedBefore e submittedAfter.
* Aplicações Web
  - Adição do cmdlet Swap-AzureRmWebAppSlot para troca regular e troca com pré-visualização
  - Expansão do cmdlet Set-AzureRmWebAppSlot para suportar a troca automática
* API Management do Azure
  - Correção dos cmdlets de Implementação de Gestão de API do Azure para AzureChinaCloud.
  - Remoção do cmdlet Set-AzureRmApiManagementTenantGitAccess, uma vez que o Acesso Git está ativado por Predefinição.
* Cópia de Segurança dos Serviços de Recuperação do Azure
  - Foi adicionado suporte para a carga de trabalho de SQL do Azure
  - Foi adicionado suporte para a criação de cópias de segurança e restauro de VMs encriptadas do Azure
  - Backup-AzureRmRecoveryServicesBackupItem - Funcionalidade de período de retenção opcional adicionada para pontos de recuperação
  - Pequenas correções de erros relacionados com filtros nos cmdlets Get-AzureRmRecoveryServicesBackupContainer e Get-AzureRmRecoveryServicesBackupItem
* Automatização do Azure
  - Get-AzureRmAutomationHybridWorkerGroup adicionado
