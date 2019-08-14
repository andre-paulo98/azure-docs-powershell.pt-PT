---
title: Registo de alterações do Azure PowerShell | Microsoft Docs
description: Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 2/20/2018
ms.openlocfilehash: 61ab0f91c3d6fffdbffd336fa0d6ed9b0ab8f6ec
ms.sourcegitcommit: b02cbcd00748a4a9a4790a5fba229ce53c3bf973
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/09/2019
ms.locfileid: "68863283"
---
# <a name="release-notes"></a>Notas de versão

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.

---

# <a name="azure-powershell-570"></a>Azure PowerShell 5.7.0

Instalador do Azure PowerShell 5.7.0: [ligação](https://github.com/Azure/azure-powershell/releases/download/v5.7.0-April2018/azure-powershell.5.7.0.msi)

Módulo da Galeria para Cmdlets ARM: [ligação](https://www.powershellgallery.com/packages/AzureRM/5.7.0)

Para instalar `AzureRM` a partir da Galeria do PowerShell, execute o seguinte comando:

```powershell-interactive
Install-Module -Name AzureRM -Repository PSGallery -Force
```

Para atualizar a partir de uma versão mais antiga do `AzureRM`, execute o seguinte comando:

```powershell-interactive
Update-Module -Name AzureRM
```

## <a name="changes-since-last-release"></a>Alterações Desde a Última Versão

#### <a name="general"></a>Geral
* Atualizado para a versão mais recente do Azure ClientRuntime

#### <a name="azurestorage"></a>Azure.Storage
* Resolução do problema de falha no carregamento de Blobs e de cmdlets File em máquinas com a política FIPS ativada
    - Set-AzureStorageBlobContent
    - Set-AzureStorageFileContent

#### <a name="azurermbilling"></a>AzureRM.Billing
* Novo Cmdlet Get-AzureRmEnrollmentAccount
  - cmdlet para obter as contas de inscrição

#### <a name="azurermcognitiveservices"></a>AzureRM.CognitiveServices
* Integração com o Cognitive Services Management SDK versão 4.0.0.
* Adição da operação Get-AzureRmCognitiveServicesAccountUsage.

#### <a name="azurermcompute"></a>AzureRM.Compute
* `Get-AzureRmVmssDiskEncryptionStatus` suporta o estado de encriptação ao nível do disco de dados
* `Get-AzureRmVmssVmDiskEncryptionStatus` suporta o estado de encriptação ao nível do disco de dados
* Atualização para Resiliência de Zona
* "New-AzureRmVm" e "New-AzureRmVmss" (conjunto de parâmetros simples) suportam zonas de disponibilidade.

#### <a name="azurermcontainerregistry"></a>AzureRM.ContainerRegistry
* Desacoplar dependência de SDKs Commands.Resources.Rest e ARM/Storage.

#### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* Adição de funcionalidades de depuração
* Atualização da versão do ADLS dataplane SDK para 1.1.2
* Export-AzureRmDataLakeStoreItem - Parâmetros PerFileThreadCount e ConcurrentFileCount preteridos, e introdução de Simultaneidade de parâmetros
* Import-AzureRMDataLakeStoreItem - Parâmetros PerFileThreadCount e ConcurrentFileCount preteridos, e introdução de Simultaneidade de parâmetros
* Get-AzureRMDataLakeStoreItemContent - Correção do comportamento de erro para conteúdos com mais de 4 MB
* Set-AzureRMDataLakeStoreItemExpiry - Introdução do novo conjunto de parâmetros SetRelativeExpiry para definição do tempo de expiração relativo
* Remove-AzureRmDataLakeStoreItem - Parâmetro Clean preterido.

#### <a name="azurermeventhub"></a>AzureRM.EventHub
* Correção de AlternameName em New-AzureRmEventHubGeoDRConfiguration

#### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Cmdlets atualizados para incluir cenários de piping
* Adição de mensagens de preterição para futuras alterações de versão de última hora

#### <a name="azurermnetwork"></a>AzureRM.Network
* Correção de mensagem de erro com cmdlets de Rede

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* Adição de "properties" em CorrelationFilter de Rules para suportar customproperties
* Atualização da ajuda de New-AzureRmServiceBusGeoDRConfiguration e correção da saída de dados do cmdlet Rules
* Correção das propriedades de reencaminhamento automático no cmdlet New-AzureRmServiceBusQueue e New-AzureRmServiceBusSubscription

#### <a name="azurermsql"></a>AzureRM.Sql
* Adição do novo cmdlet "Stop-AzureRmSqlElasticPoolActivity" para suportar o cancelamento de operações assíncronas no conjunto elástico
* Atualização das respostas para cmdlets Get-AzureRmSqlDatabaseActivity e Get-AzureRmSqlElasticPoolActivity para incluir mais informações na resposta

Alterações desde a última versão: https://github.com/Azure/azure-powershell/compare/v5.6.0-March2018...v5.7.0-April2018

## <a name="560---march-2018"></a>5.6.0 - Março de 2018

#### <a name="general"></a>Geral
* Corrigir o problema associado ao Grupo de Recursos Predefinidos no Cloud Shell
* Corrigir o problema em que scripts de arranque incorretos estavam a ser executados durante a importação do módulo

#### <a name="azurermprofile"></a>AzureRM.Profile
* Ativar a autenticação de MSI em cenários não suportados
* Adicionar suporte para a Identidade do Serviço Gerido definida pelo utilizador

#### <a name="azurermanalysisservices"></a>AzureRM.AnalysisServices
* Foi corrigido o problema associado à limpeza de scripts na compilação

#### <a name="azurermcdn"></a>AzureRM.Cdn
* Foi corrigido o problema associado à limpeza de scripts na compilação

#### <a name="azurermcompute"></a>AzureRM.Compute
* O "New-AzureRmVM" e o "New-AzureRmVMSS" suportam discos de dados.
* O "New-AzureRmVM" e o "New-AzureRmVMSS" suportam imagem personalizada por nome ou ID.
* Funcionalidade de análise de registo
    - Foi adicionado o cmdlet "Export-AzureRmLogAnalyticRequestRateByInterval"
    - Foi adicionado o cmdlet "Export-AzureRmLogAnalyticThrottledRequests"

#### <a name="azurermcontainerinstance"></a>AzureRM.ContainerInstance
* Corrigir o problema associado a conjuntos de parâmetros para o registo de contentor e a montagem de volumes de ficheiros do Azure

#### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* Foi atualizado o SDK de .Net do ADF para a versão 0.6.0-preview que contém as seguintes alterações:
    - Foram adicionadas as atividades novas AzureDatabricks, LinkedService e DatabricksNotebook
    - Foram adicionadas as propriedades headNodeSize e dataNodeSize em HDInsightOnDemand LinkedService
    - Foram adicionados os itens LinkedService, Dataset e CopySource para SalesforceMarketingCloud
    - Foi adicionado suporte para SecureOutput em todas as atividades
    - Foi adicionada a nova propriedade BatchCount na atividade ForEach que controla o número de atividades simultâneas a executar
    - Foi adicionada uma nova atividade Filter
    - Foi adicionado suporte de Parâmetros de Serviços Ligados

#### <a name="azurermdns"></a>AzureRM.Dns
* Suporte para Zonas de DNS Privado (Pré-visualização Pública)
    - Adiciona a capacidade de criar zonas DNS visíveis apenas para as redes virtuais associadas

#### <a name="azurermnetwork"></a>AzureRM.Network
* Atualização de tipos de modelo para efeitos de compatibilidade com os cmdlets de DNS.

#### <a name="azurermrecoveryservicessiterecovery"></a>AzureRM.RecoveryServices.SiteRecovery
* Alterações do ASR Azure para o Azure Site Recovery (os cmdlets suportam atualmente operações de Enterprise para Enterprise, Enterprise para Azure, HyperV para Azure e VMware para Azure)
    - New-AzureRmRecoveryServicesAsrProtectionContainer
    - New-AzureRmRecoveryServicesAsrAzureToAzureDiskReplicationConfig
    - Remove-AzureRmRecoveryServicesAsrProtectionContainer
    - Update-AzureRmRecoveryServicesAsrProtectionDirection

#### <a name="azurermstorage"></a>AzureRM.Storage
* Parâmetros obsoletos nos cmdlets novos e definidos da conta de armazenamento seguintes: EnableEncryptionService e DisableEncryptionService, uma vez que a Encriptação Inativa está ativada por predefinição e não pode ser desativada.
    - New-AzureRmStorageAccount
    - Set-AzureRmStorageAccount

#### <a name="azurermwebsites"></a>AzureRM.Websites
* Foi corrigida a ajuda de Remove-AzureRmWebAppSlot

## <a name="550---march-2018"></a>5.5.0 - março de 2018
#### <a name="azurermprofile"></a>AzureRM.Profile
* Problema corrigido ao importar aliases
* Carregar versão 10.0.3 de Newtonsoft.Json lado a lado com a versão 6.0.8

#### <a name="azurestorage"></a>Azure.Storage
* Funcionalidade Eliminação Suave do Suporte
    - Enable-AzureStorageDeleteRetentionPolicy
    - Disable-AzureStorageDeleteRetentionPolicy
    - Get-AzureStorageBlob

#### <a name="azurermanalysisservices"></a>AzureRM.AnalysisServices
* Problema corrigido ao importar aliases
* Adicione o suporte da firewall e a funcionalidade de ampliar consultas, bem como o suporte da versão de api de 2017-08-01.

#### <a name="azurermautomation"></a>AzureRM.Automation
* Problema corrigido ao importar aliases

#### <a name="azurermcdn"></a>AzureRM.Cdn
* Problema corrigido ao importar aliases

#### <a name="azurermcognitiveservices"></a>AzureRM.CognitiveServices
* Atualizar notice.txt e mensagem de aviso.

#### <a name="azurermcompute"></a>AzureRM.Compute
* "New-AzureRmVMSS" imprime cadeias de ligação no modo verboso.
* "New-AzureRmVMSS" suporta endereço IP público, regras de balanceamento de carga e regras NAT de entrada.
* Funcionalidade WriteAccelerator
    - Parâmetro de mudança de WriteAccelerator adicionado aos seguintes cmdlets: Set-AzureRmVMOSDisk Set-AzureRmVMDataDisk Add-AzureRmVMDataDisk Add-AzureRmVmssDataDisk
    - Parâmetro de mudança de OsDiskWriteAccelerator adicionado aos seguintes cmdlets:     Set-AzureRmVmssStorageProfile.
    - Parâmetro booleano de OsDiskWriteAccelerator adicionado aos seguintes cmdlets:     Update-AzureRmVM     Update-AzureRmVmss

#### <a name="azurermdatafactories"></a>AzureRM.DataFactories
* Corrija o problema de encriptação de credencial que não originou um erro significativo para algumas operações de encriptação
* Ativar o runtime de integração para ser partilhado na fábrica de dados

#### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* Adicione o parâmetro "SetupScriptContainerSasUri" e "Edition" ao cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para ativar a funcionalidade de seleção de configuração e edição personalizada
* Corrija o problema de encriptação de credencial que não originou um erro significativo para algumas operações de encriptação.
* Ativar o runtime de integração para ser partilhado na fábrica de dados

#### <a name="azurermhdinsight"></a>AzureRM.HDInsight
* Problema corrigido ao importar aliases

#### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Exemplo corrigido para Set-AzureRmKeyVaultAccessPolicy

#### <a name="azurermnetwork"></a>AzureRM.Network
* Problema corrigido ao importar aliases

#### <a name="azurermoperationalinsights"></a>AzureRM.OperationalInsights
* Problema corrigido ao importar aliases

#### <a name="azurermrecoveryservices"></a>AzureRM.RecoveryServices
* Problema corrigido ao importar aliases

#### <a name="azurermrecoveryservicessiterecovery"></a>AzureRM.RecoveryServices.SiteRecovery
* Problema corrigido ao importar aliases

#### <a name="azurermresources"></a>AzureRM.Resources
* Problema corrigido ao importar aliases

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* Propriedade EnableBatchedOperations adicionada à Fila
* Propriedade DeadLetteringOnFilterEvaluationExceptions adicionada às Subscrições

#### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* Atualização de cmdlet do Service Fabric
  - Modelos do ARM atualizados
  - As operações com falha não voltam a ser revertidas
  - Add-AzureRmServiceFabricNodeType
    - VMs predefinidas para discos geridos
    - Sub-rede de VMSS existente utilizada
    - Todas as operações são idempotentes
  - O Remove-AzureRmServiceFabricNodeType limpa o VMSS parcialmente criado e/ou os tipos de nó de cluster
  - Saída corrigida do objeto do PSCluster para tipos de propriedade complexos

#### <a name="azurermsql"></a>AzureRM.Sql
* Problema corrigido ao importar aliases
* A resposta de Get-AzureRmSqlServer, New-AzureRmSqlServer e Remove-AzureRmSqlServer inclui agora a propriedade FullyQualifiedDomainName.

#### <a name="azurermwebsites"></a>AzureRM.Websites
* Problema corrigido ao importar aliases
* New-AzureRMWebApp - conjunto de parâmetros adicionado à criação da WebApp simplificada, com suporte do repositório de git local.

## <a name="540---february-2018"></a>5.4.0 - fevereiro 2018
#### <a name="azurermautomation"></a>AzureRM.Automation
* Alias adicionado de New-AzureRmAutomationModule para Import-AzureRmAutomationModule

#### <a name="azurermcompute"></a>AzureRM.Compute
* Corrija o problema ErrorAction para alguns dos cmdlets Get.

#### <a name="azurermcontainerinstance"></a>AzureRM.ContainerInstance
* Aplicar o SDK de 01-02-2018 da Instância de Contentor do Azure
    - Etiqueta de nome DNS de suporte

#### <a name="azurermdevtestlabs"></a>AzureRM.DevTestLabs
* Corrigidos todos os cmdlets GET que anteriormente não funcionavam.

#### <a name="azurermeventhub"></a>AzureRM.EventHub
* Corrija o erro na ajuda Get-AzureRmEventHubGeoDRConfiguration

#### <a name="azurermnetwork"></a>AzureRM.Network
* Cmdlet adicionado para criar um novo monitor de ligação
    - New-AzureRmNetworkWatcherConnectionMonitor
* Cmdlet adicionado para atualizar um monitor de ligação
    - Set-AzureRmNetworkWatcherConnectionMonitor
* Cmdlet adicionado para obter monitor de ligação ou lista do monitor de ligação
    - Get-AzureRmNetworkWatcherConnectionMonitor
* Cmdlet adicionado para consultar monitor de ligação
    - Get-AzureRmNetworkWatcherConnectionMonitorReport
* Cmdlet adicionado para iniciar monitor de ligação
    - Start-AzureRmNetworkWatcherConnectionMonitor
* Cmdlet adicionado para parar monitor de ligação
    - Stop-AzureRmNetworkWatcherConnectionMonitor
* Cmdlet adicionado para remover monitor de ligação
    - Remove-AzureRmNetworkWatcherConnectionMonitor
* Documentação de Set-AzureRmApplicationGatewayBackendAddressPool atualizada para remover exemplo preterido
* Sinalizador de EnableHttp2 adicionado ao Gateway de Aplicação
    - New-AzureRmApplicationGateway atualizado: O parâmetro opcional -EnableHttp2 adicionado
* Adicionar IpTags a PublicIpAddress
    - New-AzureRmPublicIpAddress atualizado: IpTags adicionadas
    - New-AzureRmPublicIpTag para adicionar Iptag
* Adicione a propriedade DisableBgpRoutePropagation ao RouteTable e effectiveRoute.

#### <a name="azurermresources"></a>AzureRM.Resources
* Register-AzureRmProviderFeature: Exemplo em documentos em falta adicionado
* Register-AzureRmResourceProvider: Exemplo em documentos em falta adicionado

#### <a name="azurermstorage"></a>AzureRM.Storage
* Parâmetros obsoletos nos cmdlets novos e definidos da conta de armazenamento seguintes: EnableEncryptionService e DisableEncryptionService, uma vez que a Encriptação Inativa está ativada por predefinição e não pode ser desativada.
    - New-AzureRmStorageAccount
    - Set-AzureRmStorageAccount


## <a name="530---february-2018"></a>5.3.0 - fevereiro 2018
### <a name="azurermprofile"></a>AzureRM.Profile
* Aviso de preterição adicionado aos PowerShell 3 e 4
* `Add-AzureRmAccount` teve o nome alterado para `Connect-AzureRmAccount`; foi adicionado um alias ao nome antigo do cmdlet e os outros aliases (`Login-AzAccount` e `Login-AzureRmAccount`) foram redirecionados para o novo nome do cmdlet.
* `Remove-AzureRmAccount` teve o nome alterado para `Disconnect-AzureRmAccount`; foi adicionado um alias ao nome antigo do cmdlet e os outros aliases (`Logout-AzAccount` e `Logout-AzureRmAccount`) foram redirecionados para o novo nome do cmdlet.
* As Cadeias de Recursos foram corrigidas para utilizar `Connect-AzureRmAccount` em vez de `Login-AzureRmAccount`
* `Add-AzureRmEnvironment` e `Set-AzureRmEnvironment`
  - Foram adicionados `-AzureOperationalInsightsEndpoint` e `-AzureOperationalInsightsEndpointResourceId` como parâmetros para a utilização com o RP do plano de dados OperationalInsights.

### <a name="azurermanalysisservices"></a>AzureRM.AnalysisServices
* Corrigida a utilização de `Login-AzureRmAccount` para utilizar `Connect-AzureRmAccount`

### <a name="azurermcompute"></a>AzureRM.Compute
* Foi adicionado o parâmetro `-AvailabilitySetName` para o parameterset simplificado de `New-AzureRmVM`.
* Corrigida a utilização de `Login-AzureRmAccount` para utilizar `Connect-AzureRmAccount`
* Suporte de identidade atribuída ao utilizador para VM e conjunto de dimensionamento da VM
    - Os parâmetros `-IdentityType` e `-IdentityId` foram adicionados a `New-AzureRmVMConfig`, `New-AzureRmVmssConfig`, `Update-AzureRmVM` e `Update-AzureRmVmss`
* Foi adicionado o parâmetro `-EnableIPForwarding` para `Add-AzureRmVmssNetworkInterfaceConfig`
* Foi adicionado o parâmetro `-Priority` para `New-AzureRmVmssConfig`

### <a name="azurermdatalakeanalytics"></a>AzureRM.DataLakeAnalytics
* Corrigida a utilização de `Login-AzureRmAccount` para utilizar `Connect-AzureRmAccount`

### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* Corrigida a utilização de `Login-AzureRmAccount` para utilizar `Connect-AzureRmAccount`
* Corrigida a mensagem de erro de `Test-AzureRmDataLakeStoreAccount` ao executar este cmdlet sem ter a sessão iniciada com `Login-AzureRmAccount`

### <a name="azurermeventgrid"></a>AzureRM.EventGrid
* Atualizado para utilizar a versão da API "2018-01-01".

### <a name="azurermeventhub"></a>AzureRM.EventHub

* Adicionados os novos comandos abaixo para operações de Recuperação Após Desastre Georredundante.
  - Criar um novo Alias (configuração da Recuperação Após Desastre):
    - `New-AzureRmEventHubGeoDRConfiguration`
  - Obter o Alias (configuração da Recuperação Após Desastre):
    - `Get-AzureRmEventHubGeoDRConfiguration`
  - Desativar a Recuperação Após Desastre e parar a replicação de alterações de espaço de nomes principais para secundários
    - `Set-AzureRmEventHubGeoDRConfigurationBreakPair`
  - Invocar a ativação pós-falha da Recuperação Após Desastre e reconfigurar o alias de modo a apontar para o espaço de nomes secundário
    - `Set-AzureRmEventHubGeoDRConfigurationFailOver`
  - Eliminar um Alias (configuração da Recuperação Após Desastre)
    - `Remove-AzureRmEventHubGeoDRConfiguration`
* Adicionados novos comandos ao verificar o Nome do Espaço de Nomes e Nome de Configuração GeoDR - disponibilidade de Alias.
  - Verificar a disponibilidade do nome do Espaço de Nomes ou do nome do Alias (configuração da Recuperação Após Desastre):
    - `Test-AzureRmEventHubName`

### <a name="azurerminsights"></a>AzureRM.Insights
* Corrigida a utilização de `Login-AzureRmAccount` para utilizar `Connect-AzureRmAccount`

### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Corrigida a utilização de `Login-AzureRmAccount` para utilizar `Connect-AzureRmAccount`

### <a name="azurermnetwork"></a>AzureRM.Network
* Corrige a mensagem de substituição "Quer mesmo substituir o recurso"

#### <a name="azurermoperationalinsights"></a>AzureRM.OperationalInsights
* Suporte adicionado para a consulta da API V2 via `Invoke-AzureRmOperationalInsightsQuery`. Veja [https://dev.loganalytics.io/](https://dev.loganalytics.io/) para obter mais informações sobre a nova API.

### <a name="azurermresources"></a>AzureRM.Resources
* `Get-AzureRmADServicePrincipal`: `-ServicePrincipalName` removido do parâmetro Vazio predefinido dado que era redundante com o parâmetro SPN definido

### <a name="azurermservicebus"></a>AzureRM.ServiceBus

* Adicionada a correção de funcionalidade para `Remove-AzureRmServiceBusRule` e `Get-AzureRmServiceBusKey`
* Adicionados os novos commandlets abaixo para operações de Recuperação Após Desastre Georredundante.
  - Criar um novo Alias (configuração da Recuperação Após Desastre):
    - `New-AzureRmServiceBusDRConfigurations`
  - Obter o Alias (configuração da Recuperação Após Desastre):
    - `Get-AzureRmServiceBusDRConfigurations`
  - Desativar a Recuperação Após Desastre e parar a replicação de alterações de espaço de nomes principais para secundários
    - `Set-AzureRmServiceBusDRConfigurationsBreakPairing`
  - Invocar a ativação pós-falha da Recuperação Após Desastre e reconfigurar o alias de modo a apontar para o espaço de nomes secundário
    - `Set-AzureRmServiceBusDRConfigurationsFailOver`
  - Eliminar um Alias (configuração da Recuperação Após Desastre)
    - `Remove-AzureRmServiceBusDRConfigurations`
* `Test-AzureRmServiceBusName` commandlets atualizados para suportar as operações de verificação de disponibilidade do nome da Recuperação Após Desastre Georredundante - Alias.
  - Verificar a disponibilidade do nome do Espaço de Nomes ou do nome do Alias (configuração da Recuperação Após Desastre):
    - `Test-AzureRmServiceBusName`

### <a name="azurermusageaggregates"></a>AzureRM.UsageAggregates
* Corrigida a utilização de `Login-AzureRmAccount` para utilizar `Connect-AzureRmAccount`

## <a name="520---january-2018"></a>5.2.0 - Janeiro de 2018
#### <a name="azurermprofile"></a>AzureRM.Profile
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* Add-AzureRmAccount
  * Foi adicionado o início de sessão -MSI para autenticação com as credenciais da Identidade do Serviço Gerido da VM/Serviço atual
  * Foi corrigida a Autenticação KeyVault ao iniciar sessão com tokens de acesso fornecidos pelo utilizador

#### <a name="azurestorage"></a>Azure.Storage
* Foram adicionados cmdlets para obter e definir as propriedades do Serviço de armazenamento
    - Get-AzureStorageServiceProperty
    - Update-AzureStorageServiceProperty

#### <a name="azurermanalysisservices"></a>AzureRM.AnalysisServices
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermapimanagement"></a>AzureRM.ApiManagement
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* -Tags Obsoletas a favor de -Tag para New-AzureRmApiManagementProperty, Set-AzureRmApiManagementProperty e New-AzureRmApiManagement

#### <a name="azurermapplicationinsights"></a>AzureRM.ApplicationInsights
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermautomation"></a>AzureRM.Automation
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* -Tags obsoletas a favor de -Tag para Set-AzureRmAutomationRunbook

#### <a name="azurermbackup"></a>AzureRM.Backup
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermbatch"></a>AzureRM.Batch
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermcdn"></a>AzureRM.Cdn
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* -Tags obsoletas a favor de -Tag para New-AzureRmCdnEndpoint e New-AzureRmCdnProfile

#### <a name="azurermcognitiveservices"></a>AzureRM.CognitiveServices
* Integração na versão 3.0.0 do SDK da Gestão dos Serviços Cognitivos.

#### <a name="azurermcompute"></a>AzureRM.Compute
* Foi adicionado o conjunto de parâmetros simplificados a New-AzureRmVmss, que cria um Conjunto de Dimensionamento de Máquinas Virtuais e todos os recursos necessários com predefinições inteligentes
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* -Tags obsoletas a favor de -Tag para New-AzureRmVm e Update-AzureRmVm
* Foi corrigido o cmdlet Get-AzureRmComputeResourceSku quando a Zona está incluída na restrição.
* Foi atualizado o esquema da configuração do Agente de Diagnósticos para o suporte de sink do Azure Monitor.

#### <a name="azurermcontainerinstance"></a>AzureRM.ContainerInstance
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermcontainerregistry"></a>AzureRM.ContainerRegistry
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermdatafactories"></a>AzureRM.DataFactories
* Foi ativado o suporte do Azure Key Vault para todos os serviços ligados de arquivo de dados
* Foi adicionada a propriedade do tipo de licença para o runtime de integração do SSIS do Azure
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* -Tags obsoletas a favor de -Tag para New-AzureRmDataFactory

#### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* Foi ativado o suporte do Azure Key Vault para todos os serviços ligados de arquivo de dados
* Foi adicionada a propriedade do tipo de licença para o runtime de integração do SSIS do Azure
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* Foi adicionado o parâmetro "LicenseType" para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para ativar a funcionalidade AHUB

#### <a name="azurermdatalakeanalytics"></a>AzureRM.DataLakeAnalytics
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* -Tags obsoletas a favor de -Tag para New-AzureRmDataLakeAnalyticsAccount e Set-AzureRmDataLakeAnalyticsAccount

#### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* -Tags obsoletas a favor de -Tag para New-AzureRmDataLakeStoreAccount e Set-AzureRmDataLakeStoreAccount

#### <a name="azurermdevtestlabs"></a>AzureRM.DevTestLabs
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermdns"></a>AzureRM.Dns
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermeventgrid"></a>AzureRM.EventGrid
* Foi adicionado o novo cmdlet seguinte:
  - Update-AzureRmEventGridSubscription
    - Atualize as propriedades de uma subscrição de eventos do Event Grid.
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermeventhub"></a>AzureRM.EventHub
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermhdinsight"></a>AzureRM.HDInsight
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurerminsights"></a>AzureRM.Insights
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermiothub"></a>AzureRM.IotHub
* Adicionado suporte de Certificado para os cmdlets do IoTHub
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* Foi adicionado o suporte -AsJob para cmdlets de KeyVault de execução longa. Permite que os cmdlets selecionados executem no fundo e devolvam uma tarefa para controlar e rastrear o progresso.
  * O cmdlet afetado é: Remove-AzureRmKeyVault
* Foi corrigido o erro em Set-AzureRmKeyVaultAccessPolicy, em que o filtro AAD definia o SPN para o UPN fornecido, em vez de definir o UPN
  - Veja o problema seguinte para obter mais informações: https://github.com/Azure/azure-powershell/issues/5201

#### <a name="azurermlogicapp"></a>AzureRM.LogicApp
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermmachinelearning"></a>AzureRM.MachineLearning
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* -Tags obsoletas a favor de -Tag para Update-AzureRmMlCommitmentPlan

#### <a name="azurermmachinelearningcompute"></a>AzureRM.MachineLearningCompute
* Foi adicionado o parâmetro IncludeAllResources ao cmdlet Remove-AzureRmMlOpCluster
  - Utilizar este parâmetro opcional irá remover todos os recursos que foram criados originalmente com o cluster
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermmedia"></a>AzureRM.Media
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* -Tags obsoletas a favor de -Tag para Set-AzureRmMediaService e New-AzureRmMediaService

#### <a name="azurermnetwork"></a>AzureRM.Network
* Foi adicionado o suporte -AsJob para cmdlets de Rede de execução longa. Permite que os cmdlets selecionados executem no fundo e devolvam uma tarefa para controlar e rastrear o progresso.
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermnotificationhubs"></a>AzureRM.NotificationHubs
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* -Tags obsoletas a favor de -Tag para New-AzureRmNotificationHubsNamespace e Set-AzureRmNotificationHubsNamespace

#### <a name="azurermoperationalinsights"></a>AzureRM.OperationalInsights
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* -Tags obsoletas a favor de -Tag para New-AzureRmOperationalInsightsSavedSearch, Set-AzureRmOperationalInsightsSavedSearch, New-AzureRmOperationalInsightsWorkspace e Set-AzureRmOperationalInsightsWorkspace

#### <a name="azurermpowerbiembedded"></a>AzureRM.PowerBIEmbedded
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermrecoveryservices"></a>AzureRM.RecoveryServices
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermrecoveryservicesbackup"></a>AzureRM.RecoveryServices.Backup
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* Foi adicionada a opção -UseOriginalStorageAccount ao cmdlet Restore-AzureRmRecoveryServicesBackupItem.
  - Ativar este sinalizador resulta no restauro dos discos para as respetivas contas de armazenamento originais, o que permite aos utilizadores manter a configuração da VM restaurada o mais próximo possível das VMs originais.
  - Também ajuda a melhorar o desempenho da operação de restauro.

#### <a name="azurermrediscache"></a>AzureRM.RedisCache
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* Foram adicionados 3 novos cmdlets para regras de firewall
* Foram adicionados 3 novos cmdlets para georreplicação
* Foi adicionado suporte para zonas e etiquetas
* Torne o ResourceGroup opcional sempre que possível.

#### <a name="azurermrelay"></a>AzureRM.Relay
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermresources"></a>AzureRM.Resources
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* Foi adicionado o suporte -AsJob para cmdlets de Recursos de execução longa. Permite que os cmdlets selecionados executem no fundo e devolvam uma tarefa para controlar e rastrear o progresso.
* Foi adicionado um alias de Get-AzureRmProviderOperation a Get-AzureRmResourceProviderAction para estar em conformidade com as convenções de nomenclatura

#### <a name="azurermscheduler"></a>AzureRM.Scheduler
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermservermanagement"></a>AzureRM.ServerManagement
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* -Tags obsoletas a favor de -Tag para New-AzureRmServerManagementNode e New-AzureRmServerManagementGateway

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermsiterecovery"></a>AzureRM.SiteRecovery
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermsql"></a>AzureRM.Sql
* Atualizar a descrição dos parâmetros dos comandos de Auditoria
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* Foi adicionado o parâmetro -AsJob a cmdlets de execução longa
* Parâmetro -DatabaseName obsoleto de Get-AzureRmSqlServiceObjective

#### <a name="azurermstorage"></a>AzureRM.Storage
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* Foi corrigido um problema de referência nula da execução do cmdlet New-AzureRMStorageAccount com o parâmetro -EnableEncryptionService None
* Foi adicionado o suporte -AsJob para cmdlets de Armazenamento de execução longa. Permite que os cmdlets selecionados executem no fundo e devolvam uma tarefa para controlar e rastrear o progresso.
    - Os cmdlets afetados são New-, Remove-, Add- e Update- para a Conta de Armazenamento e a Regra de Rede da Conta de Armazenamento.

#### <a name="azurermstreamanalytics"></a>AzureRM.StreamAnalytics
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermtrafficmanager"></a>AzureRM.TrafficManager
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual

#### <a name="azurermwebsites"></a>AzureRM.Websites
* Foi adicionada a Conclusão de Localização aos parâmetros -Location, o que permite a conclusão de tabulação através de Localizações válidas
* Foi adicionada a Conclusão de ResourceGroup aos parâmetros -ResourceGroup, o que permite a conclusão de tabulação através de grupos de recursos na subscrição atual
* Foi adicionado o suporte -AsJob para cmdlets de Sites de execução longa. Permite que os cmdlets selecionados executem no fundo e devolvam uma tarefa para controlar e rastrear o progresso.
     - Os cmdlets afetados são New-, Remove-, Add- e Set- para WebApps, AppServicePlan e Slots

## <a name="2017128-version-511"></a>2017.12.8 Versão 5.1.1
* AnalysisServices
  - Alterar o conjunto de validação da localização para uma pesquisa dinâmica para que todas as cloud sejam suportadas.
* Automatização
  - Atualizar para Import-AzureRMAutomationRunbook
    - O suporte está agora a ser fornecido para runbooks do Python2
* Batch
  - Foi corrigido um erro em que as operações de conta sem um grupo de recursos falharam a deteção automática do grupo de recursos
* Computação
  - Get-AzureRmComputeResourceSku mostra as informações da zona.
  - Atualize Disable-AzureRmVmssDiskEncryption para corrigir o problema https://github.com/Azure/azure-powershell/issues/5038
  - Foi adicionado suporte de -AsJob para cmdlets de Computação de execução longa. Permite que os cmdlets selecionados executem no fundo e devolvam uma tarefa para controlar e rastrear o progresso.
    - Os cmdlets afetados incluem: New-, Update-, Set-, Remove-, Start-, Restart-, Stop- para Máquinas Virtuais e Conjuntos de Dimensionamento de Máquinas Virtuais
    - Foi adicionado o conjunto de parâmetros simplificados para New-AzureRmVM, que cria uma Máquina Virtual e todos os recursos necessários com predefinições inteligentes
* ContainerInstance
  - Aplicar o SDK de 01-10-2017 da Instância de Contentor do Azure
    - Suporta a execução até conclusão dos contentores
    - Suportar montagem de volume de Ficheiro do Azure
    - Suporta a abertura de várias portas para IP público
* ContainerRegistry
  - Novos cmdlets para georreplicação e webhooks
    - Get/New/Remove-AzureRmContainerRegistryReplication
    - Get/New/Remove/Test/Update-AzureRmContainerRegistryWebhook
* DataFactories
    - A funcionalidade de encriptação de credenciais agora funciona com ambos "Acesso Remoto" ativado (Pela Rede) e "Acesso Remoto" desativado (Máquina Local).
* DataFactoryV2
  - Foram adicionados dois novos cmdlets: Update-AzureRmDataFactoryV2 e Stop-AzureRmDataFactoryV2PipelineRun
* DataLakeAnalytics
  - Adicionado um parâmetro chamado ScriptParameter a Submit-AzureRmDataLakeAnalyticsJob
    - Podem ser encontradas informações detalhadas sobre ScriptParameter ao utilizar Get-Help em Submit-AzureRmDataLakeAnalyticsJob
  - Para New-AzureRmDataLakeAnalyticsAccount, foi alterado o parâmetro MaxDegreeOfParallelism para MaxAnalyticsUnits
    - Foi adicionado um alias ao parâmetro MaxAnalyticsUnits: MaxDegreeOfParallelism
  - Para New-AzureRmDataLakeAnalyticsComputePolicy, foi alterado o parâmetro MaxDegreeOfParallelismPerJob para MaxAnalyticsUnitsPerJob
    - Foi adicionado um alias ao parâmetro MaxAnalyticsUnitsPerJob: MaxDegreeOfParallelismPerJob
  - Para Set-AzureRmDataLakeAnalyticsAccount, foi alterado o parâmetro MaxDegreeOfParallelism para MaxAnalyticsUnits
    - Foi adicionado um alias ao parâmetro MaxAnalyticsUnits: MaxDegreeOfParallelism
  - Para Submit-AzureRmDataLakeAnalyticsJob, foi alterado o parâmetro DegreeOfParallelism para AnalyticsUnits
    - Foi adicionado um alias ao parâmetro AnalyticsUnits: DegreeOfParallelism
  - Para Update-AzureRmDataLakeAnalyticsComputePolicy, foi alterado o parâmetro MaxDegreeOfParallelismPerJob para MaxAnalyticsUnitsPerJob
    - Foi adicionado um alias ao parâmetro MaxAnalyticsUnitsPerJob: MaxDegreeOfParallelismPerJob
* MachineLearningCompute
  - Adicionar Set-AzureRmMlOpCluster
    - Atualizar a contagem de agentes de um cluster ou a configuração de SSL
  - As propriedades do orquestrador são opcionais
    - O serviço vai criar um principal de serviço se não for fornecido, pelo que as propriedades do orquestrador agora são opcionais
* PowerBIEmbedded
  - Adicionar suporte aos cmdlets do Power BI Embedded Capacity
  - O novo Cmdlet Get-AzureRmPowerBIEmbeddedCapacity - obtém os detalhes de um PowerBI Embedded Capacity.
  - O novo Cmdlet New-AzureRmPowerBIEmbeddedCapacity - cria um novo PowerBI Embedded Capacity
  - O novo Cmdlet Remove-AzureRmPowerBIEmbeddedCapacity - elimina uma instância do PowerBI Embedded Capacity
  - O novo Cmdlet Resume-AzureRmPowerBIEmbeddedCapacity - continua uma instância do PowerBI Embedded Capacity
  - O novo Cmdlet Suspend-AzureRmPowerBIEmbeddedCapacity - suspende uma instância do PowerBI Embedded Capacity
  - O novo Cmdlet Test-AzureRmPowerBIEmbeddedCapacity - testa a existência de uma instância do PowerBI Embedded Capacity
  - O novo Cmdlet Update-AzureRmPowerBIEmbeddedCapacity - modifica uma instância do PowerBI Embedded Capacity
* Perfil
  - USGovernmentActiveDirectoryEndpoint atualizado para https://login.microsoftonline.us/
    - Para obter mais informações sobre os mapeamentos de ponto final do Azure Government, veja o seguinte: https://docs.microsoft.com/azure/azure-government/documentation-government-developer-guide#endpoint-mapping
    - Foi adicionado suporte ao -AsJob para os cmdlets, que permite que determinados cmdlets executem em fundo e devolvam uma tarefa para rastrear e controlar o progresso
    - Foi adicionado o parâmetro -AsJob ao cmdlet Get-AzureRmSubscription
* RecoveryServices.Backup
  - Foi corrigido o erro - Get-AzureRmRecoveryServicesBackupItem deve ser feita uma comparação não sensível a maiúsculas e minúsculas para o filtro do nome do contentor.
  - Foi corrigido o erro -AzureVmItem agora tem uma propriedade que mostra a última hora em que uma operação de cópia de segurança ocorreu - LastBackupTime.
* Recursos
  - Foi corrigido o erro em que Get-AzureRMRoleAssignment resultaria numa atribuição sem nome de definição de funções para funções personalizadas
    - Os utilizadores podem agora utilizar Get-AzureRMRoleAssignment com atribuições com nomes de definição de funções, sem relação ao tipo de função
  - Foi corrigido o erro em que Set-AzureRMRoleRoleDefinition foi utilizado para lançar o erro não encontrado RD quando existiu um novo âmbito assignablescopes
    - Os utilizadores podem agora utilizar Set-AzureRMRoleRoleDefinition com âmbitos atribuíveis, incluindo novos âmbitos, independentemente da posição do âmbito
  - Permitir que os âmbitos terminem com "/"
    - Os utilizadores agora podem utilizar os commandlets RoleDefinition e RoleAssignment com âmbitos que terminem com "/", consistentes com a API e a CLI
  - Permitir aos utilizadores criar RoleAssignment utilizando o sinalizador de delegação
    - Os utilizadores podem agora utilizar New-AzureRMRoleAssignment com uma opção para adicionar o sinalizador de delegação
  - Corrigir RoleAssignment get para corresponder ao parâmetro do âmbito
  - Adicionar um alias ao ServicePrincipalName no commandlet New-AzureRmRoleAssignment
    - Os utilizadores agora podem utilizar o ApplicationId em vez do ServicePrincipalName ao utilizar o commandlet New-AzureRmRoleAssignment
* SiteRecovery
  - Adicione avisos de preterição para todos os cmdlets neste módulo em forma de preparação para o lançamento da próxima grande versão.
    - Consulte o nosso guia de alterações principais para mais informações sobre como migrar os seus cmdlets do AzureRM.
* SQL
  - Foi adicionada a capacidade de alterar o nome da base de dados com Set-AzureRmSqlDatabase
  - Problema https://github.com/Azure/azure-powershell/issues/4974 corrigido
    - Fornecer o valor AUDIT_CHANGED_GROUP inválido para os cmdlets de auditoria já não lança um erro e vai ser removido numa futura versão.
  - Problema https://github.com/Azure/azure-powershell/issues/5046 corrigido
    - O parâmetro AuditAction já não está a ser ignorado
  - Foi corrigido um problema nos cmdlets de Auditoria quando é fornecido o StorageKeyType "Secondary"
    - Ao definir a auditoria de blob, a chave de conta de armazenamento primária foi utilizada em vez da chave secundária ao fornecer o valor "Secondary" ao parâmetro StorageKeyType.
  - Alterar as palavras utilizadas para a mensagem de confirmação de Set-AzureRmSqlServerTransparentDataEncryptionProtector
* Azure (RDFE)
    - Remover todos os Cmdlets do RemoteApp
* Azure.Storage
    - Atualizar para a Biblioteca de Clientes do Armazenamento do Azure 8.6.0 e a Biblioteca de DataMovement do Armazenamento do Azure 0.6.5

## <a name="20171110-version-501"></a>2017.11.10 Versão 5.0.1
* Corrigido problema de carregamento de assemblagem que causou a falha de alguns cmdlets ao executar os seguintes módulos:
  - AzureRM.ApiManagement
  - AzureRM.Backup
  - AzureRM.Batch
  - AzureRM.Compute
  - AzureRM.DataFactories
  - AzureRM.HDInsight
  - AzureRM.KeyVault
  - AzureRM.RecoveryServices
  - AzureRM.RecoveryServices.Backup
  - AzureRM.RecoveryServices.SiteRecovery
  - AzureRM.RedisCache
  - AzureRM.SiteRecovery
  - AzureRM.Sql
  - AzureRM.Storage
  - AzureRM.StreamAnalytics

## <a name="2017118---version-500"></a>2017.11.8 - Versão 5.0.0
* NOTA: esta é uma versão com uma alteração interruptiva. Veja o guia de migração (https://aka.ms/azps-migration-guide) para obter uma lista completa das alterações interruptivas apresentadas.
* Todos os cmdlets no AzureRM suportam agora ajuda online
  - Execute Get-Help com o parâmetro -Online para abrir a ajuda online no seu browser da Internet predefinido
* AnalysisServices
  * Comando Synchronize-AzureAsInstance corrigido para funcionar com a nova API REST AsAzure para sincronização
* ApiManagement
  * Veja o guia de migração de quebras de código realizadas no ApiManagement nesta versão
  * Cmdlet Get-AzureRmApiManagementUser atualizado para corrigir o problema https://github.com/Azure/azure-powershell/issues/4510
  * Cmdlet New-AzureRmApiManagementApi atualizado para criar Api com Caminho Vazio https://github.com/Azure/azure-powershell/issues/4069
* ApplicationInsights
  * Adicionar comandos para obter/criar/remover recursos do application insights
    - Get-AzureRmApplicationInsights
    - New-AzureRmApplicationInsights
    - Remove-AzureRmApplicationInsights
  * Adicionar comandos para obter/atualizar preços/limite diário de recursos do application insights
    - Get-AzureRmApplicationInsights -IncludeDailyCap
    - Set-AzureRmApplicationInsightsPricingPlan
    - Set-AzureRmApplicationInsightsDailyCap
  * Adicionar comandos para obter/criar/atualizar/remover exportação contínua de recursos do application insights
    - Get-AzureRmApplicationInsightsContinuousExport
    - Set-AzureRmApplicationInsightsContinuousExport
    - New-AzureRmApplicationInsightsContinuousExport
    - Remove-AzureRmApplicationInsightsContinuousExport
  * Adicionar comandos para obter/criar/remover chaves de api de recursos do application insights
    - Get-AzureRmApplicationInsightsApiKey
    - New-AzureRmApplicationInsightsApiKey
    - Remove-AzureRmApplicationInsightsApiKey
* AzureBatch
  * Adicionados novos parâmetros a `New-AzureRmBatchAccount`.
    - `PoolAllocationMode`: O modo de alocação a utilizar para criar conjuntos na conta do Batch. Para criar uma conta do Batch que aloca nós do conjunto na subscrição do utilizador, defina esta opção para `UserSubscription`.
    - `KeyVaultId`: O ID de recurso do cofre de chaves do Azure associado à conta do Batch.
    - `KeyVaultUrl`: O URL do cofre de chaves do Azure associado à conta do Batch.
  * Parâmetros atualizados para `New-AzureBatchTask`.
    - Mudança `RunElevated` removida. O parâmetro `UserIdentity` foi adicionado ao substituir `RunElevated`, e o comportamento equivalente pode ser alcançado ao construir um `PSUserIdentity` conforme mostrado abaixo:
      - $autoUser = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoUserSpecification -ArgumentList @("Tarefa", "Administrador")
      - $userIdentity = New-Object Microsoft.Azure.Commands.Batch.Models.PSUserIdentity $autoUser
    - Parâmetro `AuthenticationTokenSettings` adicionado. Este parâmetro permite-lhe pedir ao serviço do Batch para fornecer um token de autenticação à tarefa quando é executada, evitando a necessidade de passar chaves da conta do Batch para a tarefa, de forma a emitir pedidos para o serviço do Batch.
    - Parâmetro `ContainerSettings` adicionado.
      - Este parâmetro permite-lhe pedir ao serviço do Batch para realizar a tarefa dentro de um contentor.
    - Parâmetro `OutputFiles` adicionado.
      - Este parâmetro permite-lhe configurar a tarefa para carregar ficheiros para o Armazenamento do Azure após ter terminado.
  * Parâmetros atualizados para `New-AzureBatchPool`.
    - Parâmetro `UserAccounts` adicionado.
      - Este parâmetro define as contas de utilizador criadas em cada nó no conjunto.
    - `TargetLowPriorityComputeNodes` adicionado e `TargetDedicated` renomeado para `TargetDedicatedComputeNodes`.
      - Foi criado um alias `TargetDedicated` para o parâmetro `TargetDedicatedComputeNodes`.
    - Parâmetro `NetworkConfiguration` adicionado.
      - Este parâmetro permite-lhe configurar as definições de rede de conjuntos.
  * Parâmetros atualizados para `New-AzureBatchCertificate`.
    - O parâmetro `Password` é agora um `SecureString`.
  * Parâmetros atualizados para `New-AzureBatchComputeNodeUser`.
    - O parâmetro `Password` é agora um `SecureString`.
  * Parâmetros atualizados para `Set-AzureBatchComputeNodeUser`.
    - O parâmetro `Password` é agora um `SecureString`.
  * Parâmetro `Name` renomeado para `Path` no `Get-AzureBatchNodeFile`, `Get-AzureBatchNodeFileContent` e `Remove-AzureBatchNodeFile`.
    - Foi criado um alias `Name` para o parâmetro `Path`.
  * Alterações a objetos
    - Veja o registo de alterações do Batch para obter a lista completa
  * Suporte adicionado para a autenticação baseada no Azure Active Directory.
    - Para utilizar a autenticação do Azure Active Directory, obtenha um objeto `BatchAccountContext` com o cmdlet `Get-AzureRmBatchAccount` e forneça este `BatchAccountContext` ao parâmetro `-BatchContext` de um cmdlet do serviço do Batch. A autenticação do Azure Active Directory é obrigatória para contas com `PoolAllocationMode = UserSubscription`.
    - Para as contas existentes ou para novas contas criadas com `PoolAllocationMode = BatchService`, pode continuar a utilizar a autenticação de chave partilhada ao obter um objeto `BatchAccountContext` com o cmdlet `Get-AzureRmBatchAccoutKeys`.
* Computação
  * Comandos de Extensão do Azure Disk Encryption
    - Novo parâmetro para "Set-AzureRmVmDiskEncryptionExtension": "-EncryptFormatAll" discos de dados com formatos encriptados
    - Novos parâmetros para "Set-AzureRmVmDiskEncryptionExtension": "-ExtensionPublisherName" e "-ExtensionType" permitirem a mudança para outras versões da extensão
    - Novos parâmetros para "Disable-AzureRmVmDiskEncryption": "-ExtensionPublisherName" e "-ExtensionType" permitirem a mudança para outras versões da extensão
    - Novos parâmetros para "Get-AzureRmVmDiskEncryptionStatus": "-ExtensionPublisherName" e "-ExtensionType" permitirem a mudança para outras versões da extensão
* DataLakeAnalytics
  * Veja o guia de migração de quebras de código realizadas no DataLakeAnalytics nesta versão
  * Alterado um dos dois OutputTypes de Get-AzureRmDataLakeAnalyticsAccount
    - Lista\<DataLakeAnalyticsAccount> para Lista\<PSDataLakeAnalyticsAccountBasic>
    - As propriedades de PSDataLakeAnalyticsAccountBasic são um subconjunto estrito das propriedades do DataLakeAnalyticsAccount
    - As propriedades adicionais que se encontram no DataLakeAnalyticsAccount não são devolvidas pelo serviço.  Por conseguinte, esta alteração serve para refletir isto com exatidão. Estas propriedades adicionais ainda estão no PSDataLakeAnalyticsAccountBasic, mas estão etiquetadas como Obsoleto.
  * Alterado um dos dois OutputTypes de Get-AzureRmDataLakeAnalyticsJob
    - Lista\<JobInformation> para Lista\<PSJobInformationBasic>
    - As propriedades de PSJobInformationBasic são um subconjunto estrito das propriedades de JobInformation
    - As propriedades adicionais que se encontrem no JobInformation não são devolvidas pelo serviço.  Por conseguinte, esta alteração serve para refletir isto com exatidão. Estas propriedades adicionais ainda estão no PSJobInformationBasic, mas estão etiquetadas como Obsoleto.
* DataLakeStore
  * Veja o guia de migração de quebras de código realizadas no DataLakeStore nesta versão
  * Alterado um dos dois OutputTypes de Get-AzureRmDataLakeStoreAccount
    - Lista\<PSDataLakeStoreAccount> para Lista\<PSDataLakeStoreAccountBasic>
    - As propriedades de PSDataLakeStoreAccountBasic são um subconjunto estrito das propriedades do PSDataLakeStoreAccount
    - As propriedades adicionais que se encontrem no PSDataLakeStoreAccount não são devolvidas pelo serviço.  Por conseguinte, esta alteração serve para refletir isto com exatidão. Estas propriedades adicionais ainda estão no PSDataLakeStoreAccountBasic, mas estão etiquetadas como Obsoleto.
* Dns
  * Suporte para tipos de registo de CAA no DNS do Azure
    - Suporta todas as operações no tipo de registo CAA
* EventHub
  * Veja o guia de migração de quebras de código realizadas no EventHub nesta versão
* Informações
  * Veja o guia de migração de quebras de código realizadas no Insights nesta versão
* Rede
  * Veja o guia de migração de quebras de código realizadas no Network nesta versão
  * Cmdlet adicionado à lista de fornecedores de serviços de Internet disponíveis para uma região do Azure especificada
    - Get-AzureRmNetworkWatcherReachabilityProvidersList
  * Cmdlet adicionado para obter a classificação de latência relativa para fornecedores de serviços de Internet a partir de uma localização especificada para regiões do Azure
    - Get-AzureRmNetworkWatcherReachabilityReport
* Perfil
  - Set-AzureRmDefault
    - Utilize este cmdlet para definir um grupo de recursos predefinido.  Isto tornará o parâmetro -ResourceGroup opcional para alguns cmdlets e utilizará a predefinição quando não for especificado um grupo de recursos
    - ```Set-AzureRmDefault -ResourceGroupName "ExampleResourceGroup"```
    - Se o grupo de recursos especificado existe na subscrição, este grupo de recursos será definido como predefinido.  Caso contrário, o grupo de recursos será criado e, em seguida, definido como predefinido.
  - Get-AzureRmDefault
    - Utilize este cmdlet para obter o grupo de recursos predefinidos atual (e outras predefinições no futuro).
    - ```Get-AzureRmDefault -ResourceGroup```
  - Clear-AzureRmDefault
    - Utilize este cmdlet para remover o grupo de recursos predefinidos atual
    - ```Clear-AzureRmDefault -ResourceGroup```
  - Add-AzureRmEnvironment e Set-AzureRmEnvironment
    - Adicione o parâmetro BatchAudience, que lhe permite especificar o público-alvo do Azure Batch Active Directory a utilizar ao adquirir os tokens de autenticação para o serviço do Batch.
* RecoveryServices.Backup
  * Foram adicionados cmdlets para realizar a recuperação instantânea de ficheiros.
    - Get-AzureRmRecoveryServicesBackupRPMountScript
    - Disable-AzureRmRecoveryServicesBackupRPMountScript
  * Versão atualizada do SDK RecoveryServices.Backup para a versão mais recente
  * Testes atualizados para a carga de trabalho da VM do Azure, para que todas as configurações necessárias para execuções de testes sejam realizadas pelos próprios testes.
  * Correções https://github.com/Azure/azure-powershell/issues/3164
* RecoveryServices.SiteRecovery
  * Alterações do ASR VMware para o Azure Site Recovery (os cmdlets suportam atualmente operações de Enterprise para Enterprise, Enterprise para Azure, HyperV para Azure)
    - New-AzureRmRecoveryServicesAsrPolicy
    - New-AzureRmRecoveryServicesAsrProtectedItem
    - Update-AzureRmRecoveryServicesAsrPolicy
    - Update-AzureRmRecoveryServicesAsrProtectionDirection
  * Suporte adicionado para cofre baseado em AAD
  * Cmdlets adicionados para gerir os recursos do VCenter
    - Get-AzureRmRecoveryServicesAsrVCenter
    - New-AzureRmRecoveryServicesAsrVCenter
    - Remove-AzureRmRecoveryServicesAsrVCenter
    - Update-AzureRmRecoveryServicesAsrVCenter
  * Adicionados outros cmdlets
    - Get-AzureRmRecoveryServicesAsrAlertSetting
    - Get-AzureRmRecoveryServicesAsrEvent
    - New-AzureRmRecoveryServicesAsrProtectableItem
    - Set-AzureRmRecoveryServicesAsrAlertSetting
    - Start-AzureRmRecoveryServicesAsrResynchronizeReplicationJob
    - Start-AzureRmRecoveryServicesAsrSwitchProcessServerJob
    - Start-AzureRmRecoveryServicesAsrTestFailoverCleanupJob
    - Update-AzureRmRecoveryServicesAsrMobilityService
* ServiceBus
  - Veja o guia de migração de quebras de código realizadas no ServiceBus nesta versão
* SQL
  * A adicionar suporte para a lista e cancelar a operação assíncrona updateslo na base de dados
    - atualizar cmdlet existente Get-AzureRmSqlDatabaseActivity para devolver o estado da operação updateslo da base de dados.
    - adicionar novo cmdlet Stop-AzureRmSqlDatabaseActivity para cancelar a operação assíncrona updateslo na base de dados.
  * A adicionar suporte para a Redundância de Zona para conjuntos elásticos e bases de dados
    - A adicionar parâmetro de mudança ZoneRedundant para New-AzureRmSqlDatabase
    - A adicionar parâmetro de mudança ZoneRedundant para Set-AzureRmSqlDatabase
    - A adicionar parâmetro de mudança ZoneRedundant para New-AzureRmSqlElasticPool
    - A adicionar parâmetro de mudança ZoneRedundant para Set-AzureRmSqlElasticPool
  * Adicionar suporte para Aliases de DNS do Servidor
    - A adicionar o cmdlet Get-AzureRmSqlServerDnsAlias que obtém os aliases de dns do servidor por servidor e o nome de alias ou uma lista de aliases de dns do servidor para um Servidor Sql do azure.
    - A adicionar o cmdlet New-AzureRmSqlServerDnsAlias, que cria o novo alias de dns do servidor para um determinado servidor Sql do Azure
    - A adicionar cmdlet Set-AzurermSqlServerDnsAlias que lhe permite atualizar um Servidor Sql do Azure para o alias de dns de servidor que está a apontar
    - A adicionar o cmdlet Remove-AzureRmSqlServerDnsAlias, que remove um alias de dns de servidor para um servidor Sql do Azure
* Azure.Storage
  * Atualizar para a Biblioteca de Clientes do Armazenamento do Azure 8.5.0 e a Biblioteca de DataMovement do Armazenamento do Azure 0.6.3
  * Funcionalidade de Suporte de Instantâneo de Partilha de Ficheiros
    - Adicionar parâmetro "SnapshotTime" a Get-AzureStorageShare
    - Adicionar parâmetro "IncludeAllSnapshot" a Remove-AzureStorageShare
