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
ms.date: 5/1/2018
ms.openlocfilehash: 8515a267e80e5d1f7bb97557efa72b9e86b7b45d
ms.sourcegitcommit: 37bfbf11fd0967a8e7977c692ab829d286baf88a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/08/2018
ms.locfileid: "33912008"
---
# <a name="release-notes"></a>Notas de versão

Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.

---

## <a name="600---may-2018"></a>6.0.0 - maio 2018

### <a name="general"></a>Geral
* Definir dependência mínima de módulos para o PowerShell 5.0

### <a name="azurestorage"></a>Azure.Storage
* Suporte como nome de contentor do blob de Armazenamento
    - New-AzureStorageBlobContainer
    - Remove-AzureStorageBlobContainer
    - Set-AzureStorageBlobContent
    - Get-AzureStorageBlobContent
* Correção do problema de alguns resultados de falha dos cmdlets de Armazenamento não conterem informações de falha de detalhe

### <a name="azurermapimanagement"></a>AzureRM.ApiManagement
* Introduzir várias alterações interruptivas
    - Veja o guia de migração para mais informações

### <a name="azurermautomation"></a>AzureRM.Automation
* Retirar alias de "Etiquetas" preteridas dos cmdlets
    - "Set-AzureRmAutomationRunbook"

### <a name="azurermbatch"></a>AzureRM.Batch
* Documentação do New-AzureBatchPool atualizada para remover exemplo preterido

### <a name="azurermcdn"></a>AzureRM.Cdn
* Introduzir várias alterações interruptivas
    - Veja o guia de migração para mais informações

### <a name="azurermcompute"></a>AzureRM.Compute
* O "New-AzureRmVm" e o "New-AzureRmVmss" suportam um resultado verboso de parâmetros
* O "New-AzureRmVm" e o "New-AzureRmVmss" (conjunto de parâmetros simples) suportam a atribuição de identidades definidas pelo sistema e (ou) definidas pelo utilizador para a(s) VM(s).
* Funcionalidade PerformMaintenance e Reimplementação do VMSS
    -  Adicionar novo parâmetro opcional -Redeploy e -PerformMaintenance to "Set-AzureRmVmss" e "Set-AzureRmVmssVM"
* Adicionar parâmetro opcional DisableVMAgent ao cmdlet "Set-AzureRmVMOperatingSystem"
* "New-AzureRmVm" e "New-AzureRmVmss" (conjunto de parâmetros simples) suportam uma imagem do "Win10".
* O cmdlet "Repair-AzureRmVmssServiceFabricUpdateDomain" foi adicionado.
* Introduzir várias alterações interruptivas
    - Veja o guia de migração para mais detalhes
* O "Set-AzureRmVmDiskEncryptionExtension" torna os parâmetros do AAD opcionais

### <a name="azurermdatafactories"></a>AzureRM.DataFactories
* Retirar alias de "Etiquetas" preteridas dos cmdlets
    - New-AzureRmDataFactory

### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* FO SDK de .Net do ADF foi atualizado para a versão 0.7.0-preview que contém as seguintes alterações:
    - Foram adicionados parâmetros de execução e propriedade de gestores de ligação na Atividade ExecuteSSISPackage
    - Serviço ligado atualizado PostgreSql MySql para utilizar a cadeia de ligação completa em vez do servidor, da base de dados, do esquema, do nome de utilizador e da palavra-passe
    - Esquema removido do serviço ligado DB2
    - Propriedade de esquema removida do serviço ligado Teradata
    - Foram adicionados o LinkedService, o Dataset e o CopySource ao Responsys

### <a name="azurermdatalakeanalytics"></a>AzureRM.DataLakeAnalytics
* Retirar alias de "Etiquetas" preteridas dos cmdlets
    - "New-AzureRmDataLakeAnalyticsAccount"
    - "Set-AzureRmDataLakeAnalyticsAccount"

### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* Adicionar nova funcionalidade da Alteração Acl recursiva a Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl
* Adicionar novo cmdlet para obter o resumo do conteúdo sob um diretório
* Adicionar novo cmdlet para obter a utilização do disco e a informação de falha de sistema de Acl
* Corrigir tipo de devolução de AzureRmDataLakeStoreItemAcl bool para IEnumerable<DataLakeStoreItemAce>
* Corrigir tipo de devolução de AzureRmDataLakeStoreItemAclEntry bool para IEnumerable<DataLakeStoreItemAce>
* Alterações interruptivas no Export-AzureRmDataLakeStoreItem, Import-AzureRmDataLakeStoreItem, Remove-AzureRmDataLakeStoreItem

