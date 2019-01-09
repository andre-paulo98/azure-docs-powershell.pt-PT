## <a name="100---december-2018"></a>1.0.0 - Dezembro de 2018
### <a name="general"></a>Geral

- Disponibilidade Geral do Módulo do Az
- Ajuda online para cada módulo
- Para obter mais detalhes e um mapa, consulte a [página de Anúncio do módulo Az](https://aka.ms/azps-announce)
- Consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM

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
- Combina os cmdlets Billing, Consumption e UsageAggregates; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes

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
- O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes

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