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
ms.date: 2/20/2018
ms.openlocfilehash: f726559915d8c68469a88126f73f17c3cca5c7b4
ms.sourcegitcommit: 5fe9a579d2e0d1cb5a05aadaeba5db784f1b18fa
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/28/2018
---
# <a name="release-notes"></a>Notas de versão

Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.

---

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
    - New-AzureRmApplicationGateway atualizado: Parâmetro opcional adicionado -EnableHttp2
* Adicionar IpTags a PublicIpAddress
    - New-AzureRmPublicIpAddress atualizado: IpTags adicionado
    - New-AzureRmPublicIpTag para adicionar Iptag
* Adicione a propriedade DisableBgpRoutePropagation ao RouteTable e effectiveRoute.

#### <a name="azurermresources"></a>AzureRM.Resources
* Register-AzureRmProviderFeature: exemplo em falta adicionado aos documentos
* Register-AzureRmResourceProvider: exemplo em falta adicionado aos documentos

#### <a name="azurermstorage"></a>AzureRM.Storage
* Parâmetros seguintes obsoletos em cmdlets novos e definidos da Conta de Armazenamento: EnableEncryptionService e DisableEncryptionService, uma vez que a Encriptação Inativa está ativada por predefinição e não pode ser desativada.
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
    -Criar um novo Alias (configuração de Recuperação Após Desastre):- `New-AzureRmEventHubGeoDRConfiguration` - Obter Alias (configuração de Recuperação Após Desastre): - `Get-AzureRmEventHubGeoDRConfiguration` -Desativar a Recuperação Após Desastre e parar de replicar alterações de nomes de espaço primários a secundários - `Set-AzureRmEventHubGeoDRConfigurationBreakPair` -Invocar a ativação pós-falha de Recuperação Após Desastre e reconfigurar o alias para apontar para o nome de espaços secundário - `Set-AzureRmEventHubGeoDRConfigurationFailOver` -Eliminar um Alias (configuração de Recuperação Após Desastre) - `Remove-AzureRmEventHubGeoDRConfiguration`
* Adicionados novos comandos ao verificar o Nome do Espaço de Nomes e Nome de Configuração GeoDR - disponibilidade de Alias.
    -Verifica a Disponibilidade do nome do Espaço de Nomes ou nome de Alias (configuração de Recuperação Após Desastres): - `Test-AzureRmEventHubName`

### <a name="azurerminsights"></a>AzureRM.Insights
* Corrigida a utilização de `Login-AzureRmAccount` para utilizar `Connect-AzureRmAccount`

### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Corrigida a utilização de `Login-AzureRmAccount` para utilizar `Connect-AzureRmAccount`

### <a name="azurermnetwork"></a>AzureRM.Network
* Corrige a mensagem de substituição "Quer mesmo substituir o recurso"

#### <a name="azurermoperationalinsights"></a>AzureRM.OperationalInsights
* Suporte adicionado para a consulta da API V2 via `Invoke-AzureRmOperationalInsightsQuery`. Consulte [https://dev.loganalytics.io/](https://dev.loganalytics.io/) para obter mais informações sobre a nova API.

### <a name="azurermresources"></a>AzureRM.Resources
* `Get-AzureRmADServicePrincipal`: `-ServicePrincipalName` removido do parâmetro Vazio predefinido dado que era redundante com o parâmetro SPN definido

### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* Adicionada a correção de funcionalidade para `Remove-AzureRmServiceBusRule` e `Get-AzureRmServiceBusKey`
* Adicionados os novos commandlets abaixo para operações de Recuperação Após Desastre Georredundante.
    -Criar um novo Alias (configuração de Recuperação Após Desastre):- `New-AzureRmServiceBusDRConfigurations` - Obter Alias (configuração de Recuperação Após Desastre): - `Get-AzureRmServiceBusDRConfigurations` -Desativar a Recuperação Após Desastre e parar de replicar alterações de nomes de espaço primários a secundários - `Set-AzureRmServiceBusDRConfigurationsBreakPairing` -Invocar a ativação pós-falha de Recuperação Após Desastre e reconfigurar o alias para apontar para o nome de espaços secundário - `Set-AzureRmServiceBusDRConfigurationsFailOver` -Eliminar um Alias (configuração de Recuperação Após Desastre) - `Remove-AzureRmServiceBusDRConfigurations`
* `Test-AzureRmServiceBusName` commandlets atualizados para suportar as operações de verificação de disponibilidade do nome da Recuperação Após Desastre Georredundante - Alias.
    -Verifica a Disponibilidade do nome do Espaço de Nomes ou nome de Alias (configuração de Recuperação Após Desastres): - `Test-AzureRmServiceBusName`

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
   - Veja o seguinte problema para obter mais informações: https://github.com/Azure/azure-powershell/issues/5201

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
    - Adicionados dois novos cmdlets: Update-AzureRmDataFactoryV2 e Stop-AzureRmDataFactoryV2PipelineRun
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
    - Foi atualizado USGovernmentActiveDirectoryEndpoint para https://login.microsoftonline.us/
        - Para obter mais informações sobre os mapeamentos dos pontos finais do Azure Government, consulte o seguinte: https://docs.microsoft.com/en-us/azure/azure-government/documentation-government-developer-guide#endpoint-mapping
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
    - Problema corrigido https://github.com/Azure/azure-powershell/issues/4974
        - Fornecer o valor AUDIT_CHANGED_GROUP inválido para os cmdlets de auditoria já não lança um erro e vai ser removido numa futura versão.
    - Problema corrigido https://github.com/Azure/azure-powershell/issues/5046
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
* NOTA: Esta é uma versão de quebra de código. Veja o guia de migração (https://aka.ms/azps-migration-guide) para obter uma lista completa das quebras de código apresentadas.
* Todos os cmdlets no AzureRM suportam agora ajuda online
    - Execute Get-Help com o parâmetro -Online para abrir a ajuda online no seu browser da Internet predefinido
* AnalysisServices
    * Comando Synchronize-AzureAsInstance corrigido para funcionar com a nova API REST AsAzure para sincronização
* ApiManagement
    * Veja o guia de migração de quebras de código realizadas no ApiManagement nesta versão
    * Cmdlet Get-AzureRmApiManagementUser atualizado para corrigir problema https://github.com/Azure/azure-powershell/issues/4510
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