### <a name="azurermdns"></a>AzureRM.Dns
* Introduzir várias alterações interruptivas
    - Veja o guia de migração para mais informações

### <a name="azurermeventhub"></a>AzureRM.EventHub
* Ajuda Atualizada para os cmdlets com exemplos em falta

### <a name="azurerminsights"></a>AzureRM.Insights
* Várias alterações interruptivas introduzidas
    - Veja o guia de migração para mais informações

### <a name="azurermiothub"></a>AzureRM.IotHub
* Ativar etiquetas e Sku Básico para o IotHub

### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Alterações interruptivas para suportar cenários de piping
* Novos cmdlets adicionados: Backup/Restore-AzureKeyVaultManagedStorageAccount, Backup/Restore-AzureKeyVaultCertificate, Undo-AzureKeyVaultManagedStorageSasDefinitionRemoval e Undo-AzureKeyVaultManagedStorageAccountRemoval

### <a name="azurermmachinelearning"></a>AzureRM.MachineLearning
* Retirar alias de "Etiquetas" preteridas dos cmdlets
    - Update-AzureRmMlCommitmentPlan

### <a name="azurermmedia"></a>AzureRM.Media
* Retirar alias de "Etiquetas" preteridas dos cmdlets
    - "Set-AzureRmMediaService"

### <a name="azurermnetwork"></a>AzureRM.Network
* Adicionar suporte ao recurso de plano de proteção contra DDoS
* Várias alterações interruptivas introduzidas
    - Veja o guia de migração para mais informações

### <a name="azurermnotificationhubs"></a>AzureRM.NotificationHubs
* Introduzir várias alterações interruptivas
    - Veja o guia de migração para mais informações

### <a name="azurermoperationalinsights"></a>AzureRM.OperationalInsights
* Introduzir várias alterações interruptivas
    - Veja o guia de migração para mais informações

### <a name="azurermprofile"></a>AzureRM.Profile
* Ativar gravação automática do contexto por predefinição
* Adicionar propriedades USGovernmentOperationalInsightsEndpoint e USGovernmentOperationalInsightsEndpointResourceId ao ambiente do Azure para US Gov.

### <a name="azurermrecoveryservicessiterecovery"></a>AzureRM.RecoveryServices.SiteRecovery
* Cabeçalho de Autenticação corrigida em cenários de SiteRecovery

### <a name="azurermrediscache"></a>AzureRM.RedisCache
* Várias alterações interruptivas introduzidas
    - Veja o guia de migração para mais informações

### <a name="azurermresources"></a>AzureRM.Resources
* Remova o parâmetro obsoleto -AtScopeAndBelow da chamada Get-AzureRmRoledefinition
* Incluir atribuições a Utilizadores/Grupos/ServicePrincipals eliminados no resultado do Get-AzureRmRoleAssignment
* Adicionar completadores de Separador de Âmbito e ResourceType
* Adicionar cmdlet de conveniência para criar ServicePrincipals
* Unir funcionalidade Get- e Find- no Get-AzureRmResource
* Adicionar Cmdlets do AD:
  - Remove-AzureRmADGroupMember
  - Get-AzureRmADGroup
  - New-AzureRmADGroup
  - Remove-AzureRmADGroup
  - Remove-AzureRmADUser
  - Update-AzureRmADApplication
  - Update-AzureRmADServicePrincipal
  - Update-AzureRmADUser

### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* Atualizar sku de versão de imagem do Linux predefinido
  - Atualização do Sku UbuntuServer1604 predefinido do NewAzureServiceFabricCluster.cs

### <a name="azurermstorage"></a>AzureRM.Storage
* Várias alterações interruptivas introduzidas
    - Veja o guia de migração para mais informações

### <a name="azurermwebsites"></a>AzureRM.Websites
* Atualizar para a versão mais recente do SDK de Sites
* Propriedades -AssignIdentity e -Httpsonly adicionadas a Set-AzureRmWebApp e a Set-AzureRmWebAppSlot
* Dois novos cmdlets adicionados: Get-AzureRmWebAppSnapshots e Restore-AzureRmWebAppSnapshot
