---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.openlocfilehash: bee24af99da4b36e89cff9852c77214e2e09a542
ms.sourcegitcommit: 6a91b4c545350d316d3cf8c62f384478e3f3ba24
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/21/2020
ms.locfileid: "81740546"
---
## <a name="380---april-2020"></a>3.8.0 - Abril de 2020
#### <a name="azaccounts"></a>Az.Accounts
* Atualização do URL de inquérito do Azure PowerShell em "Resolve-AzError" [#11507]

#### <a name="azapimanagement"></a>Az.ApiManagement
* Adicionado aviso de alteração interruptiva para a alteração de resultados de cmdlets de Ficheiro do Azure numa versão futura
* Documentação atualizada de "Set-AzApiManagementGroup" para especificar o parâmetro GroupId

#### <a name="azcdn"></a>Az.Cdn
* Correção da apresentação do SKU de preços relacionados com ChinaCDN

#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* Suporte para Identidade, Encriptação, UserOwnedStorage 

#### <a name="azcompute"></a>Az.Compute
* Adicionado o cmdlet "Set-AzVmssOrchestrationServiceState".
* "Get-AzVmss" com -InstanceView mostra os estados de OrchestrationService.

#### <a name="aziothub"></a>Az.IotHub
* Gestão da configuração do dispositivo duplo de IoT. Os novos cmdlets são:
    - "Get-AzIotHubDeviceTwin"
    - "Update-AzIotHubDeviceTwin"
* Adicionado cmdlet para invocar o método direto num dispositivo num hub IoT.
* Gestão da configuração do módulo duplo do dispositivo de IoT. Os novos cmdlets são:
    - "Get-AzIotHubModuleTwin"
    - "Update-AzIotHubModuleTwin"
* Gestão da configuração da gestão automática de dispositivos IoT em escala. Os novos cmdlets são:
    - "Add-AzIotHubConfiguration"
    - "Get-AzIotHubConfiguration"
    - "Remove-AzIotHubConfiguration"
    - "Set-AzIotHubConfiguration"
* Adicionado cmdlet para invocar um método de módulo de periferia num Hub IoT.

#### <a name="azkeyvault"></a>Az.KeyVault
* Adicionado um novo cmdlet "Update-AzKeyVault" que pode permitir a eliminação recuperável e a proteção contra remoções num cofre
* Adicionado suporte para Microsoft.PowerShell.SecretManagement [#11178]
* Correção do erro nos exemplos de "Remove-AzKeyVaultManagedStorageSasDefinition" [#11479]
* Adicionado suporte para o ponto final privado

#### <a name="azmaintenance"></a>Az.Maintenance
* Publicação da versão de lançamento dos cmdlets de Manutenção para Disponibilidade Geral

#### <a name="azmonitor"></a>Az.Monitor
* Adicionados cmdlets para o âmbito de ligação privada
    - "Get-AzInsightsPrivateLinkScope"
    - "Remove-AzInsightsPrivateLinkScope"
    - "New-AzInsightsPrivateLinkScope"
    - "Update-AzInsightsPrivateLinkScope"
    - "Get-AzInsightsPrivateLinkScopedResource"
    - "New-AzInsightsPrivateLinkScopedResource"
    - "Remove-AzInsightsPrivateLinkScopedResource"

#### <a name="aznetwork"></a>Az.Network
* Atualização dos cmdlets para permitir a ligação num IP privado para o Gateway de Rede Virtual.
    - "New-AzVirtualNetworkGateway"
    - "Set-AzVirtualNetworkGateway"
    - "New-AzVirtualNetworkGatewayConnection"
    - "Set-AzVirtualNetworkGatewayConnection"
* Atualização dos cmdlets para permitir LocalNetworkGateways e VpnSites com base em FQDN
    - "New-AzLocalNetworkGateway"
    - "New-AzVpnSiteLink"
* Adicionado suporte para a família de endereços IPv6 em ExpressRouteCircuitConnectionConfig (Alcance Global)
    - Adicionado "Set-AzExpressRouteCircuitConnectionConfig"
        - permite a definição de todas as propriedades existentes, incluindo o IPv6CircuitConnectionProperties
    - Atualização de "Add-AzExpressRouteCircuitConnectionConfig"
        - Adicionado outro parâmetro opcional AddressPrefixType para especificar a família de endereços do prefixo de endereço
* Atualização dos cmdlets para permitir a definição do Tempo Limite de DPD nas Ligações do Gateway de Rede Virtual.
    - New-AzVirtualNetworkGatewayConnection
    - Set-AzVirtualNetworkGatewayConnection

#### <a name="azpolicyinsights"></a>Az.PolicyInsights
* Adicionado o cmdlet "Start-AzPolicyComplianceScan" para acionar análises de conformidade de políticas
* Adição de definição de políticas, definição de conjuntos e versões de atribuição ao resultado de "Get-AzPolicyState"

#### <a name="azservicefabric"></a>Az.ServiceFabric
* Melhorias da formatação e usabilidade do código dos exemplos de "New-AzServiceFabricCluster"

#### <a name="azsql"></a>Az.Sql
* Adicionados os cmdlets "Get-AzSqlInstanceOperation" e "Stop-AzSqlInstanceOperation"
* Suporte de auditorias a uma conta de armazenamento numa VNet.

#### <a name="azstorage"></a>Az.Storage
* Adicionado aviso de alteração interruptiva para a alteração de resultados de cmdlets de Ficheiro do Azure numa versão futura
* Suportado novo SkuName StandardGZRS, StandardRAGZRS ao criar/atualizar a Conta de armazenamento
    - "New-AzStorageAccount"
    - "Set-AzStorageAccount"
* Suportado o DataLake Gen2 
    - "New-AzDataLakeGen2Item"
    - "Get-AzDataLakeGen2Item"
    - "Get-AzDataLakeGen2ChildItem"
    - "Move-AzDataLakeGen2Item"
    - "Set-AzDataLakeGen2ItemAclObject"
    - "Update-AzDataLakeGen2Item"
    - "Get-AzDataLakeGen2ItemContent"
    - "Remove-AzDataLakeGen2Item"

# <a name="azure-powershell-release-notes"></a>Notas de versão do Azure PowerShell
## <a name="370---march-2020"></a>3.7.0 - Março de 2020
#### <a name="azaccounts"></a>Az.Accounts
* Foram corrigidos os parâmetros "Get-AzTenant"/"Get-AzDefault"/"Set-AzDefault" que emitiam uma NullReferenceException quando a sessão não estava iniciada [#10292]

#### <a name="azcompute"></a>Az.Compute
* Foram adicionados os seguintes parâmetros ao cmdlet "New-AzDiskConfig": 
    - DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference
* A propriedade Encryption foi permitida para o parâmetro Target do cmdlet "New-AzGalleryImageVersion".
* Foi corrigido o problema de tempDisk para os cmdlets "Set-AzVmss" -Reimage e "Invoke-AzVMReimage". [#11354]
* Foi adicionado suporte aos cmdlets abaixo para a nova Extensão SAP
    - "Set-AzVMAEMExtension"
    - "Get-AzVMAEMExtension"
    - "Remove-AzVMAEMExtension"
    - "Update-AzVMAEMExtension"
* Foram corrigidos os erros em exemplos do documento de ajuda
* É apresentado o valor de cadeia exato para o PowerState da VM no formato de tabela.
* "New-AzVmssConfig": foi corrigida a serialização da propriedade AutomaticRepairs quando a opção SinglePlacementGroup está desativada. [#11257]

#### <a name="azdatafactory"></a>Az.DataFactory
* Atualização da versão do SDK .Net do ADF para 4.8.0
* Foram adicionados parâmetros opcionais ao comando "Invoke-AzDataFactoryV2Pipeline" para suportar uma nova execução

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* Foi adicionada a descrição da alteração interruptiva para "Export-AzDataLakeStoreItem" e "Import-AzDataLakeStoreItem"
* Foi adicionada a opção de codificação de bytes para "New-AzDataLakeStoreItem", "Add-AzDAtaLakeStoreItemContent" e "Get-AzDAtaLakeStoreItemContent"

#### <a name="azhdinsight"></a>Az.HDInsight
* É suportada a versão de TLS mínima suportada ao criar o cluster.

#### <a name="aziothub"></a>Az.IotHub
* Foi adicionado suporte para gerir as definições distribuídas por dispositivo. Os novos cmdlets são:
    - "Get-AzIotHubDistributedTracing"
    - "Set-AzIotHubDistributedTracing"

#### <a name="azkeyvault"></a>Az.KeyVault
* Foram adicionados os atributos da alteração interruptiva a "New-AzKeyVault"

#### <a name="azmonitor"></a>Az.Monitor
* Foi atualizada a documentação de "New-AzScheduledQueryRuleLogMetricTrigger"

#### <a name="aznetwork"></a>Az.Network
* Foram atualizados os cmdlets para permitir VirtualHubVnetConnections entre inquilinos
    - "New-AzVirtualHubVnetConnection"
    - "Update-AzVirtualHubVnetConnection"
    - "New-AzVirtualHub"
    - "Update-AzVirtualHub"
* Foi removida a dependência do SDK do SQL Management

#### <a name="azpolicyinsights"></a>Az.PolicyInsights
* Mensagens de erro melhoradas

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* O Azure Site Recovery adicionou suporte para nova proteção e atualização das propriedades de VM para Máquinas Virtuais encriptadas em disco do Azure.
* Foi adicionada monitorização DR das propriedades VmwareToAzure ao Azure Site Recovery
* O Azure Backup adicionou suporte para repetir a atualização de políticas para itens falhados.
* O Azure Backup adicionou suporte para definições de exclusão do disco durante a cópia de segurança e o restauro.
* O Azure Backup adicionou suporte para restaurar vários ficheiros/pastas no AzureFileShare
* O Azure Backup adicionou suporte para o Resourcegroup especificado pelo utilizador durante a atualização da Política IaasVM

#### <a name="azresources"></a>Az.Resources
* Foi corrigido o parâmetro "Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType" para utilizar a apiVersion real dos recursos em vez da apiVersion predefinida [#11267]
* Foi adicionado o registo de correlationId para cenários de erro
* Pequena alteração à documentação referente a "Get-AzResourceLock". Exemplo adicionado.
* Aspas com caráter de escape no valor de parâmetro "Get-AzADUser" [#11317]
* Foram adicionados novos cmdlets aos Scripts de Implementação ("Get-AzDeploymentScript", "Get-AzDeploymentScriptLog", "Save-AzDeploymentScriptLog", "Remove-AzDeploymentScript")

#### <a name="azsql"></a>Az.Sql
* Foi adicionado um parâmetro secundário legível a "Invoke-AzSqlDatabaseFailover"
* Foi adicionado o cmdlet "Disable-AzSqlServerActiveDirectoryOnlyAuthentication"
* Classificação de sensibilidade guardada ao classificar as colunas na base de dados.

#### <a name="azsupport"></a>Az.Support
* Disponibilidade geral do módulo "Az.Support"

#### <a name="azwebsites"></a>Az.Websites
* Foi adicionado suporte para utilizar Regras de Encaminhamento de Tráfego webapp através dos novos cmdlets abaixo
    - "Get-AzWebAppTrafficRouting"
    - "Update-AzWebAppTrafficRouting"
    - "Add-AzWebAppTrafficRouting"
    - "Remove-AzWebAppTrafficRouting"

## <a name="361---march-2020"></a>3.6.1 - Março de 2020
#### <a name="azaccounts"></a>Az.Accounts
* Abrir a página de inquérito do Azure PowerShell em "Send-Feedback" [#11020]
* Apresentar o URL de inquérito do Azure PowerShell em "Resolve-Error" [#11021]
* Adicionada versão de Az em UserAgent

#### <a name="azapimanagement"></a>Az.ApiManagement
* Adicionado suporte para a obtenção e configuração do Domínio Personalizado no Ponto Final do DeveloperPortal [#11007]
* "Export-AzApiManagementApi" Adicionado suporte para a transferência da definição da API no formato JSON [#9987]
* "Import-AzApiManagementApi" Adicionado suporte para a importação da definição de OpenApi 3.0 a partir de documento JSON
* "New-AzApiManagementIdentityProvider" e "Set-AzApiManagementIdentityProvider" Adicionado suporte para a configuração de "Inquilino de Início de Sessão" para Fornecedor de AAD B2C [#9784]

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* Adicionada referência a System.Buffers explicitamente em csproj e psd1.

#### <a name="aziothub"></a>Az.IotHub
* Suporte adicionado para gerir dispositivos num Hub IoT. Os novos cmdlets são:
    - "Add-AzIotHubDevice"
    - "Get-AzIotHubDevice"
    - "Remove-AzIotHubDevice"
    - "Set-AzIotHubDevice"
* Adicionado suporte para a gestão de módulos num dispositivo IoT de destino num Hub IoT. Os novos cmdlets são:
    - "Add-AzIotHubModule"
    - "Get-AzIotHubModule"
    - "Remove-AzIotHubModule"
    - "Set-AzIotHubModule"
* Adicionado cmdlet para obter a cadeia de ligação de um dispositivo IoT de destino num Hub IoT.
* Adicionado cmdlet para obter a cadeia de ligação de um módulo num dispositivo IoT de destino num Hub IoT.
* Adicionado suporte para obter/definir dispositivo principal de um dispositivo IoT. Os novos cmdlets são:
    - "Get-AzIotHubDeviceParent"
    - "Set-AzIotHubDeviceParent"
* Adicionado suporte para gerir relações principal-subordinado de um dispositivo.

#### <a name="azmonitor"></a>Az.Monitor
* Corrigido o valor de saída de "Get-AzMetricDefinition" [#9714]

#### <a name="aznetwork"></a>Az.Network
* Sdk Sql Management atualizado.
* Corrigido um problema de diferença de nomes na classe PrivateLinkServiceConnectionState.
    - Mapeamento do campo ActionsRequired para ActionRequired.
* Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"

#### <a name="azresources"></a>Az.Resources
* Correção para erro de referência nula em "Get-AzRoleAssignment"
* Comutadores "-Force" e "-PassThru" marcados como opcionais em "Remove-AzADGroup" [#10849]
* Corrigido problema em que "MailNickname" não devolve "Remove-AzADGroup" [#11167]
* Corrigido problema em que a operação de pipe "Remove-AzADGroup" não funciona [#11171]
* Correção para erro de referência nula em GetAzureRoleAssignmentCommand
* Adicionados atributos de alterações interruptivas para futuras alterações a cmdlets de política
* "Get-AzResourceGroup" atualizado para realizar filtragem de etiqueta de grupo de recursos no lado do servidor
* Cmdlets Tag alargados para accept -ResourceId
    - Get-AzTag -ResourceId
    - New-AzTag -ResourceId
    - Remove-AzTag -ResourceId
* Adicionado cmdlet Tag novo
    - Update-AzTag -ResourceId
* ScopedDeployment trazido de SDK 3.3.0

#### <a name="azsql"></a>Az.Sql
* Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"
* Adicionado suporte para configuração de cópia de segurança de Retenção de Longo Prazo para Bases de Dados Geridas
    - Política Get/Set numa base de dados gerida
    - Obter cópia(s) de segurança LTR por base de dados gerida, por instância gerida ou por localização
    - Remover uma cópia de segurança LTR
    - Restaurar uma cópia de segurança LTR para criar uma base de dados gerida nova
* Adicionado MinimalTlsVersion a New-AzSqlServer e Set-AzSqlServer
* Adicionado MinimalTlsVersion a New-AzSqlInstance e Set-AzSqlInstance
* Versão de SDK SQL atualizada para Az.Network

#### <a name="azstorage"></a>Az.Storage
* AllowProtectedAppendWrite suportada em ImmutabilityPolicy
    - "Set-AzRmStorageContainerImmutabilityPolicy"
* Adicionada uma mensagem de aviso de alteração interruptiva para alteração do tipo AzureStorageTable numa futura versão
    - "New-AzStorageTable"
    - "Get-AzStorageTable"

#### <a name="azwebsites"></a>Az.Websites
* Adicionado o parâmetro Tag para "New-AzAppServicePlan" e "Set-AzAppServicePlan"
* Paragem da execução de cmdlet caso seja emitida uma exceção ao adicionar um domínio personalizado a um site
* Adicionado suporte para a realização de operações para Serviços de Aplicações em grupos de recursos diferentes do Plano do Serviço de Aplicações
* Aplicada restrição de acesso a WebApp/Função em diferentes grupos de recursos
* Corrigido problema para definir os nomes de anfitrião personalizados para WebAppSlots

## <a name="350---february-2020"></a>3.5.0 - Fevereiro de 2020
### <a name="highlights-since-the-last-major-release"></a>Destaques desde a última versão principal
* Telemetria do lado do cliente atualizada.
* O Az.IotHub adicionou cmdlets para suportar a gestão de dispositivos.
* O Az.SqlVirtualMachine adicionou cmdlets ao Serviço de Escuta do Grupo de Disponibilidade.

#### <a name="azaccounts"></a>Az.Accounts
* SubscriptionId, TenantId e tempo de execução adicionados aos dados de telemetria do lado do cliente

#### <a name="azautomation"></a>Az.Automation
* Foi corrigido o erro no Exemplo 1 na documentação de referência de "New-AzAutomationSoftwareUpdateConfiguration"

#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* SDK atualizado para a versão 7.0
* Mensagem de erro melhorada quando o servidor responde ao corpo vazio

#### <a name="azcompute"></a>Az.Compute
* Valor vazio permitido para ProximityPlacementGroupId durante a atualização

#### <a name="azfrontdoor"></a>Az.FrontDoor
* Cmdlet adicionado para obter definições de regras geridas que podem ser utilizadas na WAF

#### <a name="aziothub"></a>Az.IotHub
* Suporte adicionado para gerir dispositivos num Hub IoT. Os novos cmdlets são:
    - "Add-AzIotHubDevice"
    - "Get-AzIotHubDevice"
    - "Remove-AzIotHubDevice"
    - "Set-AzIotHubDevice"

#### <a name="azkeyvault"></a>Az.KeyVault
* Texto duplicado fixo para Add-AzKeyVaultKey.md

#### <a name="azmonitor"></a>Az.Monitor
* Descrição fixa do cmdlet Get-AzLog.
* Foi adicionado um novo parâmetro chamado ActionGroupId ao comando "New-AzMetricAlertRuleV2".
    - O utilizador pode fornecer ActionGroupId(string) ou ActionGorup(ActivityLogAlertActionGroup).

#### <a name="aznetwork"></a>Az.Network
* Foi adicionada uma nota de parâmetro adicional para o parâmetro "-EnableProxyProtocol" para o cmdlet "New-AzPrivateLinkService".
* Exemplo de FilterData fixo em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.
* Exemplo de Captura de Pacotes adicionado para capturar todos os pacotes internos e externos em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.
* Política do Azure Firewall suportada em firewalls VNet
    - Não foram adicionados novos cmdlets. Simplificação da restrição da política de firewall em firewalls VNet

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* Suporte adicionado da funcionalidade Restaurar como ficheiros para Bases de Dados SQL.

#### <a name="azresources"></a>Az.Resources
* Cmdlets de implementação de modelos refatorizados
    - Foram adicionados novos cmdlets para gerir implementações no grupo de gestão: *-AzManagementGroupDeployment
    - Foram adicionados novos cmdlets para gerir implementações no inquilino: *-AzTenantDeployment
    - Cmdlets *-AzDeployment refatorizados para trabalhar especificamente no âmbito da subscrição
    - Foram criados aliases *-AzSubscriptionDeployment para os cmdlets *-AzDeployment
* "Update-AzADApplication" fixo quando o parâmetro "AvailableToOtherTenants" não está definido
* ApplicationObjectWithoutCredentialParameterSet removido para evitar AmbiguousParameterSetException.
* Ficheiros de ajuda regenerados

#### <a name="azsql"></a>Az.Sql
* Suporte adicionado para restauro para um ponto anterior no tempo entre subscrições nas Instâncias Geridas.
* Suporte adicionado para alterar a geração de hardware das Instâncias Geridas de SQL existentes
* Exemplos de ajuda "Update-AzSqlServerVulnerabilityAssessmentSetting" fixos: saída do parâmetro/propriedade - EmailAdmins

#### <a name="azsqlvirtualmachine"></a>Az.SqlVirtualMachine
* Cmdlets adicionados para o Serviço de Escuta do Grupo de Disponibilidade

#### <a name="azstoragesync"></a>Az.StorageSync
* Conjuntos de carateres suportados atualizados em "Invoke-AzStorageSyncCompatibilityCheck".

## <a name="340---february-2020"></a>3.4.0 - Fevereiro de 2020
### <a name="highlights-since-the-last-major-release"></a>Destaques desde a última versão principal
* Versão inicial Az.CosmosDB 0.1.0 lançada
* Foi adicionado suporte para Az.Network ConnectionMonitor V2

#### <a name="azaccounts"></a>Az.Accounts
* Foi desativada a gravação automática de contexto quando AzureRmContext.json não está disponível
* Atualização da referência ao Azure Powershell Common para a pré-visualização 1.3.5

#### <a name="azapimanagement"></a>Az.ApiManagement
* **Get-AzApiManagementApiSchema** Foi corrigido ao obter Open-Api Schema associado a uma API   https://github.com/Azure/azure-powershell/issues/10626
* **New-AzApiManagementProduct*** e **Set-AzApiManagementProduct**
  - Foi corrigida a documentação para https://github.com/Azure/azure-powershell/issues/10472
* **Set-AzApiManagementApi** Exemplo adicionado para mostrar como atualizar o ServiceUrl com o cmdlet

#### <a name="azcompute"></a>Az.Compute
* Foi limitado o número de estados de VM a 100 para evitar limitações quando Get-AzVM-Status é executado sem o nome da VM.
* Foi adicionado o cmdlet Update-AzDiskEncryptionSet
* Foram adicionados os parâmetros EncryptionType e DiskEncryptionSetId aos seguintes cmdlets:
    - New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig
* Foi adicionado o parâmetro ColocationStatus ao cmdlet Get-AzProximityPlacementGroup.

#### <a name="azdatafactory"></a>Az.DataFactory
* Atualização do SDK .NET do ADF para a versão 4.7.0

#### <a name="azdeploymentmanager"></a>Az.DeploymentManager
* Adiciona operações LIST para os recursos
* Adiciona a capacidade de realizar operações nos passos de Verificação de Estado de Funcionamento

#### <a name="azhdinsight"></a>Az.HDInsight
* Foi corrigido o erro do documento de New-AzHDInsightCluster.

#### <a name="azkeyvault"></a>Az.KeyVault
* Foi adicionado o alias do Nome ao atributo VaultName para tornar Remove-AzureKeyVault consistente com New-AzureKeyVault.

#### <a name="aznetwork"></a>Az.Network
* Foi adicionado um novo exemplo a Set-AzNetworkWatcherConfigFlowLog.md para demonstrar o cenário de desativação da Análise de Tráfego.
* Foi adicionado suporte para atribuir a configuração IP de gestão ao Azure Firewall, uma sub-rede dedicada e IP Público que a firewall utilizará no tráfego de gestão
    - cmdlet New-AzFirewall atualizado:
        - Foi adicionado o parâmetro -ManagementPublicIpAddress (não obrigatório) que aceita um objeto de Endereço IP Público
        - Foi adicionado o método SetManagementIpConfiguration no objeto de firewall. Requer uma sub-rede e um endereço IP Público como entrada. O nome da sub-rede tem de ser "AzureFirewallManagementSubnet"
* Foram corrigidos os exemplos de Get-AzNetworkSecurityGroup para mostrar exemplos de NSGs em vez de interfaces de rede.
* Foi corrigido um erro no comando New-AzVpnSite que estava a impedir o ID do recurso de concluir um parâmetro.
* Foi adicionado suporte para a Configuração do URL em Reescrever Conjunto de Ações de Regras no Gateway de Aplicação
    - Foram adicionados novos cmdlets:
        - New-AzApplicationGatewayRewriteRuleUrlConfiguration
    - Foram atualizados cmdlets com o parâmetro opcional - UrlConfiguration
        - New-AzApplicationGatewayRewriteRuleActionSet
* Foi adicionado suporte para os recursos do NetworkWatcher ConnectionMonitor versão 2

#### <a name="azpolicyinsights"></a>Az.PolicyInsights
* Foi adicionado suporte para avaliar a conformidade antes de determinar o recurso a remediar
    - Foi adicionado o parâmetro "-ResourceDiscoverMode" a Start-AzPolicyRemediation
* Foi adicionado o cmdlet Get-AzPolicyMetadata para obter os recursos de metadados da política
* Get-AzPolicyState e Get-AzPolicyStateSummary atualizados para a versão da API 2019-10-01

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* Foi adicionado suporte do Azure Site Recovery para remover um disco replicado.
* O Azure Backup adicionou suporte para adicionar etiquetas ao criar um Cofre dos Serviços de Recuperação.

#### <a name="azresources"></a>Az.Resources
* -Scope foi tornado opcional nos cmdlets *-AzPolicyAssignment com subscrição de contexto predefinida
* Foram adicionados exemplos de criação de ADServicePrincipal com credenciais de palavras-passe e chaves

#### <a name="azsql"></a>Az.Sql
Foi corrigido o cmdlet New-AzSqlDatabaseSecondary para verificar a existência de PartnerDatabaseName em vez da existência de DatabaseName.

#### <a name="azstorage"></a>Az.Storage
* Foi definido o suporte de Tipo de Chave de Encriptação na Tabela/Fila em Criar Conta de Armazenamento
    - New-AzStorageAccount
* Será apresentado RequestId quando StorageException não tiver ExtendedErrorInformation
* Foi corrigido o exemplo 6 do cmdlet Start-AzStorageBlobCopy

#### <a name="azwebsites"></a>Az.Websites
* Set-AzWebapp e Set-AzWebappSlot suportam as propriedades AlwaysOn, MinTls e FtpsState
* Foi corrigido o problema em que a definição de HttpsOnly, juntamente com a alteração de AppservicePlan ao utilizar o único comando Set-AzWebApp, estava a repor HttpsOnly para o valor predefinido

## <a name="330---january-2020"></a>3.3.0 – janeiro de 2020
#### <a name="azaccounts"></a>Az.Accounts
* Add-AzEnvironment e Set-AzEnvironment foram atualizados para aceitar os parâmetros AzureAttestationServiceEndpointResourceId e AzureAttestationServiceEndpointSuffix

#### <a name="azcdn"></a>Az.Cdn
* Apresentação dos detalhes da resposta de erro no cmdlet New-AzCdnEndpoint

#### <a name="azcompute"></a>Az.Compute
* Correção do cmdlet Set-AzVMCustomScriptExtension para uma VM com disco OD gerido sem perfil de SO.

#### <a name="azcontainerinstance"></a>Az.ContainerInstance
* Foram corrigidos os nomes de parâmetros utilizados pelo exemplo de New-AzContainerGroup

#### <a name="azdataboxedge"></a>Az.DataBoxEdge
* Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageContainer"
  - Obter o Contentor de Armazenamento Edge
* Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageContainer"
  - Criar novo Contentor de Armazenamento Edge
* Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageContainer"
  - Remover o Contentor de Armazenamento Edge
* Foi adicionado o cmdlet "Invoke-AzDataBoxEdgeStorageContainer"
  - Invocar ação para atualizar os dados no Contentor de Armazenamento Edge
* Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageAccount"
  - Obter a Conta de Armazenamento Edge
* Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageAccount"
  - Criar nova Conta de Armazenamento Edge
* Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageAccount"
  - Remover a Conta de Armazenamento Edge
* Invocar o cmdlet "Invoke-AzDataBoxEdgeShare"
  - Invocar ação para atualizar os dados na partilha
* Foi adicionado o cmdlet "Set-AzDataBoxEdgeStorageAccountCredential"
  - Definição de AzDataBoxEdgeStorageAccountCredential

#### <a name="azdatafactory"></a>Az.DataFactory
* Adição das propriedades AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId e VersionStatus para o cmd Get-AzDataFactoryV2IntegrationRuntime
* Atualização do SDK .NET do ADF para a versão 4.6.0
* Adição do parâmetro "PublicIPs" para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a criação de Azure-SSIS IR com endereços IP públicos estáticos.

#### <a name="azdevtestlabs"></a>Az.DevTestLabs
* Remoção da ligação quebrada em Get-AzDtlAllowedVMSizesPolicy.md

#### <a name="azeventhub"></a>Az.EventHub
* Correção do problema 10634: Correção da referência de objeto nulo para remover eventhubnamespace

#### <a name="azhdinsight"></a>Az.HDInsight
* Correção do erro Invoke-AzHDInsightHiveJob.md.

#### <a name="azmachinelearning"></a>Az.MachineLearning
* Foram removidos os cmdlets abaixo porque MachineLearningCompute já não está disponível
  - Get-AzMlOpCluster
  - Get-AzMlOpClusterKey
  - New-AzMlOpCluster
  - Remove-AzMlOpCluster
  - Set-AzMlOpCluster
  - Test-AzMlOpClusterSystemServicesUpdateAvailability
  - Update-AzMlOpClusterSystemService

#### <a name="aznetwork"></a>Az.Network
* Atualização da dependência de Microsoft.Azure.Management.SQL da versão 1.36-preview para 1.37-preview

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* Alteração do Azure Site Recovery para suportar VMs de disco gerido com encriptação inativa com chaves geridas pelo cliente para o fornecedor do Azure.
* Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional para ativar a proteção de VMware para o Azure.
* Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional ao nível do disco para ativar a proteção de VMware para o Azure.
* Suporte do Azure Site Recovery para atualizar o item protegido por replicação com encriptação de discos e definir o mapa para HyperV para o Azure.

#### <a name="azresources"></a>Az.Resources
* Correção de um erro no documento de ajuda de "Remove-AzTag".

#### <a name="azsql"></a>Az.Sql
* Correção da funcionalidade dos cmdlets de linha de base do conjunto de avaliação de vulnerabilidades para funcionar na base de dados mestre da base de dados do Azure e limitá-la nas bases de dados do sistema de instância gerida
* Correção de um erro ao criar o grupo de ativação pós-falha de instância SQL

#### <a name="azsqlvirtualmachine"></a>Az.SqlVirtualMachine
* Adição de DR como um novo tipo de Licença válido

#### <a name="azstorage"></a>Az.Storage
* Adição de uma mensagem de aviso de alteração interruptiva para alteração do valor de DefaultAction numa futura versão
    - Update-AzStorageAccountNetworkRuleSet
* Suporte para obter a hora da última sincronização da conta de armazenamento ao executar get-AzureRMStorageAccount com o parâmetro -IncludeGeoReplicationStats
    - Get-AzureRMStorageAccount

## <a name="320---december-2019"></a>3.2.0 - Dezembro de 2019

### <a name="general"></a>Geral
* Atualização das referências em .psd1 para utilizar o caminho relativo para todos os módulos

#### <a name="azaccounts"></a>Az.Accounts
* Definição do UserAgent correto para telemetria do lado do cliente para a pré-visualização do Az 4.0
* Apresentação de mensagem de erro amigável de utilizador quando o contexto é nulo na pré-visualização do Az 4.0

#### <a name="azbatch"></a>Az.Batch
* Correção do problema [10602](https://github.com/Azure/azure-powershell/issues/10602), em que **New-AzBatchPool** não enviava corretamente "VirtualMachineConfiguration.ContainerConfiguration" ou "VirtualMachineConfiguration.DataDisks" para o servidor.

#### <a name="azdatafactory"></a>Az.DataFactory
* Atualização do SDK .NET do ADF para a versão 4.5.0

#### <a name="azfrontdoor"></a>Az.FrontDoor
* Adição do suporte de exclusão de regras geridas pela WAF
* Adição de SocketAddr ao preenchimento automático

#### <a name="azhealthcareapis"></a>Az.HealthcareApis
* Processamento de Exceções

#### <a name="azkeyvault"></a>Az.KeyVault
* Correção do erro em que era acedido um valor potencialmente não definido
* Gestão de Certificados de Criptografia de Curva Elíptica
    - Adicionado suporte para especificar a Curva das Políticas de Certificado

#### <a name="azmonitor"></a>Az.Monitor
* Adição de um argumento opcional ao comando Adicionar Definições de Diagnóstico. Um argumento de opção que, se estiver presente, indica que a exportação para o Log Analytics deve ser feita para um esquema fixo (também conhecido como tipo de dados dedicado)

#### <a name="aznetwork"></a>Az.Network
* Suporte para IpGroups na aplicação AzureFirewall, Nat e Regras de Rede.

#### <a name="azresources"></a>Az.Resources
* Correção de um problema em que a implementação do modelo não consegue ler um parâmetro se o nome estiver em conflito com um nome de parâmetro incorporado.
* Os cmdlets da política foram atualizados para utilizar a nova versão de API 2019-09-01 que introduz suporte de agrupamento nas definições do conjunto de políticas.

#### <a name="azsql"></a>Az.Sql
* Criação do armazenamento atualizada na ativação automática da Avaliação de Vulnerabilidades para StorageV2

#### <a name="azstorage"></a>Az.Storage
* Suporte para gerar um token de SAS baseado na Identidade do Blob/Contentor com Contexto de Armazenamento baseado na autenticação OAuth
    - New-AzStorageContainerSASToken
    - New-AzStorageBlobSASToken
* Suporte para revogar as Chaves de Delegação do Utilizador da Conta de Armazenamento, pelo que todos os tokens de SAS da identidade são revogados
    - Revoke-AzStorageAccountUserDelegationKeys
* Atualização de Microsoft.Azure.Management.Storage 14.2.0 para suportar a nova versão de API 2019-06-01.
* Suporte de QuotaGiB (Quota de Partilha em Gibibye) para obter valores superiores a 5120 no plano de Gestão de cmdlets de Partilha de Ficheiros e foi adicionado o alias do parâmetro "Quota" ao parâmetro "QuotaGiB".
    - New-AzRmStorageShare
    - Update-AzRmStorageShare
* Adição do alias do parâmetro "QuotaGiB" ao parâmetro "Quota"
    - Set-AzStorageShareQuota
* Correção do problema em que Set-AzStorageContainerAcl consegue limpar a Política de Acesso armazenada
    - Set-AzStorageContainerAcl

## <a name="310---november-2019"></a>3.1.0 - Novembro de 2019
### <a name="highlights-since-the-last-major-release"></a>Destaques desde a última versão principal
* Az.DataBoxEdge 1.0.0 já disponível
* Az.SqlVirtualMachine 1.0.0 já disponível

#### <a name="azcompute"></a>Az.Compute
* Funcionalidade de Reaplicação da VM
    - Adição do parâmetro Reapply ao cmdlet Set-AzVM
* Funcionalidade AutomaticRepairs do Conjunto de Dimensionamento de VM:
    - Adição dos parâmetros EnableAutomaticRepair, AutomaticRepairGracePeriod e AutomaticRepairMaxInstanceRepairsPercent aos seguintes cmdlets:   New-AzVmssConfig   Update-AzVmss
* Suporte para imagens de galeria entre inquilinos para New-AzVM
* Adição de "Spot" ao preenchedor de argumentos do parâmetro Priority nos cmdlets New-AzVM, New-AzVMConfig e New-AzVmss
* Adição dos parâmetros DiskIOPSReadWrite e DiskMBpsReadWrite ao cmdlet Add-AzVmssDataDisk
* Alteração do parâmetro SourceImageId do cmdlet New-AzGalleryImageVersion para opcional
* Adição dos parâmetros OSDiskImage e DataDiskImage ao cmdlet New-AzGalleryImageVersion
* Adição do parâmetro HyperVGeneration ao cmdlet New-AzGalleryImageDefinition
* Adição dos parâmetros SkipExtensionsOnOverprovisionedVMs aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss

#### <a name="azdataboxedge"></a>Az.DataBoxEdge
* Adição do cmdlet `Get-AzDataBoxEdgeOrder`
    - Obter a Encomenda
* Adição do cmdlet `New-AzDataBoxEdgeOrder`
    - Criar nova Encomenda
* Adição do cmdlet `Remove-AzDataBoxEdgeOrder`
    - Remover a Encomenda
* Alteração no cmdlet `New-AzDataBoxEdgeShare`
    - Agora cria uma Partilha Local
* Adição do cmdlet `Set-AzDataBoxEdgeRole`
    - Agora, o IotRole pode ser mapeado para a Partilha
* Adição do cmdlet `Invoke-AzDataBoxEdgeDevice`
    - Invocar verificação da atualização, transferência da atualização, instalação das atualizações no dispositivo
* Adição do cmdlet `Get-AzDataBoxEdgeTrigger`
    - Obtém as informações sobre os Acionadores
* Adição do cmdlet `New-AzDataBoxEdgeTrigger`
    - Criar novos Acionadores
* Adição do cmdlet `Remove-AzDataBoxEdgeTrigger`
    - Remover os Acionadores

#### <a name="azdatafactory"></a>Az.DataFactory
* Atualização do SDK .NET do ADF para a versão 4.4.0
* Adição do parâmetro "ExpressCustomSetup" para o cmdlet "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir configurações e componentes de terceiros sem scripts de configuração personalizados.

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* Atualização da documentação de Get-AzDataLakeStoreDeletedItem e Restore-AzDataLakeStoreDeletedItem

#### <a name="azeventhub"></a>Az.EventHub
* Correção do problema 10301: Correção do formato de data do token de SAS

#### <a name="azfrontdoor"></a>Az.FrontDoor
* Adição do parâmetro MinimumTlsVersion a Enable-AzFrontDoorCustomDomainHttps e New-AzFrontDoorFrontendEndpointObject
* Adição dos parâmetros HealthProbeMethod e EnabledState a New-AzFrontDoorHealthProbeSettingObject
* Adição de um novo cmdlet para criar um objeto BackendPoolsSettings para passar para a criação/atualização do Front Door
    - New-AzFrontDoorBackendPoolsSettingObject

#### <a name="aznetwork"></a>Az.Network
* Alteração dos exemplos de opções FilterData de "Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" e "Start-AzVirtualnetworkGatewayPacketCapture.md".

#### <a name="azprivatedns"></a>Az.PrivateDns
* Atualização do SDK .NET do PrivateDns para a versão 1.0.0

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* Suporte do Azure Site Recovery para selecionar o tipo de disco ao ativar a proteção.
* Correção do Azure Site Recovery para a edição de ações do plano de recuperação.
* Suporte de Restauro de SQL do Azure Backup para aceitar BDs de filestream.

#### <a name="azrediscache"></a>Az.RedisCache
* Adição do parâmetro "MinimumTlsVersion" nos cmdlets "New-AzRedisCache" e "Set-AzRedisCache". Adição, também, de "MinimumTlsVersion" na saída do cmdlet "Get-AzRedisCache".
* Adição da validação no parâmetro "-Size" para os cmdlets "Set-AzRedisCache" e "New-AzRedisCache"

#### <a name="azresources"></a>Az.Resources
- Atualização dos cmdlets de política no sentido de utilizar a nova versão de api 2019-06-01, a qual tem a nova propriedade EnforcementMode na atribuição de política.
- Atualização do exemplo de ajuda da definição da política de criação
- Correção do erro Remove-AZADServicePrincipal -ServicePrincipalName. Apresentação de uma referência nula quando o nome do principal do serviço não é encontrado.
- Correção do erro New-AZADServicePrincipal. Apresentação de uma referência nula quando o inquilino não tem uma subscrição.
- Alteração de New-AzAdServicePrincipal para adicionar credenciais apenas a aplicações associadas.

#### <a name="azsql"></a>Az.Sql
* Adição de suporte para a base de dados ReadReplicaCount.
* Correção de Set-AzSqlDatabase quando a redundância de zona não está definida

## <a name="300---november-2019"></a>3.0.0 - Novembro de 2019
### <a name="general"></a>Geral
* Disponibilização do Az.PrivateDns 1.0.0

#### <a name="azaccounts"></a>Az.Accounts
* Adição de uma mensagem de descontinuação para o alias "Resolve-Error".

#### <a name="azadvisor"></a>Az.Advisor
* Adição da nova categoria "Excelência Operacional" ao cmdlet Get-AzAdvisorRecommendation.

#### <a name="azbatch"></a>Az.Batch
* Mudança de nome de `CoreQuota` em `BatchAccountContext` para `DedicatedCoreQuota`. Existe também um novo `LowPriorityCoreQuota`.
  - Isto afeta **Get-AzBatchAccount**.
* O parâmetro **New-AzBatchTask** `-ResourceFile` assume agora uma coleção de objetos `PSResourceFile`, os quais podem ser construídos com o novo cmdlet **New-AzBatchResourceFile**.
* Novo cmdlet **New-AzBatchResourceFile** para ajudar a criar objetos `PSResourceFile`. Estes podem ser fornecidos a **New-AzBatchTask** no parâmetro `-ResourceFile`.
  - Isto suporta dois novos tipos de ficheiro de recursos para além do caminho `HttpUrl` existente:
    - Os ficheiros de recursos baseados em `AutoStorageContainerName` transferem um contentor integral de armazenamento automático para o nó do Batch.
    - Os ficheiros de recursos baseados em `StorageContainerUrl` transferem o contentor especificado no URL para o nó do Batch.
* Remoção da propriedade `ApplicationPackages` de `PSApplication` devolvida por **Get-AzBatchApplication**.
  - Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com **Get-AzBatchApplicationPackage**. Por exemplo: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.
* Mudança de nome de `ApplicationId` para `ApplicationName` em **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication** e **Set-AzBatchApplication**.
  - `ApplicationId` é agora um alias de `ApplicationName`.
* Adição da nova propriedade `PSWindowsUserConfiguration` a `PSUserAccount`.
* Mudança de nome de `Version` para `Name` em `PSApplicationPackage`.
* Mudança de nome de `BlobSource` para `HttpUrl` em `PSResourceFile`.
* Remoção da propriedade `OSDisk` de `PSVirtualMachineConfiguration`.
* Remoção de **Set-AzBatchPoolOSVersion**. Esta operação deixou de ser suportada.
* Remoção de `TargetOSVersion` de `PSCloudServiceConfiguration`.
* Mudança de nome de `CurrentOSVersion` para `OSVersion` em `PSCloudServiceConfiguration`.
* Remoção de `DataEgressGiB` e `DataIngressGiB` de `PSPoolUsageMetrics`.
* Remoção de **Get-AzBatchNodeAgentSku** e substituição deste por **Get-AzBatchSupportedImage**.
  - **Get-AzBatchSupportedImage** devolve os mesmos dados de **Get-AzBatchNodeAgentSku**, mas num formato mais acessível.
  - As novas imagens não verificadas agora também são devolvidas. Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.
* Adição da capacidade de montagem de sistemas de ficheiros remotos em cada nó de um conjunto através do novo parâmetro `MountConfiguration` de **New-AzBatchPool**.
* Adição do suporte a regras de segurança de rede que bloqueiam o acesso de rede a um conjunto com base na porta de origem do tráfego. Isto ocorre através da propriedade `SourcePortRanges` em `PSNetworkSecurityGroupRule`.
* Ao executar um contentor, o Batch agora suporta a execução da tarefa no diretório de trabalho do contentor ou no diretório de trabalho da tarefa do Batch. Isto é controlado pela propriedade `WorkingDirectory` em `PSTaskContainerSettings`.
* Adição da capacidade de especificar uma coleção de IPs públicos em `PSNetworkConfiguration` através da nova propriedade `PublicIPs`. Isto garante que os nós no Conjunto terão um IP da lista de IPs fornecidos pelo utilizador.
* Quando não for especificado, o valor predefinido de `WaitForSuccess` em `PSSTartTask` é agora `$True` (era `$False`).
* Quando não for especificado, o valor predefinido de `Scope` em `PSAutoUserSpecification` é agora `Pool` (era `Task` no Windows e `Pool` no Linux).

#### <a name="azcdn"></a>Az.Cdn
* Introdução de UrlRewriteAction e CacheKeyQueryStringAction em RulesEngine.
* Correção de vários erros como a falta da Entrada "Seletor" no cmdlet New-AzDeliveryRuleCondition.

#### <a name="azcompute"></a>Az.Compute
* Funcionalidade Conjunto de Encriptação de Discos
    - Novos cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet
    - Adição do parâmetro DiskEncryptionSetId aos seguintes cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk
    - Adição dos parâmetros DiskEncryptionSetId e EncryptionType aos seguintes cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig
* Adição do parâmetro PublicIPAddressVersion a New-AzVmssIPConfig
* Movimentação de FileUris da extensão de script personalizado da definição pública para a definição protegida
* Adição de ScaleInPolicy aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss
* Alterações interruptivas
    - Utilização do parâmetro UploadSizeInBytes em vez de DiskSizeGB para New-AzDiskConfig quando CreateOption é Carregar
    - Substituição de PublishingProfile.Source.ManagedImage.Id por StorageProfile.Source.Id no objeto GalleryImageVersion

#### <a name="azdatafactory"></a>Az.DataFactory
* Atualização da versão do SDK .Net do ADF para 4.3.0

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* Atualização da versão do SDK ADLS (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) ) com as seguintes correções
* Evita a apresentação de uma exceção ao mesmo tempo que não consegue anular a serialização do creationtime do lixo ou da entrada de diretório.
* Expõe a definição por tempo limite do pedido em adlsclient
* Correção da passagem do syncflag original para a recuperação de badoffset
* Correção de EnumerateDirectory para obter o token de continuação após a verificação da resposta
* Correção do Erro de Concatenação

#### <a name="azfrontdoor"></a>Az.FrontDoor
* Correção de diversos erros de digitação em vários módulos

#### <a name="azhdinsight"></a>Az.HDInsight
* Correção do erro em que o cliente recebe o erro "Não é uma cadeia Base 64 válida" quando utiliza Get-AzHDInsightCluster para obter o cluster com o armazenamento ADLSGen1.
* Adição de um parâmetro com o nome "ApplicationId" a três cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig e New-AzHDInsightCluster para que o cliente consiga fornecer o ID da aplicação do principal de serviço que permite aceder ao Azure Data Lake.
* Alteração de Microsoft.Azure.Management.HDInsight da versão 2.1.0 para a 5.1.0
* Remoção de cinco cmdlets:
    - Get-AzHDInsightOMS
    - Enable-AzHDInsightOMS
    - Disable-AzHDInsightOMS
    - Grant-AzHDInsightRdpServicesAccess
    - Revoke-AzHDInsightRdpServicesAccess
* Adição de três cmdlets:
    - Get-AzHDInsightMonitoring para substituir Get-AzHDInsightOMS.
    - Enable-AzHDInsightMonitoring para substituir Enable-AzHDInsightOMS.
    - Disable-AzHDInsightMonitoring para substituir Disable-AzHDInsightOMS.
* Correção do cmdlet Get-AzHDInsightProperties para suportar a obtenção de informações sobre capacidades de uma localização específica.
* Remoção de conjuntos de parâmetros("Spark1", "Spark2") de Add-AzHDInsightConfigValue.
* Adição de exemplos aos documentos de ajuda do cmdlet Add-AzHDInsightSecurityProfile.
* Alteração do tipo de saída dos seguintes cmdlets:
*  - Alteração do tipo de saída de Get-AzHDInsightProperties de CapabilitiesResponse para AzureHDInsightCapabilities.
*  - Alteração do tipo de saída de Remove-AzHDInsightCluster de ClusterGetResponse para booleano.
*  - Alteração do tipo de saída de Set-AzHDInsightGatewaySettings de HttpConnectivitySettings para GatewaySettings.
* Adição de alguns casos de teste de cenários.
* Remoção de alguns alias: "Add-AzHDInsightConfigValues", "Get-AzHDInsightProperties".

#### <a name="aziothub"></a>Az.IotHub
* Alterações interruptivas:
    - O cmdlet "Add-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.
    - O conjunto de parâmetros "__AllParameterSets" do cmdlet "Add-AzIotHubEventHubConsumerGroup" foi removido.
    - O cmdlet "Get-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.
    - O conjunto de parâmetros "__AllParameterSets" do cmdlet "Get-AzIotHubEventHubConsumerGroup" foi removido.
    - A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties" foi removida.
    - A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties" foi removida.
    - O cmdlet "New-AzIotHubExportDevice" deixou de suportar o alias "New-AzIotHubExportDevices".
    - O cmdlet "New-AzIotHubImportDevice" deixou de suportar o alias "New-AzIotHubImportDevices".
    - O cmdlet "Remove-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.
    - O conjunto de parâmetros "__AllParameterSets" do cmdlet "Remove-AzIotHubEventHubConsumerGroup" foi removido.
    - O cmdlet "Set-AzIotHub" deixou de suportar o parâmetro "OperationsMonitoringProperties" e não foi encontrado qualquer alias para o nome de parâmetro original.
    - O conjunto de parâmetros "UpdateOperationsMonitoringProperties" do cmdlet "Set-AzIotHub" foi removido.

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* Suporte do Azure Site Recovery para configurar recursos de rede como NSG, IP público e balanceadores de carga internos do Azure para o Azure.
* Suporte do Azure Site Recovery para escrever para um disco gerido do VMware para o Azure.
* Suporte do Azure Site Recovery para redução de NIC do VMware para o Azure.
* Suporte do Azure Site Recovery para aceleração de rede do Azure para o Azure.
* Suporte do Azure Site Recovery para a atualização automática do agente do Azure para o Azure.
* Suporte do Azure Site Recovery para SSD Standard do Azure para o Azure.
* Suporte do Azure Site Recovery para a codificação em dois passos do Azure Disk Encryption do Azure para o Azure.
* Suporte do Azure Site Recovery para a proteção de um disco adicionado recentemente do Azure para o Azure.
* Adição da funcionalidade SoftDelete para VM e de testes para softdelete

#### <a name="azresources"></a>Az.Resources
* Atualização da assemblagem de dependências Microsoft.Extensions.Caching.Memory da versão 1.1.1 para a 2.2

#### <a name="aznetwork"></a>Az.Network
* Alteração de todos os cmdlets para PrivateEndpointConnection para suportar o fornecedor de serviços genérico.
    - Cmdlet atualizado:
        - Approve-AzPrivateEndpointConnection
        - Deny-AzPrivateEndpointConnection
        - Get-AzPrivateEndpointConnection
        - Remove-AzPrivateEndpointConnection
        - Set-AzPrivateEndpointConnection
* Adição de novo cmdlet para PrivateLinkResource também com suporte de fornecedor de serviços genérico.
    - Novo cmdlet:
        - Get-AzPrivateLinkResource
* Adição de novos campos e parâmetro para a funcionalidade Protocolo de Proxy V2.
    - Adição da propriedade EnableProxyProtocol em PrivateLinkService
    - Adição da propriedade LinkIdentifier em PrivateEndpointConnection
    - Atualização de New-AzPrivateLinkService para adicionar um novo parâmetro adicional EnableProxyProtocol.
* Correção da descrição incorreta do parâmetro na documentação de referência "New-AzApplicationGatewaySku"
* Novos cmdlets para suportar a política de firewall do Azure
* Adição de suporte para o recurso subordinado RouteTables de VirtualHub
    - Foram adicionados novos cmdlets:
        - Add-AzVirtualHubRoute
        - Add-AzVirtualHubRouteTable
        - Get-AzVirtualHubRouteTable
        - Remove-AzVirtualHubRouteTable
        - Set-AzVirtualHub
* Adição de suporte para o SKU de novas propriedades de VirtualHub e VirtualWANType de VirtualWan
    - Cmdlets atualizados com parâmetros adicionais:
        - New-AzVirtualHub : adição do parâmetro Sku
        - Update-AzVirtualHub : adição do parâmetro Sku
        - New-AzVirtualWan : adição do parâmetro VirtualWANType
        - Update-AzVirtualWan : adição do parâmetro VirtualWANType
* Adição de suporte para a propriedade EnableInternetSecurity para HubVnetConnection, VpnConnection e ExpressRouteConnection
    - Foram adicionados novos cmdlets:
        - Update-AzureRmVirtualHubVnetConnection
    - Cmdlets atualizados com parâmetros adicionais:
        - New-AzureRmVirtualHubVnetConnection : adição do parâmetro EnableInternetSecurity
        - New-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity
        - Update-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity
        - New-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity
        - Set-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity
* Adição de suporte para Configurar a Política WebApplicationFirewall de Nível Superior
    - Foram adicionados novos cmdlets:
        - New-AzApplicationGatewayFirewallPolicySetting
        - New-AzApplicationGatewayFirewallPolicyExclusion
        - New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride
        - New-AzApplicationGatewayFirewallPolicyManagedRuleOverride
        - New-AzApplicationGatewayFirewallPolicyManagedRule
        - New-AzApplicationGatewayFirewallPolicyManagedRuleSet
    - Cmdlets atualizados com parâmetros adicionais:
        - New-AzApplicationGatewayFirewallPolicy : adição do parâmetro PolicySetting, ManagedRule
* Adição de suporte para o operador GeoMatch em CustomRule
    - Adição de GeoMatch ao operador em FirewallCondition
* Adição de suporte para a Política de firewall perListener e perSite
    - Cmdlets atualizados com parâmetros adicionais:
        - New-AzApplicationGatewayHttpListener : adição do parâmetro FirewallPolicy, FirewallPolicyId
        - New-AzApplicationGatewayPathRuleConfig : adição do parâmetro FirewallPolicy, FirewallPolicyId
* Correção da sub-rede necessária com o nome AzureBastionSubnet em "PSBastion" pode não ser sensível às maiúsculas e minúsculas
* Suporte para FQDNs de Destino nas Regras de Rede e para FQDN Traduzido em Regras NAT para o Azure Firewall
* Adição de suporte para o recurso de nível superior RouteTables de IpGroup
    - Foram adicionados novos cmdlets:
        - New-AzIpGroup
        - Remove-AzIpGroup
        - Get-AzIpGroup
        - Set-AzIpGroup

#### <a name="azservicefabric"></a>Az.ServiceFabric
* Remoção do cmdlet Add-AzServiceFabricApplicationCertificate uma vez que este cenário é abrangido por Add-AzVmssSecret.

#### <a name="azsql"></a>Az.Sql
* Adição de suporte para o restauro de bases de dados removidas em Instâncias Geridas.
* Descontinuação dos cmdlets de auditoria antigos do código.
* Remoção de aliases descontinuados:
* Get-AzSqlDatabaseIndexRecommendations (utilize antes Get-AzSqlDatabaseIndexRecommendation)
* Get-AzSqlDatabaseRestorePoints (utilize antes Get-AzSqlDatabaseRestorePoint)
* Remoção do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy
* Remoção dos aliases dos cmdlets descontinuados das Definições de Avaliação de Vulnerabilidades
* Descontinuação dos cmdlets das Definições de Deteção Avançada de Ameaças
* Adição de cmdlets para Desativar e Ativar as recomendações de sensibilidade nas colunas de uma base de dados.

#### <a name="azstorage"></a>Az.Storage
* Suporte à ativação da partilha de Ficheiros de Grandes Dimensões ao criar ou atualizar uma Conta de armazenamento
    -  New-AzStorageAccount
    -  Set-AzStorageAccount
* Ao fechar/obter o Identificador de ficheiro, ignorar a verificação do caminho de entrada corresponde a Diretório de ficheiros ou Ficheiro, de forma a evitar a falha com o objeto no estado DeletePending
    -  Get-AzStorageFileHandle
    -  Close-AzStorageFileHandle

## <a name="280---october-2019"></a>2.8.0 - Outubro de 2019
### <a name="general"></a>Geral
* Versão Az.HealthcareApis 1.0.0

#### <a name="azaccounts"></a>Az.Accounts
* Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.

#### <a name="azapimanagement"></a>Az.ApiManagement
* **Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet
    - Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068

#### <a name="azautomation"></a>Az.Automation
* Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.

#### <a name="azbatch"></a>Az.Batch
* **Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.

#### <a name="azcompute"></a>Az.Compute
* Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss
* Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey
* Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.
* Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.

#### <a name="azdatafactory"></a>Az.DataFactory
* Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.
* Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.
* Atualização da versão do SDK .Net do ADF para 4.2.0

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio

#### <a name="azhealthcareapis"></a>Az.HealthcareApis
* Atualização da versão do PowerShell para 1.0.0
* Atualização da versão do SDK para 1.0.2
* Atualização em testes para mencionarem a nova versão do SDK
* Atualização da estrutura de saída de aninhada para bidimensional.

#### <a name="aziothub"></a>Az.IotHub
* Adição de nova origem de encaminhamento: DigitalTwinChangeEvents
* Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId

#### <a name="azmonitor"></a>Az.Monitor
* Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver
* Utilização do esquema de alerta comum ativada para os recetores. Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz
* Os Webhooks suportam agora a autenticação do Azure Active Directory.

#### <a name="aznetwork"></a>Az.Network
* Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.
* Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual
    - Foram adicionados novos cmdlets:
        - New-AzureRmTrafficSelectorPolicy
    - Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection
* Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede
    - cmdlets atualizados:
        - Add-AzNetworkSecurityRuleConfig
        - New-AzNetworkSecurityRuleConfig
        - Set-AzNetworkSecurityRuleConfig
* Melhoria do processamento de exceções em cmdlets Cortex
* Novas Gerações e SKUs para VirtualNetworkGateways
  - Introdução de novas Gerações para VirtualNetworkGateways.
  - Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.

#### <a name="azrediscache"></a>Az.RedisCache
* Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"

#### <a name="azsql"></a>Az.Sql
* Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida

#### <a name="azstorage"></a>Az.Storage
* Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0
* A listagem de contentores com a API de plano de gestão será feita com NextPageLink
    -  Get-AzRmStorageContainer
* A listagem de contas de armazenamento da subscrição será feita com NextPageLink
    -  Get-AzStorageAccount

#### <a name="azstoragesync"></a>Az.StorageSync
* Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.

#### <a name="azwebsites"></a>Az.Websites
* Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar

## <a name="270---september-2019"></a>2.7.0 - Setembro de 2019
#### <a name="azapimanagement"></a>Az.ApiManagement
* Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"
* Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência. Em alternativa, foi utilizado "Set-AzApiManagement".

#### <a name="azautomation"></a>Az.Automation
* Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"
* Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode
* Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.

#### <a name="azcompute"></a>Az.Compute
* Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig
* Adição do parâmetro Incremental a New-AzSnapshotConfig
* Adição de uma funcionalidade de máquina virtual de baixa prioridade:
    - Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.
    - O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.
* Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.
* Correção da exceção numa para Get-AzRemoteDesktopFile.
* Correção do método VHD Seek para a posição end-relative.
* Correção do problema de UltraSSD para New-AzVM e Update-AzVM.

#### <a name="azdatafactory"></a>Az.DataFactory
* Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus
* Atualização da versão do SDK .Net do ADF para 4.1.3

#### <a name="azhdinsight"></a>Az.HDInsight
* Chamada de alterações interruptivas

#### <a name="aziothub"></a>Az.IotHub
* Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.
* Adição de suporte para gerir o melhoramento de mensagens para um IotHub. Os novos cmdlets são:
    - Add-AzIotHubMessageEnrichment
    - Get-AzIotHubMessageEnrichment
    - Remove-AzIotHubMessageEnrichment
    - Set-AzIotHubMessageEnrichment

#### <a name="azmonitor"></a>Az.Monitor
* Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview
   - Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos. Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.
   - A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**. Os testes de cenário foram atualizados para acomodar esta alteração.
   - Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**. Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets. **NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.
   - A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior. Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.
   - A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior. Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.
* Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2
    - New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico
    - Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico
* Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)
 - Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)
 - O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda
 - Foram adicionados exemplos para o parâmetro opcional "ActionGroup"
 - Melhoria geral dos ficheiros de ajuda
* Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"

#### <a name="aznetwork"></a>Az.Network
* Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"
* Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote
* Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs
* Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes
* Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK
* Correção do mapeamento incorreto de modelos de Regra de Segurança
* Adição de propriedades à interface de rede para a funcionalidade de IP privado
    - Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface
    - Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration
    - Adição da nova classe de modelo PSIpConfigurationConnectivityInformation
* Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall
* Suporte de Multiligação na WAN Virtual
    - Novos cmdlets
        - New-AzVpnSiteLink
        - New-AzVpnSiteLinkConnection
    - Cmdlet atualizado:
        - New-VpnSite
        - Update-VpnSite
        - New-VpnConnection
        - Update-VpnConnection
* Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount
* Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original

#### <a name="azresources"></a>Az.Resources
* Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.

#### <a name="azservicefabric"></a>Az.ServiceFabric
* Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"
* Adição de novos cmdlets para a gestão de aplicações e serviços:
    - New-AzServiceFabricApplication
    - New-AzServiceFabricApplicationType
    - New-AzServiceFabricApplicationTypeVersion
    - New-AzServiceFabricService
    - Update-AzServiceFabricApplication
    - Get-AzServiceFabricApplication
    - Get-AzServiceFabricApplicationType
    - Get-AzServiceFabricApplicationTypeVersion
    - Get-AzServiceFabricService
    - Remove-AzServiceFabricApplication
    - Remove-AzServiceFabricApplicationType
    - Remove-AzServiceFabricApplicationTypeVersion
    - Remove-AzServiceFabricServic
* Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.

#### <a name="azsignalr"></a>Az.SignalR
* Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage

#### <a name="azsql"></a>Az.Sql
* Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"
* Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).
* Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy
* Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.
* Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).

#### <a name="azstorage"></a>Az.Storage
* Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"
* Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino
    -  Set-AzStorageFileContent
    -  Get-AzStorageFileContent
* Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.
    -  Set-AzStorageBlobContent
* Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão
    -  New-AzRmStorageShare
    -  Get-AzRmStorageShare
    -  Update-AzRmStorageShare
    -  Remove-AzRmStorageShare

#### <a name="azwebsites"></a>Az.Websites
* Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP
* Correção de Publish-AzureWebapp para funcionar no Linux e no Windows
* Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"

## <a name="260---august-2019"></a>2.6.0 - Agosto de 2019
#### <a name="general"></a>Geral
* Correção de diversos erros de digitação em vários módulos

#### <a name="azaccounts"></a>Az.Accounts
* Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)

#### <a name="azaks"></a>Az.Aks
* Correção do problema com a saída "Get-AzAks"
    * Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847

#### <a name="azapimanagement"></a>Az.ApiManagement
* Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351
    - Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId
* **Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.
  https://github.com/Azure/azure-powershell/issues/9482
* **New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752
* Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"

#### <a name="azbatch"></a>Az.Batch
* Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows

#### <a name="azcdn"></a>Az.Cdn
* Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN

#### <a name="azcompute"></a>Az.Compute
* VmssId adicionado ao cmdlet New-AzVMConfig
* Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss
* Propriedade HyperVGeneration adicionada ao objeto de imagem da VM
* Funcionalidades Host e HostGroup adicionadas
    - Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost
    - O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM
* Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto
* Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"

#### <a name="azdatafactory"></a>Az.DataFactory
* Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"
* Atualização da versão do SDK .Net do ADF para 4.1.2
* Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime
* PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.

#### <a name="azeventhub"></a>Az.EventHub
* Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet
* Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT
* Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace
* Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta

#### <a name="azmarketplaceordering"></a>Az.MarketplaceOrdering
* Correção do erro de digitação na documentação em que "Azure" estava em minúsculas

#### <a name="azmonitor"></a>Az.Monitor
* Foi corrigido nome de parâmetro incorreto na documentação de ajuda

#### <a name="aznetwork"></a>Az.Network
* New-AzPrivateLinkServiceIpConfig atualizado
    - O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.
    - Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.
* Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados
* Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.
* Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.
* Descrição atualizada do parâmetro Location para AzNetworkServiceTag

#### <a name="azoperationalinsights"></a>Az.OperationalInsights
* Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"
    - Exemplo adicionado
    - Descrição atualizada para o parâmetro "-Name"
* Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource
* Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"

#### <a name="azresources"></a>Az.Resources
* Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource
    - Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades
    - Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo
* Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda

#### <a name="azservicebus"></a>Az.ServiceBus
* Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet
* Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta
* Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico

#### <a name="azservicefabric"></a>Az.ServiceFabric
* Correção de erros no cmdlet de tipo de nó:
    - Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric. Correção do problema: https://github.com/Azure/azure-powershell/issues/8681
    - Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster. Correção do problema: https://github.com/Azure/azure-powershell/issues/8407
    - Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate

#### <a name="azsql"></a>Az.Sql
* Documentação dos cmdlets de Auditoria antigos atualizada.

#### <a name="azstorage"></a>Az.Storage
* Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas
* Suporte de StandardBlobTier no blob de carregamento e de cópia
    -  Set-AzStorageBlobContent
    -  Start-AzStorageBlobCopy
* Suporte de Rehydrate Priority no blob de cópia
    -  Start-AzStorageBlobCopy

#### <a name="azwebsites"></a>Az.Websites
* Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot

## <a name="250---july-2019"></a>2.5.0 - Julho de 2019
#### <a name="azaccounts"></a>Az.Accounts
* Atualizar o código comum para utilizar a versão mais recente do ClientRuntime

#### <a name="azapplicationinsights"></a>Az.ApplicationInsights
* Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"

#### <a name="azautomation"></a>Az.Automation
* Correção do erro de digitação na cadeia de recursos

#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* Adicionado suporte de NetworkRuleSet.

#### <a name="azcompute"></a>Az.Compute
* Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.

#### <a name="azcontainerregistry"></a>Az.ContainerRegistry
* Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação
    - Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633

#### <a name="azdatafactory"></a>Az.DataFactory
* Atualização da versão do SDK .Net do ADF para 4.1.0
* Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"

#### <a name="azeventhub"></a>Az.EventHub
* Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken
* Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído

#### <a name="azkeyvault"></a>Az.KeyVault
* Adicionado suporte para especificar o KeySize das Políticas de Certificado

#### <a name="azlogicapp"></a>Az.LogicApp
* Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa
    - Adicionado novo parâmetro MapType para filtragem

#### <a name="azmanagedservices"></a>Az.ManagedServices
* Adicionado suporte para a versão de API 2019-06-01 (GA)

#### <a name="aznetwork"></a>Az.Network
* Adicionado suporte para ponto final privado e serviço de ligação privada
    - Novos cmdlets
        - Set-AzPrivateEndpoint
        - Set-AzPrivateLinkService
        - Approve-AzPrivateEndpointConnection
        - Deny-AzPrivateEndpointConnection
        - Get-AzPrivateEndpointConnection
        - Remove-AzPrivateEndpointConnection
        - Test-AzPrivateLinkServiceVisibility
        - Get-AzAutoApprovedPrivateLinkService
* Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork
    - Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig
        - Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.
        - Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.
* O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade
* Ativação do protocolo ICMP para configurações de regra de segurança de rede
    - Cmdlets atualizados
        - Add-AzNetworkSecurityRuleConfig
        - New-AzNetworkSecurityRuleConfig
        - Set-AzNetworkSecurityRuleConfig
* Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection
* Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration
    - Cmdlet atualizado:
        - New-AzLoadBalancerFrontendIpConfig
        - Add-AzLoadBalancerFrontendIpConfig
        - Set-AzLoadBalancerFrontendIpConfig
* Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda
    - Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end. Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.

#### <a name="azoperationalinsights"></a>Az.OperationalInsights
* Atualização da versão predefinida das pesquisas guardadas como 1.
* Correção do processamento de regex nula de registo personalizado

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* Atualização de "Get-AzRecoveryServicesBackupJob.md"
* Atualização de "Get-AzRecoveryServicesBackupContainer.md"
* Atualização de "Get-AzRecoveryServicesVault.md"
* Atualização de "Wait-AzRecoveryServicesBackupJob.md"
* Atualização de "Set-AzRecoveryServicesVaultContext.md"
* Atualização de "Get-AzRecoveryServicesBackupItem.md"
* Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"
* Atualização de "Restore-AzRecoveryServicesBackupItem.md"
* Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure
* Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"

#### <a name="azresources"></a>Az.Resources
- Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"
- Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01

#### <a name="azservicebus"></a>Az.ServiceBus
* Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken
* Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído

#### <a name="azsql"></a>Az.Sql
* Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary
* Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail
* Correção de um pequeno erro de digitação numa mensagem de aviso.

#### <a name="azstorage"></a>Az.Storage
* Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto

#### <a name="azstoragesync"></a>Az.StorageSync
* A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.
* Correção do Problema 9551 referente a TierFilesOlderThanDays

#### <a name="azwebsites"></a>Az.Websites
* Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp
* Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp
* Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp

## <a name="240---july-2019"></a>2.4.0 - Julho de 2019
#### <a name="azaccounts"></a>Az.Accounts
* Adicionar suporte para cmdlets de perfil
* Adicionar suporte para ambientes e planos de dados nos cmdlets gerados
* Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell

#### <a name="azadvisor"></a>Az.Advisor
* Versão GA do Az.Advisor
* Este módulo está agora incluído como parte do módulo `Az` de rollup

#### <a name="azapimanagement"></a>Az.ApiManagement
* Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671
    - **Get-AzApiManagementSubscription**
        - Foi adicionado suporte para consultar subscrições por Utilizador e Produto
        - Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"
* Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432
    - **Import-AzApiManagementApi**
        - Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis

#### <a name="azautomation"></a>Az.Automation
* Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).

#### <a name="azcompute"></a>Az.Compute
* Adicionar parâmetro HyperVGeneration a New-AzImageConfig

#### <a name="azdatafactory"></a>Az.DataFactory
* A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.

#### <a name="azeventgrid"></a>Az.EventGrid
* Corrigir erro de digitação na documentação "New-AzEventGridSubscription"

#### <a name="aziothub"></a>Az.IotHub
* Adicione suporte para regenerar chaves de política de autorização.

#### <a name="aznetwork"></a>Az.Network
* Foi adicionado "RoutingPreference" para etiquetas de IP público
* Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"

#### <a name="azpolicyinsights"></a>Az.PolicyInsights
* Corrigir problema de referência nula em Get-AzPolicyState
    - Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446

#### <a name="azoperationalinsights"></a>Az.OperationalInsights
* Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* Corrigir para o comando get-policy para IaaSVMs

#### <a name="azresources"></a>Az.Resources
    - Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top
    - Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias
    - Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject
    - Várias atualizações de documento e exemplo para cmdlets de Política

#### <a name="azservicebus"></a>Az.ServiceBus
* Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes

#### <a name="azsql"></a>Az.Sql
* Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública
* Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.
    - Set-AzSqlServerAudit
    - Get-AzSqlServerAudit
    - Remove-AzSqlServerAudit
    - Set-AzSqlDatabaseAudit
    - Get-AzSqlDatabaseAudit
    - Remove-AzSqlDatabaseAudit
* Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades

#### <a name="azstorage"></a>Az.Storage
* Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:
    -  Enable-AzStorageStaticWebsite
* Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo
* Mostrar mais informações de erro quando o cmdlet falhou com o StorageException
* Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure
    -  New-AzStorageAccount
    -  Set-AzStorageAccount
* Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro
    - Get-AzStorageFileHandle
    - Close-AzStorageFileHandle

#### <a name="azstoragesync"></a>Az.StorageSync
* Este módulo está agora incluído como parte do módulo `Az` de rollup

## <a name="232---june-2019"></a>2.3.2 - Junho de 2019
#### <a name="azaccounts"></a>Az.Accounts
* Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções
    - Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983
* Correção de problema em aliases de cmdlets do AzureRM para Az
  - Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic
  - Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest

#### <a name="azcompute"></a>Az.Compute
* Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".
* Correção de erro de digitação na documentação de referência "New-AzVM"

#### <a name="azdns"></a>Az.Dns
* Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".

#### <a name="azeventgrid"></a>Az.EventGrid
* Atualizado para utilizar a versão de API 2019-06-01.
* Novos cmdlets:
    - New-AzureRmEventGridDomain
        - Cria um novo Domínio do Azure Event Grid.
    - Get-AzureRmEventGridDomain
        - Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.
    - Remove-AzureRmEventGridDomain
        - Remove um Domínio do Azure Event Grid.
    - New-AzureRmEventGridDomainKey
        - Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.
    - Get-AzureRmEventGridDomainKey
        - Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.
    - New-AzureRmEventGridDomainTopic:
        - Cria um novo Tópico de Domínio do Azure Event Grid.
    - Get-AzureRmEventGridDomainTopic
        - Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual
    - Remove-AzureRmEventGridDomainTopic:
        - Remove um Tópico de Domínio do Azure Event Grid existente.
* cmdlets atualizados:
    - New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:
        - Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.
        - Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.
        - Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).
        - Foram adicionados novos parâmetros opcionais para especificar:
            - Data de expiração da subscrição de eventos,
            - Parâmetros de filtragem avançada.
        - Adição de uma nova enumeração para servicebusqueue como destino.
        - Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por
    - Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:
        - Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.
    - Remove-AzureRmEventGridSubscription
        - Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.
        - Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.

#### <a name="azfrontdoor"></a>Az.FrontDoor
* New-AzFrontDoorWafMatchConditionObject
    - Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)
* New-AzFrontDoorWafManagedRuleObject
    - Adição de novos valores de preenchimento automático

#### <a name="aznetwork"></a>Az.Network
* Adição de suporte para o Recurso de Gateway de Rede Virtual
    - Novos cmdlets
        - Get-AzVirtualNetworkGatewayVpnClientConnectionHealth
* Adição de AvailablePrivateEndpointType
    - Novos cmdlets
        - Get-AzAvailablePrivateEndpointType
* Adição de PrivatePrivateLinkService
    - Novos cmdlets
        - Get-AzPrivateLinkService
        - New-AzPrivateLinkService
        - Remove-AzPrivateLinkService
        - New-AzPrivateLinkServiceIpConfig
        - Set-AzPrivateEndpointConnection
* Adição de PrivateEndpoint
    - Novos cmdlets
        - Get-AzPrivateEndpoint
        - New-AzPrivateEndpoint
        - Remove-AzPrivateEndpoint
        - New-AzPrivateLinkServiceConnection
* Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection
    - New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.
    - Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.
* Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.
* Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.
* Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit
* Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration
* Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.
* Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration
* Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças
* Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway
* Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway
* Foi adicionado o cmdlet Get-AzNetworkServiceTag
* Adição de suporte para vários endereços IP públicos para o Azure Firewall
    - cmdlet New-AzFirewall atualizado:
        - Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público
        - Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual
        - Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada
        - Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName
* Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.
    - New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.
    - Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.
    - Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.

#### <a name="azoperationalinsights"></a>Az.OperationalInsights
* Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"

#### <a name="azresources"></a>Az.Resources
* Suporte para opções adicionais de Exportação de Modelo
    - Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup
    - Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup
    - Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados

#### <a name="azservicefabric"></a>Az.ServiceFabric
* Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos

#### <a name="azsql"></a>Az.Sql
* Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection
* Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection
* Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas
   - Add-AzSqlInstanceKeyVaultKey
   - Get-AzSqlInstanceKeyVaultKey
   - Remove-AzSqlInstanceKeyVaultKey
   - Get-AzSqlInstanceTransparentDataEncryptionProtector
   - Set-AzSqlInstanceTransparentDataEncryptionProtector

#### <a name="azstorage"></a>Az.Storage
* Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento
    - New-AzStorageAccount
* Foi clarificada a descrição do cmdlet de imutabilidade do blob
    -  Remove-AzRmStorageContainerImmutabilityPolicy

#### <a name="azwebsites"></a>Az.Websites
* Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente
* Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot

## <a name="220---june-2019"></a>2.2.0 - Junho de 2019
#### <a name="azcdn"></a>Az.Cdn
* Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.

#### <a name="azcompute"></a>Az.Compute
* Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.
    - cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM

#### <a name="azeventhub"></a>Az.EventHub
* Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas
* Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName

#### <a name="aznetwork"></a>Az.Network
* Atualização de ResourceId e InputObject para o NAT Gateway
    - Adição do alias para ResourceId e InputObject

#### <a name="azpolicyinsights"></a>Az.PolicyInsights
* Correção do problema de referência Null em Get-AzPolicyEvent

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* Retenção mínima da política IaaSVM em dias alterada de 1 para 7

#### <a name="azservicebus"></a>Az.ServiceBus
* Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName

#### <a name="azservicefabric"></a>Az.ServiceFabric
* Correção da mensagem de erro para "Update-AzServiceFabricReliability"
* Correção do caráter em falta nos cmdlines do Service Fabric

#### <a name="azsql"></a>Az.Sql
* Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.
* Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy
* Mudança do nome dos cmdlets para o Advanced Threat Protection
* Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.

#### <a name="azwebsites"></a>Az.Websites
* corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas

## <a name="210---may-2019"></a>2.1.0 - Maio de 2019
#### <a name="azapimanagement"></a>Az.ApiManagement
* Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API
    - **Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado
    - **New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API
    - **New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo
    - **New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.
    - **New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico
    - **Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API
    - **Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API
* Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement
    - **Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches
    - **New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica
    - **Remove-AzApiManagementCache** - permite remover uma cache
    - **Update-AzApiManagementCache** - permite atualizar uma cache
* Foram criados novos Cmdlets para gerir o Esquema da API
    - **New-AzApiManagementSchema** - permite criar um novo Esquema para uma API
    - **Get-AzApiManagementSchema** - permite obter os esquemas configurados na API
    - **Remove-AzApiManagementSchema** - permite remover o esquema configurado na API
    - **Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API
* Foi criado o novo Cmdlet para gerar um Token de Utilizador.
    - **New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./
* Foi criado um novo cmdlet para obter o Estado da Rede
    - **Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API. Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.
* Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement
    - Foi adicionado suporte para o novo SKU "Consumption"
    - Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"
    - O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end". Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.
    - Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.
* Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada
* Foi atualizado o cmdlet para apresentar Mensagens de Erro inline
     > PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]
* Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"
* Foi atualizado o cmdlet **Import-AzApiManagementApi**
    - Para importar a API da especificação de documento "OpenApi 3.0"
    - Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").
    - Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.
* Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"
* Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"
* Foi atualizado o cmdlet **New-AzApiManagementApi**
    - Para configurar a API com o servidor de autorização "OpenId".
    - Para criar uma API num "ApiVersionSet"
    - Para clonar uma API com "SourceApiId" e "SourceApiRevision".
    - Capacidade de configurar "SubscriptionRequired" no âmbito da API.
* Foi atualizado o cmdlet **Set-AzApiManagementApi**
    - Para configurar a API com o servidor de autorização "OpenId".
    - Para atualizar uma API num "ApiVersionSet"
    - Capacidade de configurar "SubscriptionRequired" no âmbito da API.
* Foi atualizado o cmdlet **New-AzApiManagementRevision**
    - Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision". A nova Revisão assume o "ApiId" do elemento principal.
    - Para fornecer uma "ApiRevisionDescription"
    - Para substituir o "ServiceUrl" ao clonar uma API.
* Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**
    - Para configurar "AAD" ou "AADB2C" com uma "Autoridade"
    - Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"
* Foi atualizado o cmdlet **New-AzApiManagementSubscription**
    - Para considerar o novo SubscriptonModel com "Scope" e "UserId"
    - Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"
    - Adição do suporte para ativar "AllowTracing" ao nível da subscrição.
* Foi atualizado o cmdlet **Set-AzApiManagementSubscription**
    - Para considerar o novo SubscriptonModel com "Scope" e "UserId"
    - Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"
    - Adição do suporte para ativar "AllowTracing" ao nível da subscrição.
* Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada
    - "New-AzApiManagementContext"
        > New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso
    - "Get-AzApiManagementApiRelease"
        > Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId
    - "Get-AzApiManagementApiVersionSet"
        > Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset
    - "Get-AzApiManagementAuthorizationServer"
    - "Get-AzApiManagementBackend"
        > Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric
    - "Get-AzApiManagementCertificate"
    - "Remove-AzApiManagementApiVersionSet"
    - "Remove-AzApiManagementSubscription"

#### <a name="azautomation"></a>Az.Automation
* Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.
    - Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977
    - Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600
* Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.
    * Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347
* Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós. Agora devolve apenas o nó correspondente.

#### <a name="azcompute"></a>Az.Compute
* Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.
* O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure

#### <a name="azmonitor"></a>Az.Monitor
* Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda

#### <a name="aznetwork"></a>Az.Network
* Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas
    - Cmdlet atualizado:
        - Get-AzEffectiveRouteTable
* Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate

#### <a name="azresources"></a>Az.Resources
* Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação

#### <a name="azsql"></a>Az.Sql
* Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição

## <a name="200---may-2019"></a>2.0.0 - Maio de 2019
#### <a name="azaccounts"></a>Az.Accounts
* Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe

#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.
* Correção do erro quando a criação da conta falha.

#### <a name="azcompute"></a>Az.Compute
* Funcionalidade do grupo de colocação em proximidade.
    - Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup
    - O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig
* O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.
* TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.
* O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss
* Alterações interruptivas
    - Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.
    - Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.

#### <a name="azdeploymentmanager"></a>Az.DeploymentManager
* Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure

#### <a name="azdns"></a>Az.Dns
* Delegação de NameServer de DNS automática
    - A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.
    - Adiciona os registos NS na zona principal para a zona subordinada recém-criada.

#### <a name="azfrontdoor"></a>Az.FrontDoor
* Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service
* Alteração do nome dos cmdlets da WAF para incluir "Waf"
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a>Az.HDInsight
* Foram removidos dois cmdlets:
    - Grant-AzHDInsightHttpServicesAccess
    - Revoke-AzHDInsightHttpServicesAccess
* Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess
* O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:
    - Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.
    - Os utilizadores com a função de operador do HDInsight não serão afetados.

#### <a name="azmonitor"></a>Az.Monitor
* Novos cmdlets para a API SQR (Regra de Consulta Agendada)
    - New-AzScheduledQueryRuleAlertingAction
    - New-AzScheduledQueryRuleAznsActionGroup
    - New-AzScheduledQueryRuleLogMetricTrigger
    - New-AzScheduledQueryRuleSchedule
    - New-AzScheduledQueryRuleSource
    - New-AzScheduledQueryRuleTriggerCondition
    - New-AzScheduledQueryRule
    - Get-AzScheduledQueryRule
    - Set-AzScheduledQueryRule
    - Update-AzScheduledQueryRule
    - Remove-AzScheduledQueryRule
    - [Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR
    - Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)

#### <a name="aznetwork"></a>Az.Network
* Foi adicionado suporte para o Recurso de Gateway de NAT
    - Novos cmdlets
        - New-AzNatGateway
        - Get-AzNatGateway
        - Set-AzNatGateway
        - Remove-AzNatGateway
   - Cmdlets atualizados
        - New-AzureVirtualNetworkSubnetConfigCommand
        - Add-AzureVirtualNetworkSubnetConfigCommand
* Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.
    - New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.
    - Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.

#### <a name="azpolicyinsights"></a>Az.PolicyInsights
* Suporte para consultar os detalhes de avaliação da política.
    - Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState. Suporte para "-Expand PolicyEvaluationDetails".

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* Suporte para recuperação de sites Azure para o Azure entre subscrições.
* Marcação das próximas alterações interruptivas do Azure Site Recovery.
* Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.
* Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.
* Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.
* Outras pequenas correções.

#### <a name="azrelay"></a>Az.Relay
* Corrigir erros de digitação nas mensagens direcionadas ao cliente

#### <a name="azservicebus"></a>Az.ServiceBus
* Adicionados novos cmdlets para o NetworkRuleSet do Namespace

#### <a name="azstorage"></a>Az.Storage
* Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")
* Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.
* A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"
    - New-AzStorageAccount
* Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")
    - New-AzStorageAccount
    - Get-AzStorageAccount
    - Set-AzStorageAccount

#### <a name="azwebsites"></a>Az.Websites
* A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp
* Marcação de Get-AzWebApp*Metrics e Get-AzAppServicePlanMetrics preterida

## <a name="180---april-2019"></a>1.8.0 - Abril de 2019
### <a name="highlights-since-the-last-major-release"></a>Destaques desde a última versão principal
* Disponibilidade geral do módulo `Az`
* Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce
* Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/
* Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network
* Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1
* Adicionado o suporte para runbooks do Python 2 em Az.Automation
* Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote

#### <a name="azaccounts"></a>Az.Accounts
* Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac

#### <a name="azbatch"></a>Az.Batch
* Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.

#### <a name="azcdn"></a>Az.Cdn
* Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.

#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.

#### <a name="azcompute"></a>Az.Compute
* Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas
* Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.
* Corrigida a documentação sobre carateres universais

#### <a name="azdatafactory"></a>Az.DataFactory
* Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.

#### <a name="azeventgrid"></a>Az.EventGrid
* Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.

#### <a name="azeventhub"></a>Az.EventHub
* Adicionados novos cmdlets para o NetworkRuleSet do Namespace

#### <a name="azhdinsight"></a>Az.HDInsight
* Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.

#### <a name="aziothub"></a>Az.IotHub
* Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.

#### <a name="azkeyvault"></a>Az.KeyVault
* Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.
* Corrigida a documentação sobre carateres universais

#### <a name="azmachinelearning"></a>Az.MachineLearning
* Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.

#### <a name="azmedia"></a>Az.Media
* Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.

#### <a name="azmonitor"></a>Az.Monitor
  * Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)
      - New-AzMetricAlertRuleV2DimensionSelection
      - New-AzMetricAlertRuleV2Criteria
      - Remove-AzMetricAlertRuleV2
      - Get-AzMetricAlertRuleV2
      - Add-AzMetricAlertRuleV2
  * Atualizado o SDK de Monitor para a versão 0.22.0-preview

#### <a name="aznetwork"></a>Az.Network
* Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.
* Corrigida a documentação sobre carateres universais

#### <a name="aznotificationhubs"></a>Az.NotificationHubs
* Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.

#### <a name="azoperationalinsights"></a>Az.OperationalInsights
* Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.

#### <a name="azpowerbiembedded"></a>Az.PowerBIEmbedded
* Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.
* Atualizado o formato de tabela para SQL na VM do Azure
* Adicionado um método alternativo para obter a localização no AzureFileShare
* ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário

#### <a name="azrediscache"></a>Az.RedisCache
* Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.

#### <a name="azresources"></a>Az.Resources
* Corrigida a documentação sobre carateres universais

#### <a name="azsql"></a>Az.Sql
* Substitua a dependência do Monitor de SDK com um código comum
* Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.
* Melhorado o processo de classificação de várias colunas.
* Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.
* Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.
* Suporte para o parâmetro de fuso horário na criação de Instância Gerida.
* Corrigida a documentação sobre carateres universais

#### <a name="azwebsites"></a>Az.Websites
* corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar
* Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.
* Atualizado o SDK dos Websites.
* Removida a propriedade AdminSiteName de PSAppServicePlan.

## <a name="170---april-2019"></a>1.7.0 - Abril de 2019
### <a name="highlights-since-the-last-major-release"></a>Destaques desde a última versão principal
* Disponibilidade geral do módulo `Az`
* Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce
* Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/
* Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network
* Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1
* Adicionado o suporte para runbooks do Python 2 em Az.Automation
* Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote

#### <a name="azaccounts"></a>Az.Accounts
* Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId

#### <a name="azanalysisservices"></a>Az.AnalysisServices
* Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original
* Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva

#### <a name="azautomation"></a>Az.Automation
* Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões. Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.
* Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure

#### <a name="azcompute"></a>Az.Compute
* Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig
* Permitir a criação de VM com imagem de galeria de outros inquilinos.

#### <a name="azcontainerinstance"></a>Az.ContainerInstance
* Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita

#### <a name="azdatafactory"></a>Az.DataFactory
* Atualização da versão do SDK de .Net do ADF para 3.0.2
* Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.

#### <a name="azresources"></a>Az.Resources
* Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"
* Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"
    - Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando
    - Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856
* Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas
    - Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856

#### <a name="azsql"></a>Az.Sql
* Suporte para a Classificação de Dados de Base de Dados.

#### <a name="azstorage"></a>Az.Storage
* Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure
    - New-AzStorageContext
* Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão
    - Update-AzStorageBlobServiceProperty
    - Get-AzStorageBlobServiceProperty
    - Enable-AzStorageBlobDeleteRetentionPolicy
    - Disable-AzStorageBlobDeleteRetentionPolicy
* Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets
    - Get-AzStorageBlobContent
    - Set-AzStorageBlobContent
    - Get-AzStorageFileContent
    - Set-AzStorageFileContent

## <a name="160---march-2019"></a>1.6.0 - março de 2019
### <a name="highlights-since-the-last-major-release"></a>Destaques desde a última versão principal
* Disponibilidade geral do módulo `Az`
* Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce
* Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/
* Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network
* Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1
* Adicionado o suporte para runbooks do Python 2 em Az.Automation
* Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote

#### <a name="azautomation"></a>Az.Automation
* Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:
    * Agrupamento dinâmico
    * Script de pré-publicação
    * Definição de reinício

#### <a name="azcompute"></a>Az.Compute
* Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData
* Atualização da biblioteca de cliente de Computação para 25.0.0.

#### <a name="azkeyvault"></a>Az.KeyVault
* Foi adicionado o suporte a carateres universais para os cmdlets KeyVault

#### <a name="aznetwork"></a>Az.Network
* Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall
* Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo
* Adicionado o suporte a pipe para anular o registo a contentores

#### <a name="azresources"></a>Az.Resources
* Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup
* Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM

#### <a name="azsql"></a>Az.Sql
* alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.

#### <a name="azstorage"></a>Az.Storage
* Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento
    - Set-AzStorageAccountManagementPolicy
    - Get-AzStorageAccountManagementPolicy
    - Remove-AzStorageAccountManagementPolicy
    - Add-AzStorageAccountManagementPolicyAction
    - New-AzStorageAccountManagementPolicyFilter
    - New-AzStorageAccountManagementPolicyRule

#### <a name="azwebsites"></a>Az.Websites
* Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"

## <a name="150---march-2019"></a>1.5.0 – Março de 2019
#### <a name="azaccounts"></a>Az.Accounts
* Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados
* Foram atualizados os exemplos de Connect-AzAccount

#### <a name="azautomation"></a>Az.Automation
* Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure
* Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais. Devolve agora todos os nós

#### <a name="azcdn"></a>Az.Cdn
* Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos

#### <a name="azcompute"></a>Az.Compute
* Foi adicionado o suporte de carateres universais para cmdlets Get

#### <a name="azdatafactory"></a>Az.DataFactory
* Foi atualizada a versão do SDK .NET do ADF para a 3.0.1

#### <a name="azlogicapp"></a>Az.LogicApp
* Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados

#### <a name="aznetwork"></a>Az.Network
* Foi adicionado o suporte de carateres universais para cmdlets Network

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* Foi adicionado um servidor SQL ao suporte de VM do Azure
* Atualização do SDK
* Foi removida a verificação VMappContainer em Get-ProtectableItem
* Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem

#### <a name="azresources"></a>Az.Resources
* Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação
    - Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933
* Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`
    - Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240
* Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`
    - Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930

#### <a name="azsql"></a>Az.Sql
* AuditingEndpointsCommunicator está a ser atualizado.
    - Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.

#### <a name="azstorage"></a>Az.Storage
* Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount

## <a name="140---february-2019"></a>1.4.0 – Fevereiro de 2019
#### <a name="azanalysisservices"></a>Az.AnalysisServices
* O cmdlet AddAzureASAccount foi preterido

#### <a name="azautomation"></a>Az.Automation
* Atualização da ajuda para Import-AzAutomationDscNodeConfiguration
* Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration
* Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration

#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.

#### <a name="azcompute"></a>Az.Compute
* Foi corrigido o problema com os conjuntos de parâmetros de ID
* Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name
* Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage
* O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL

#### <a name="azeventhub"></a>Az.EventHub
* Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub

#### <a name="azkeyvault"></a>Az.KeyVault
* Foi corrigida a etiquetagem em Set-AzKeyVaultSecret

#### <a name="azlogicapp"></a>Az.LogicApp
* Adição de sku básico para Contas de Integração
* Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos
* Novos cmdlets para Assemblies de Contas de Integração
    - Get-AzIntegrationAccountAssembly
    - New-AzIntegrationAccountAssembly
    - Remove-AzIntegrationAccountAssembly
    - Set-AzIntegrationAccountAssembly
* Novos cmdlets para Configuração de Lote de Contas de Integração
    - Get-AzIntegrationAccountBatchConfiguration
    - New-AzIntegrationAccountBatchConfiguration
    - Remove-AzIntegrationAccountBatchConfiguration
    - Set-AzIntegrationAccountBatchConfiguration
* Atualização do SDK de Aplicação Lógica para a versão 4.1.0

#### <a name="azmonitor"></a>Az.Monitor
* Atualização da ajuda para Get-AzMetric

#### <a name="aznetwork"></a>Az.Network
* Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError

#### <a name="azoperationalinsights"></a>Az.OperationalInsights
* Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.
    - Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.
    - Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.

#### <a name="azresources"></a>Az.Resources
* Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166
* Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235
* Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219
* Correção de erro que impedia a criação repetida de KeyCredentials

#### <a name="azsql"></a>Az.Sql
* Suporte adicionado para a camada Hyperscale da BD SQL
* Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro

#### <a name="azwebsites"></a>Az.Websites
* Correção de exemplo em Get-AzWebAppSlotMetrics

## <a name="130---february-2019"></a>1.3.0 - Fevereiro de 2019
#### <a name="azaccounts"></a>Az.Accounts
* Atualização para a versão mais recente do ClientRuntime

#### <a name="azanalysisservices"></a>Az.AnalysisServices
Disponibilidade geral para o módulo Az.AnalysisServices.

#### <a name="azcompute"></a>Az.Compute
* Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80
* Descrição de ajuda atualizada para Set-AzVMBootDiagnostics
* Descrição de ajuda e exemplo atualizados para Update-AzImage

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
Disponibilidade geral para o módulo Az.RecoveryServices.

#### <a name="azresources"></a>Az.Resources
* As etiquetas dos grupos de recursos foram corrigidas
    - Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166
* Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction
    - Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235

#### <a name="azsql"></a>Az.Sql
* Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy
* Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL
* Exceção nullref corrigida em Get-AzSqlCapability

## <a name="121---january-2019"></a>1.2.1 - Janeiro de 2019
#### <a name="azaccounts"></a>Az.Accounts
* Lançamento da versão correta de Autenticação

#### <a name="azanalysisservices"></a>Az.AnalysisServices
* Versão com a dependência de Autenticação atualizada

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* Versão com a dependência de Autenticação atualizada

## <a name="120---january-2019"></a>1.2.0 - Janeiro de 2019
#### <a name="azaccounts"></a>Az.Accounts
* Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1
* Foram atualizados URLs de ajuda online incorretos
* Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm

#### <a name="azaks"></a>Az.Aks
* Foram atualizados URLs de ajuda online incorretos

#### <a name="azautomation"></a>Az.Automation
* Suporte adicionado para runbooks do Python 2
* Foram atualizados URLs de ajuda online incorretos

#### <a name="azcdn"></a>Az.Cdn
* Foram atualizados URLs de ajuda online incorretos

#### <a name="azcompute"></a>Az.Compute
* Foi adicionado o cmdlet Invoke-AzVMReimage
* Foi adicionado o parâmetro TempDisk a Set-AzVmss
* Foi corrigida a mensagem de aviso de New-AzVM

#### <a name="azcontainerregistry"></a>Az.ContainerRegistry
* Foram atualizados URLs de ajuda online incorretos

#### <a name="azdatafactory"></a>Az.DataFactory
* Foi atualizada a versão do SDK .NET do ADF para a 3.0.0

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI
    - Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462
* Foram atualizados URLs de ajuda online incorretos

#### <a name="aziothub"></a>Az.IotHub
* Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.

#### <a name="azkeyvault"></a>Az.KeyVault
* Foram atualizados URLs de ajuda online incorretos

#### <a name="aznetwork"></a>Az.Network
* Foram atualizados URLs de ajuda online incorretos

#### <a name="azresources"></a>Az.Resources
* Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"
* Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos
* Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode
* Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522
* Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747
* Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"
    - Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123

#### <a name="azservicefabric"></a>Az.ServiceFabric
* Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932
* Foram corrigidas algumas mensagens de erro.
* Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.
* Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.

#### <a name="azsignalr"></a>Az.SignalR
* Foram atualizados URLs de ajuda online incorretos

#### <a name="azsql"></a>Az.Sql
* Foram atualizados URLs de ajuda online incorretos
* Foi atualizada a descrição do parâmetro LicenseType com valores possíveis
* Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada
* Suporte para o agrupamento personalizado na instância gerida

#### <a name="azstorage"></a>Az.Storage
* Foram atualizados URLs de ajuda online incorretos
* Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.
    - Get/Set-AzStorageServiceLoggingProperty
    - Get/Set-AzStorageServiceMetricsProperty

#### <a name="aztrafficmanager"></a>Az.TrafficManager
* Foram atualizados URLs de ajuda online incorretos

#### <a name="azwebsites"></a>Az.Websites
* Foram atualizados URLs de ajuda online incorretos
* Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.
* Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação

## <a name="110---january-2019"></a>1.1.0 - Janeiro de 2019
#### <a name="azaccounts"></a>Az.Accounts
* Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias

#### <a name="azcompute"></a>Az.Compute
* O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage
* Foi atualizada a descrição do ID nos ficheiros de ajuda
* Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.
    - Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token

#### <a name="azeventgrid"></a>Az.EventGrid
* Foi atualizado para utilizar a versão de API 2019-01-01.
* Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01
    - New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:
        - TTL de Evento,
        - Número máximo de tentativas de entrega para os eventos,
        - Ponto final de mensagens não entregues.
    - Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:
        - TTL de Evento,
        - Número máximo de tentativas de entrega para os eventos,
        - Ponto final de mensagens não entregues.
* Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.
* É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.

#### <a name="aziothub"></a>Az.IotHub
* Foi atualizado para a versão mais recente do SDK IotHub

#### <a name="azlogicapp"></a>Az.LogicApp
* Get-AzLogicApp lista tudo sem um Nome especificado

#### <a name="azresources"></a>Az.Resources
* Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"
    - Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875
* Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition
* Foi corrigido o erro de digitação na documentação de New-AzDeployment
* Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"
    - Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220

#### <a name="azsignalr"></a>Az.SignalR
* Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts

#### <a name="azsql"></a>Az.Sql
* Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.

#### <a name="azstorage"></a>Az.Storage
* Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo
    - New-AzStorageContext
* Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo
    - New-AzStorageBlobSASToken

#### <a name="azwebsites"></a>Az.Websites
* Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"
* Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts

## <a name="100---december-2018"></a>1.0.0 - Dezembro de 2018
### <a name="general"></a>Geral

- Disponibilidade Geral do Módulo do Az
- Ajuda online para cada módulo
- Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)
- Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM

### <a name="azaccounts"></a>Az.Accounts
- Nome para o qual foi alterado o nome anterior Az.Profile
- Correção de formatos de tabela para tipos de perfil e de contexto

### <a name="azapimanagement"></a>Az.ApiManagement
- Correções para #7002
- Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes

### <a name="azbatch"></a>Az.Batch
- Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.
- A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.
- Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes

### <a name="azbilling"></a>Az.Billing
- Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes

### <a name="azcognitivservices"></a>Az.CognitivServices
- Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount
- Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus

### <a name="azcontainerinstance"></a>Az.ContainerInstance
- Foi adicionado suporte de ManagedIdentity

### <a name="azdatalakeanalytics"></a>Az.DataLakeAnalytics
- Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes

### <a name="azdatalakestore"></a>Az.DataLakeStore
- Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes

### <a name="azmonitor"></a>Az.Monitor
- O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes

### <a name="azkeyvault"></a>Az.KeyVault
- A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída

### <a name="azmachinelearning"></a>Az.MachineLearning
- Foram incluídos os cmdlets do módulo Az.MachineLearningCompute

### <a name="azmedia"></a>Az.Media
- Foi removido o alias preterido -Tags de New-AzMediaService

### <a name="aznetwork"></a>Az.Network
Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação
    - Foram adicionados novos cmdlets:
        - Add-AzureRmApplicationGatewayRewriteRuleSet
        - Get-AzureRmApplicationGatewayRewriteRuleSet
        - New-AzureRmApplicationGatewayRewriteRuleSet
        - Remove-AzureRmApplicationGatewayRewriteRuleSet
        - Set-AzureRmApplicationGatewayRewriteRuleSet
        - New-AzureRmApplicationGatewayRewriteRule
        - New-AzureRmApplicationGatewayRewriteRuleActionSet
        - New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration
    - Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet
        - New-AzureRmApplicationGateway
        - New-AzureRmApplicationGatewayRequestRoutingRule
        - Add-AzureRmApplicationGatewayRequestRoutingRule
        - New-AzureRmApplicationGatewayPathRuleConfig
        - Add-AzureRmApplicationGatewayUrlPathMapConfig
        - New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.
    - Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret
        - Add-AzApplicationGatewaySslCertificate
        - New-AzApplicationGatewaySslCertificate
        - Set-AzApplicationGatewaySslCertificate
    - O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity
- Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes

### <a name="azoperationalinsights"></a>Az.OperationalInsights
- Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes

### <a name="azprofile"></a>Az.Profile
- O nome do módulo foi alterado para Az.Accounts

### <a name="azrecoveryservices"></a>Az.RecoveryServices
- Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes

### <a name="azresources"></a>Az.Resources
- Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes

### <a name="azservicefabric"></a>Az.ServiceFabric
- Suporte para a especificação do certificado pelo nome comum e thumbprint
- Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes

### <a name="azsignalr"></a>Az.SIgnalR
- Disponibilidade Geral de cmdlets do PowerShell para o SignalR

### <a name="azsql"></a>Az.Sql
- Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças
- Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL
- Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes

### <a name="azstorage"></a>Az.Storage
- Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes

### <a name="azwebsites"></a>Az.Websites
- Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes

## <a name="070---december-2018"></a>0.7.0 - Dezembro de 2018

### <a name="general"></a>Geral

* Pequenas alterações para a futura transição do AzureRM para Az

### <a name="azcompute"></a>Az.Compute

* Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.

### <a name="azdatalakestore"></a>Az.DataLakeStore

* Foi corrigida a barra final do domínio da conta do ADLS

### <a name="azfrontdoor"></a>Az.FrontDoor

* Foram corrigidas algumas ligações quebradas
    - Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.
    - No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.

### <a name="azrecoveryservices"></a>Az.RecoveryServices

* Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.
* storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.

### <a name="azresources"></a>Az.Resources

* Correção para https://github.com/Azure/azure-powershell/issues/7679
    - Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.

### <a name="azsql"></a>Az.Sql

* Pequenas alterações para a futura transição do AzureRM para Az
* Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet
* Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.

### <a name="azstorage"></a>Az.Storage

* -EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount
* Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext
    - Start-AzureStorageFileCopy
* Suporte da configuração de Web Site Estático
    - Enable-AzureStorageStaticWebsite
    - Disable-AzureStorageStaticWebsite

### <a name="azwebsites"></a>Az.Websites

* Set-AzureRmWebApp e Set-AzureRmWebAppSlot
    - Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux. Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.

## <a name="061---november-2018"></a>0.6.1 - Novembro de 2018

### <a name="azapimanagement"></a>Az.ApiManagement
* Atualização das dependências para o problema do mapeamento de tipos

### <a name="azautomation"></a>Az.Automation
* Cmdlets da Automatização do Azure baseados no Swagger
* Adicionados cmdlets da Gestão de Atualizações
* Adicionados cmdlets de Controlo de Código Fonte
* Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup
* Corrigido o comando de Nó de Registo de DSC

### <a name="azcompute"></a>Az.Compute
* Corrigido o problema de identidade da identidade SystemAssigned
* Atualização das dependências para o problema do mapeamento de tipos

### <a name="azcontainerinstance"></a>Az.ContainerInstance
* Atualização das dependências para o problema do mapeamento de tipos

### <a name="azmarketplaceordering"></a>Az.MarketplaceOrdering
* Atualização da descrição dos exemplos dos cmdlets do marketplace

### <a name="aznetwork"></a>Az.Network
* Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError
* Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall
* Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.
* Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork

### <a name="azrecoveryservicesbackup"></a>Az.RecoveryServices.Backup
* Correção para modificar a política de uma partilha de ficheiros protegida.
* Conversão do fuso horário da política em maiúsculas.

### <a name="azrecoveryservicessiterecovery"></a>Az.RecoveryServices.SiteRecovery
* Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem
* Atualização das dependências para o problema do mapeamento de tipos

### <a name="azrelay"></a>Az.Relay
* Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.

### <a name="azresources"></a>Az.Resources
* Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`
* Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata
* Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703

### <a name="azservicefabric"></a>Az.ServiceFabric
* Adicionadas mensagens de preterição para futuras alterações interruptivas

### <a name="azsql"></a>Az.Sql
* Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure
    - Get-AzureRmSqlInstance
    - New-AzureRmSqlInstance
    - Set-AzureRmSqlInstance
    - Remove-AzureRmSqlInstance
    - Get-AzureRmSqlInstanceDatabase
    - New-AzureRmSqlInstanceDatabase
    - Restore-AzureRmSqlInstanceDatabase
    - Remove-AzureRmSqlInstanceDatabase
* Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.
    - Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.
    - Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.
    - Set-AzureRmSqlServerAuditing.
    - Get-AzureRmSqlServerAuditing.
    - Set-AzureRmSqlDatabaseAuditing.
    - Get-AzureRmSqlDatabaseAuditing.
* Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido

## <a name="050---november-2018"></a>0.5.0 - Novembro de 2018
#### <a name="general"></a>Geral
* Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa

#### <a name="azprofile"></a>Az.Profile
* Atualizar o código comum para utilizar a versão mais recente do ClientRuntime
* O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId
* A descrição de TenantId para Connect-AzAccount foi atualizada
* Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino
    - https://github.com/Azure/azure-powershell/issues/6936
* Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino
    - https://github.com/Azure/azure-powershell/issues/7453
* Corrigido o problema com os pontos finais DataLake ao utilizar MSI
    - https://github.com/Azure/azure-powershell/issues/7462
* Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.

#### <a name="azcompute"></a>Az.Compute
* Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk
* Get-AzVMImage mostra AutomaticOSUpgradeProperties
* Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* Atualizar o pacote DataLake para 1.1.10.
* Adicionada a Concorrência predefinida para operações com vários threads.

#### <a name="azinsights"></a>Az.Insights
* Corrigido o problema n.º 7267 (área de dimensionamento automático)
    - Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).
* Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição
    - Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado

#### <a name="aznetwork"></a>Az.Network
* Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-
    - Get-AzExpressRouteCircuitRouteTable
    - Get-AzExpressRouteCircuitARPTable
    - Get-AzExpressRouteCircuitRouteTableSummary
    - Get-AzExpressRouteCrossConnectionArpTable
    - Get-AzExpressRouteCrossConnectionRouteTable
    - Get-AzExpressRouteCrossConnectionRouteTableSummary

#### <a name="azpolicyinsights"></a>Az.PolicyInsights
* Adicionados os cmdlets de remediação de política

#### <a name="azresources"></a>Az.Resources
* Correção para https://github.com/Azure/azure-powershell/issues/7402
    - Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"

#### <a name="azservicebus"></a>Az.ServiceBus
* Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.

#### <a name="azservicefabric"></a>Az.ServiceFabric
* Corrigida a adição de certificado ao Linux VMSS.
* Correção de "Add-AzServiceFabricClusterCertificate"
    - Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).
    - Exibir corretamente a exceção (Azure/service-fabric-issues#1054).
* Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.

## <a name="040---october-2018"></a>0.4.0 - Outubro de 2018
#### <a name="azprofile"></a>Az.Profile
* Foi corrigido o problema de Get-AzSubscription no CloudShell
* Atualizar o código comum para utilizar a versão mais recente do ClientRuntime

#### <a name="azcompute"></a>Az.Compute
* Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"
* Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* Adicionar suporte para as Regras de Rede Virtual
    - Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.
    - Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.
    - Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.
    - Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.

#### <a name="aznetwork"></a>Az.Network
* Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.
* Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.

#### <a name="azresources"></a>Az.Resources
* Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário. Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".

## <a name="030---october-2018"></a>0.3.0 - Outubro de 2018
#### <a name="azurestorage"></a>Azure.Storage
* Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados
    - Start-AzureStorageBlobCopy
    - Start-AzureStorageFileCopy
* Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.
    - Get-AzStorageUsage

#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.

#### <a name="azcompute"></a>Az.Compute
* Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário
* Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.
* Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption

#### <a name="azdatafactoryv2"></a>Az.DataFactoryV2
* Atualização da versão do SDK .NET do ADF para a 2.3.0.

#### <a name="aznetwork"></a>Az.Network
* Adição da funcionalidade NetworkProfile. novos cmdlets adicionados
    - Get-AzNetworkProfile
    - New-AzNetworkProfile
    - Remove-AzNetworkProfile
    - Set-AzNetworkProfile
    - New-AzContainerNicConfig
    - New-AzContainerNicConfigIpConfig
* Adição de uma ligação de associação do serviço no Modelo de Sub-rede
* Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap
* Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig

#### <a name="azrediscache"></a>Az.RedisCache
* Permitir que qualquer cadeia como parâmetro Size permaneça. Adição de P5 no pop-up de PSArgumentCompleter

#### <a name="azresources"></a>Az.Resources
* Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition
* Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador

#### <a name="azsql"></a>Az.Sql
* Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure

#### <a name="azwebsites"></a>Az.Websites
* Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor
* Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows

## <a name="020---september-2018"></a>0.2.0 - Setembro de 2018
 Versão Inicial
