---
title: Registo de alterações do Azure PowerShell | Microsoft Docs
description: Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 5/1/2018
ms.openlocfilehash: 255e26aea5ea3cea866faa0d095cdf643c8ef0a8
ms.sourcegitcommit: de0e60800df1add9f3400166faacca202ef567d9
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/03/2018
ms.locfileid: "37406488"
---
# <a name="release-notes"></a>Notas de versão

Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.

---
## <a name="640---july-2018"></a>6.4.0 - julho de 2018
#### <a name="general"></a>Geral
* Correção da formatação de OutputType nos ficheiros de ajuda para a maioria dos módulos

#### <a name="azurermprofile"></a>AzureRM.Profile
* Foi adicionado o atributo Ps1Xml aos tipos de saída básicos

#### <a name="azurermcompute"></a>AzureRM.Compute
* Funcionalidade de Etiqueta IP para VMSS
    - Foi adicionado o cmdlet "New-AzureRmVmssIpTagConfig"
    - Foi adicionado o parâmetro IpTag a New-AzureRmVmssIpConfig
* Funcionalidade de Reversão do SO automática para VMSS
    - Foram adicionados parâmetros DisableAutoRollback a New-AzureRmVmssConfig e Update-AzureRmVmss
* Funcionalidade de Histórico de Atualização do SO para Vmss
    - Foi adicionado o parâmetro OSUpgradeHistory a Get-AzureRmVmss

#### <a name="azurermdatalakeanalytics"></a>AzureRM.DataLakeAnalytics
* Adição de suporte para ACLs de Catálogo através dos seguintes comandos:
    - Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry
    - Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry
    - Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry

#### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* Adição de suporte ao cancelamento e de controlo do progresso para Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry e Set-AzureRmDataLakeStoreItemAcl
* Adição de suporte ao cancelamento para Export-AzureRmDataLakeStoreChildItemProperties
* Correção da remoção de mensagens de depuração para cmdlets que realizam operações recursivas
* Correção da localização de teste de cmdlets do DataLake

#### <a name="azurermeventhub"></a>AzureRM.EventHub
* Adição do parâmetro Optional MaxCount aos cmdlets Get-AzureRmEventHub e Get-AzureRmEventHubConsumerGroup de List Operations
* Correção de problema no cmdlet New-AzureRmEventHub, no qual era necessário, pelo menos, um parâmetro durante a criação de um novo EventHub. Conjunto de Parâmetros Predefinidos fornecido.
* Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmEventHubKey, o que permite ao utilizador fornecer o KeyValue.

#### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Correção de problema no qual todos os recursos eram devolvidos por Get-AzureRmKeyVault -Tag

#### <a name="azurermnetwork"></a>AzureRM.Network
* Apresentação de novos SKUs para VirtualNetworkGateways com redundância de zona
* Adição de novos comandos para a funcionalidade: APIs de Parceiro do ExpressRoute via ARM
    - Adição de Get-AzureRmExpressRouteCrossConnection
    - Adição de Set-AzureRmExpressRouteCrossConnection
    - Adição de Add-AzureRmExpressRouteCrossConnectionPeering
    - Adição de Get-AzureRmExpressRouteCrossConnectionPeering
    - Adição de Remove-AzureRmExpressRouteCrossConnectionPeering
    - Adição de Get-AzureRMExpressRouteCrossConnectionArpTable
    - Adição de Get-AzureRMExpressRouteCrossConnectionRouteTable
    - Adição de Get-AzureRMExpressRouteCrossConnectionRouteTableSummary

#### <a name="azurermrecoveryservicesbackup"></a>AzureRM.RecoveryServices.Backup
* Adição do cmdlet Get-AzureRmRecoveryServicesBackupStatus. Este cmdlet vai buscar um ID da VM e verifica se a VM está protegida por algum cofre na subscrição. Se o cofre existir, o cmdlet devolve os detalhes do cofre.

