---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 04/30/2019
ms.openlocfilehash: 8a9a399f72ed9e3e9a3cbc09c8a4abaa91339c24
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/05/2020
ms.locfileid: "71319299"
---
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