#### <a name="azurermresources"></a>AzureRM.Resources
* Atualização de cmdlets Get-AzureRmPolicyAssignment:
    - Adição de suporte para a listagem de valores -Scope ao nível do grupo de gestão
    - Adição de suporte para a obtenção de atribuições individuais com valores -Scope ao nível do grupo de gestão
    - Adição de parâmetros -Effective e -All ao parâmetro de controlo
* Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicyDefinition
    - Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão
    - Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição
* Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicySetDefinition
    - Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão
    - Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição
* Adição de suporte de referência de segredo do KeyVault nos parâmetros ao utilizar "TemplateParameterObject" em "New-AzureRmResourceGroupDeployment"
* Correção de problema em que o parâmetro "-EndDate" era ignorado para "New-AzureRmADAppCredential"
    - https://github.com/Azure/azure-powershell/issues/6505
* Correção de problema em que "Add-AzureRmADGroupMember" utilizava o URL incorreto para fazer o pedido
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmServiceBusKey, o que permite ao utilizador fornecer o KeyValue.

#### <a name="azurermsql"></a>AzureRM.Sql
* Esclarecimento dos Pontos de Restauro Definidos pelo Utilizador para SQLDW na ajuda de New-AzureRmSqlDatabaseRestorePoint
* Atualização da documentação do parâmetro -ComputeGeneration em vários cmdlets

## <a name="630---june-2018"></a>6.3.0 - junho de 2018
#### <a name="azurermprofile"></a>AzureRM.Profile
* Atualização das mensagens de erro de Enable-AzureRmContextAutoSave
* Criação de contexto para cada subscrição ao executar "Connect-AzureRmAccount" sem contexto anterior

#### <a name="azurestorage"></a>Azure.Storage
* Adição de outras informações sobre o parâmetro -Permissions nos ficheiros de ajuda.

#### <a name="azurermcompute"></a>AzureRM.Compute
* "Get-AzureRmVmDiskEncryptionStatus" corrige um problema observado em VMs sem discos de dados 
* Atualização da versão da biblioteca de cliente de Computação para corrigir os seguintes cmdlets
    - Grant-AzureRmDiskAccess
    - Grant-AzureRmSnapshotAccess
    - Save-AzureRmVMImage
* Correção dos seguintes cmdlets para mostrar o "ID da operação" e o "estado da operação" corretamente:
    - Start-AzureRmVM
    - Stop-AzureRmVM
    - Restart-AzureRmVM
    - Set-AzureRmVM
    - Remove-AzuerRmVM
    - Set-AzureRmVmss
    - Start-AzureRmVmssRollingOSUpgrade
    - Stop-AzureRmVmssRollingUpgrade
    - Start-AzureRmVmss
    - Restart-AzureRmVmss
    - Stop-AzureRmVmss
    - Remove-AzureRmVmss
    - ConvertTo-AzureRmVMManagedDisk
    - Revoke-AzureRmSnapshotAccess
    - Remove-AzureRmSnapshot
    - Revoke-AzureRmDiskAccess
    - Remove-AzureRmDisk
    - Remove-AzureRmContainerService
    - Remove-AzureRmAvailabilitySet

#### <a name="azurermeventgrid"></a>AzureRM.EventGrid
* Remoção das condições de validação ValidateNotNullOrEmpty para SubjectBeginsWith/SubjectEndsWith no cmdlet Update-AzureRmEventGridSubscription para permitir a alteração destes parâmetros para uma cadeia vazia, se necessário.

#### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Correção de problema em que não são devolvidas Etiquetas quando Get-AzureRmKeyVault -Tag é executado

#### <a name="azurermpolicyinsights"></a>AzureRM.PolicyInsights
* Disponibilização pública de cmdlets de Informações de Política
    - Utilização da versão da API 2018-04-04
    - Adição de PolicyDefinitionReferenceId aos resultados de Get-AzureRmPolicyStateSummary

#### <a name="azurermrecoveryservicesbackup"></a>AzureRM.RecoveryServices.Backup
* Adição do parâmetro -Vault a cmdlets RecoveryServices.Backup. Ao ser transmitido, substitui o cmdlet Set-AzureRmRecoveryServicesContext.

#### <a name="azurermsql"></a>AzureRM.Sql
* Atualização de exemplo no ficheiro de ajuda para Get-AzureRmSqlDatabaseExpanded

#### <a name="azurermtrafficmanager"></a>AzureRM.TrafficManager
* Atualização do ficheiro de ajuda para Add-AzureRmTrafficManagerEndpointConfig

#### <a name="azurermwebsites"></a>AzureRM.Websites
* Atualização de "Set-AzureRmWebApp" de modo a não substituir AppSettings quando -AssignIdentity é utilizado
* Atualização de "New-AzureRmWebAppSlot" de modo a honrar AppServicePlan como um parâmetro opcional

## <a name="621---june-2018"></a>6.2.1 - junho de 2018
### <a name="azurermoperationalinsights"></a>AzureRM.OperationalInsights
* Atualização do modelo de PSWorkspace para permitir que a Rede utilize o tipo como um parâmetro

## <a name="620---june-2018"></a>6.2.0 - junho de 2018
#### <a name="azurermprofile"></a>AzureRM.Profile
* Corrija o problema onde a versão 10.0.3 de Newtonsoft.Json não foi carregada na importação do módulo

#### <a name="azurermcompute"></a>AzureRM.Compute
* Funcionalidade Atualização da VM VMSS
    - Cmdlets "Update-AzureRmVmssVM" e "New-AzureRmVMDataDisk" adicionados
    - Adicione o parâmetro VirtualMachineScaleSetVM ao cmdlet "Add-AzureRmVMDataDisk" para suportar a adição de um disco de dados à VM Vmss.

#### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* O SDK de .Net do ADF foi atualizado para a versão 0.8.0-preview que contém as seguintes alterações:
    - Foi adicionada a operação de Configuração de fábrica do repositório
    - QuickBooks LinkedService atualizado para expor as propriedades consumerKey e consumerSecret
    - Vários tipos de modelos Atualizados de SecretBase para Object
    - Acionador de Eventos de Blob adicionado

### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Documentação de atualização com resultado de exemplo

### <a name="azurermnetwork"></a>AzureRM.Network
* Ativar parâmetros da Análise de Tráfego em cmdlets do Observador de Rede

#### <a name="azurermresources"></a>AzureRM.Resources
* Corrija o problema com a propriedade "Propriedades" do(s) objeto(s) "PSResource" devolvidos por "Get-AzureRmResource"

#### <a name="azurermscheduler"></a>AzureRM.Scheduler
* Corrija o problema com a atualização ServiceBusQueueJob sem definir novos valores de Autenticação

### <a name="azurermsql"></a>AzureRM.Sql
* Cmdlets seguintes atualizados com parâmetro opcional LicenseType
    - New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase
    - New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool
    - New-AzureRmSqlDatabaseCopy
    - New-AzureRmSqlDatabaseSecondary
    - Restore-AzureRmSqlDatabase

#### <a name="azurermwebsites"></a>AzureRM.Websites
* "New-AzureRMWebApp" está atualizado para utilizar algoritmos comuns da biblioteca Estratégia.

## <a name="610---may-2018"></a>6.1.0 - Maio de 2018
#### <a name="azurermprofile"></a>AzureRM.Profile
* Correção do problema em que a execução de "Clear-AzureRmContext" mantinha um contexto vazio com o nome do contexto predefinido anterior, o que impedia o utilizador de criar um novo contexto com o nome antigo

#### <a name="azurermanalysisservices"></a>AzureRM.AnalysisServices
* Permitir operações de associação/desassociação do Gateway no AS.

#### <a name="azurermapimanagement"></a>AzureRM.ApiManagement
* Foi adicionado suporte para ApiVersions, ApiReleases e ApiRevisions
* Foi adicionado suporte para o Back-end do ServiceFabric
* Foi adicionado suporte para o Logger do Application Insights
* Foi adicionado suporte para reconhecer o SKU "Básico" como um SKU válido do serviço Gestão de API
* Foi adicionado suporte para instalar Certificados emitidos por AC privadas como Raiz ou AC
* Foi adicionado suporte para aceitar Certificados SSL personalizados através do KeyVault e de vários nomes de anfitrião de proxy
* Foi adicionado suporte para a identidade MSI
* Foi adicionado suporte para aceitar políticas através de Url. NOTA: Os cmdlets seguintes serão preteridos numa versão futura
   - Import-AzureRmApiManagementHostnameCertificate
   - New-AzureRmApiManagementHostnameConfiguration
   - Set-AzureRmApiManagementHostnames
   - Update-AzureRmApiManagementDeployment

#### <a name="azurermbatch"></a>AzureRM.Batch
* Lançamento do novo cmdlet Get-AzureBatchPoolNodeCounts
* Lançamento do novo cmdlet Start-AzureBatchComputeNodeServiceLogUpload

#### <a name="azurermconsumption"></a>AzureRM.Consumption
* Adição dos novos parâmetros Expand, ResourceGroup, InstanceName, InstanceId, Tags e Top no Cmdlet Get-AzureRmConsumptionUsageDetail

#### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* Correção do exemplo de Export-AzureRmDataLakeStoreChildItemProperties
* Correção da exceção do parâmetro nulo do caso Recursivo em Set-AzureRmDataLakeStoreItemAclEntry 
* Correção dos ficheiros de ajuda de Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry 

#### <a name="azurermnetwork"></a>AzureRM.Network
* Aumento da versão do SDK de Rede de 18.0.0-preview para 19.0.0-preview
* Foi adicionado um cmdlet para criar a configuração de protocolo
    - New-AzureRmNetworkWatcherProtocolConfiguration
* Foi adicionado um cmdlet para adicionar uma nova ligação de circuito a um circuito existente do ExpressRoute.
    - Add-AzureRmExpressRouteCircuitConnectionConfig
* Foi adicionado um cmdlet para remover uma ligação de circuito de um circuito existente do ExpressRoute.
    - Remove-AzureRmExpressRouteCircuitConnectionConfig
* Foi adicionado um cmdlet para obter uma ligação de circuito
    - Get-AzureRmExpressRouteCircuitConnectionConfig

#### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* Correção da utilização da autenticação de servidor com certificados gerados (Problema #5998)

#### <a name="azurermsql"></a>AzureRM.Sql
* Atualização dos cmdlets de Auditoria para permitir a remoção de AuditActions ou AuditActionGroups
* Correção do problema de Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy ao definir uma nova política de retenção flexível em que o comando falhava com "Configurar a política de retenção de longo-prazo com o cofre e a política do serviço de recuperação do Azure já não é suportado. Submeta um pedido com a nova política de retenção flexível".
* Atualize todos os cmdlets relacionados com as Bases de Dados SQL do Azure/Criação de Conjuntos Elásticos/Atualização para utilizar a nova API de Base de Dados, que suporta a propriedade SKU para propriedades relacionadas com dimensionamento e escalão.
* Os cmdlets atualizados, incluindo: 
    - New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase
    - New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool
    - New-AzureRmSqlDatabaseCopy
    - New-AzureRmSqlDatabaseSecondary
    - Restore-AzureRmSqlDatabase

#### <a name="azurermtrafficmanager"></a>AzureRM.TrafficManager
* Atualize os parâmetros de "Get-AzureRmTrafficManagerProfile" para que o parâmetro -ResourceGroupName seja necessário ao utilizar o parâmetro -Name.