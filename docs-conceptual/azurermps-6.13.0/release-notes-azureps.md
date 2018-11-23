---
title: Registo de alterações do Azure PowerShell | Microsoft Docs
description: Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 08/28/2018
ms.openlocfilehash: 7f517f0b3768a2075557b131158ee1264ea9ab3f
ms.sourcegitcommit: 80a3da199954d0ab78765715fb49793e89a30f12
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/22/2018
ms.locfileid: "52260006"
---
# <a name="release-notes"></a>Notas de versão

Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.

---
## <a name="6130---november-2018"></a>6.13.0 - Novembro de 2018
#### <a name="azurermprofile"></a>AzureRM.Profile
* Atualizar o código comum para utilizar a versão mais recente do ClientRuntime

#### <a name="azurermapimanagement"></a>AzureRM.ApiManagement
* Atualização das dependências para o problema do mapeamento de tipos

#### <a name="azurermautomation"></a>AzureRM.Automation
* Cmdlets da Automatização do Azure baseados no Swagger
* Adicionados cmdlets da Gestão de Atualizações
* Adicionados cmdlets de Controlo de Código Fonte
* Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup
* Corrigido o comando de Nó de Registo de DSC

#### <a name="azurermcompute"></a>AzureRM.Compute
* Corrigido o problema de identidade da identidade SystemAssigned
* Atualização das dependências para o problema do mapeamento de tipos

#### <a name="azurermcontainerinstance"></a>AzureRM.ContainerInstance
* Atualização das dependências para o problema do mapeamento de tipos

#### <a name="azurermmarketplaceordering"></a>AzureRM.MarketplaceOrdering
* Atualização da descrição dos exemplos dos cmdlets do marketplace

#### <a name="azurermnetwork"></a>AzureRM.Network
* Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError
* Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall
* Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta. 
* Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork

#### <a name="azurermrecoveryservicesbackup"></a>AzureRM.RecoveryServices.Backup
* Correção para modificar a política de uma partilha de ficheiros protegida.
* Conversão do fuso horário da política em maiúsculas.

#### <a name="azurermrecoveryservicessiterecovery"></a>AzureRM.RecoveryServices.SiteRecovery
* Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem
* Atualização das dependências para o problema do mapeamento de tipos

#### <a name="azurermrelay"></a>AzureRM.Relay
* Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.

#### <a name="azurermresources"></a>AzureRM.Resources
* Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`
* Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata
* Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703

#### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* Adicionadas mensagens de preterição para futuras alterações interruptivas

#### <a name="azurermsql"></a>AzureRM.Sql
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

## <a name="6120---november-2018"></a>6.12.0 - Novembro de 2018
#### <a name="azurermprofile"></a>AzureRM.Profile
* Atualizar o código comum para utilizar a versão mais recente do ClientRuntime
* Mudar o nome do parâmetro TenantId no cmdlet Connect-AzureRmAccount para Tenant e adicionar um alias para TenantId
* Descrição de TenantId atualizada para Connect-AzureRmAccount
* Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino
    - https://github.com/Azure/azure-powershell/issues/6936
* Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino
    - https://github.com/Azure/azure-powershell/issues/7453
* Corrigido o problema com os pontos finais DataLake ao utilizar MSI
    - https://github.com/Azure/azure-powershell/issues/7462
* Corrigido o problema em que "Disconnect-AzureRmAccount" é lançado se não estiver ligado
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azurermautomation"></a>AzureRM.Automation
* Foi mudado o nome do ficheiro DLL de cmdlett para Microsoft.Azure.Commands.Automation.dll

#### <a name="azurermcognitiveservices"></a>AzureRM.CognitiveServices
* Adicionar a operação Get-AzureRmCognitiveServicesAccountSkus.

#### <a name="azurermcompute"></a>AzureRM.Compute
* Adicionar os cmdlets Add-AzureRmVmssVMDataDisk e Remove-AzureRmVmssVMDataDisk
* Get-AzureRmVMImage mostra AutomaticOSUpgradeProperties
* Corrigidos os valores de opção SetAzureRmVMChefExtension -BootstrapOptions e -JsonAttribute no formato json.

#### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* Atualizar o pacote DataLake para 1.1.10.
* Adicionada a Concorrência predefinida para operações com vários threads.

#### <a name="azurerminsights"></a>AzureRM.Insights
* Corrigido o problema n.º 7267 (área de dimensionamento automático)
    - Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).
* Corrigido o problema n.º 7513 [Insights] Set-AzureRMDiagnosticSetting requer especificação explícita das categorias durante a criação da definição
    - Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado

#### <a name="azurermnetwork"></a>AzureRM.Network
* Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-
    - Get-AzureRmExpressRouteCircuitRouteTable
    - Get-AzureRmExpressRouteCircuitARPTable
    - Get-AzureRmExpressRouteCircuitRouteTableSummary
    - Get-AzureRMExpressRouteCrossConnectionArpTable
    - Get-AzureRMExpressRouteCrossConnectionRouteTable
    - Get-AzureRMExpressRouteCrossConnectionRouteTableSummary

#### <a name="azurermpolicyinsights"></a>AzureRM.PolicyInsights
* Adicionados os cmdlets de remediação de política

#### <a name="azurermrecoveryservicesbackup"></a>AzureRM.RecoveryServices.Backup
* Foi adicionado suporte para as partilhas de ficheiro do Azure nos serviços de recuperação.

#### <a name="azurermresources"></a>AzureRM.Resources
* Correção para https://github.com/Azure/azure-powershell/issues/7402
    - Permitir a listagem de recursos a utilizar o parâmetro "-ResourceId" para "-GetAzureRmResource"

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.

#### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* Corrigida a adição de certificado ao Linux VMSS.
* Correção de "Add-AzureRmServiceFabricClusterCertificate"
    - Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).
    - Exibir corretamente a exceção (Azure/service-fabric-issues#1054).
* Corrigir "Update-AzureRmServiceFabricDurability" para atualizar a configuração do cluster antes de iniciar a operação de VMSS CreateOrUpdate.

## <a name="6110---october-2018"></a>6.11.0 - outubro de 2018
#### <a name="azurermprofile"></a>AzureRM.Profile
* Corrigir o problema do Get-AzureRmSubscription no CloudShell
* Atualizar o código comum para utilizar a versão mais recente do ClientRuntime

#### <a name="azurermbackup"></a>AzureRM.Backup
* Cmdlets do Azure Backup preteridos.

#### <a name="azurermcompute"></a>AzureRM.Compute
* Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais as redes aceleradas vão ser ativadas quando a utilizar o simples conjunto de parâmetros para "New-AzureRmVm"
* Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.

#### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* Adicionar suporte para as Regras de Rede Virtual
    - Get-AzureRmDataLakeStoreVirtualNetworkRule: obtém ou listas a regra de rede virtual do Azure Data Lake Store.
    - Add-AzureRmDataLakeStoreVirtualNetworkRule: adiciona uma regra de rede virtual à conta especificada do Data Lake Store.
    - Set-AzureRmDataLakeStoreVirtualNetworkRule: modifica a regra especificada de rede virtual na conta do Data Lake Store.
    - Remove-AzureRmDataLakeStoreVirtualNetworkRule: elimina uma regra de rede virtual do Azure Data Lake Store.

#### <a name="azurermnetwork"></a>AzureRM.Network
* Atualizar o cmdlet Test-AzureRmNetworkWatcherConnectivity, passar o valor do protocolo para o back-end.
* Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.

#### <a name="azurermresources"></a>AzureRM.Resources
* Corrigir o problema em que Get-AzureRMRoleDefinition lança uma exceção ininteligível (quando o perfil predefinido não tem subscrição e não é especificado um âmbito) ao adicionar uma exceção significativa no cenário. Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".

## <a name="6100---october-2018"></a>6.10.0 - Outubro de 2018
#### <a name="azurestorage"></a>Azure.Storage
* Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados
    - Start-AzureStorageBlobCopy
    - Start-AzureStorageFileCopy

#### <a name="azurermcognitiveservices"></a>AzureRM.CognitiveServices
* Suporte para Get-AzureRmCognitiveServicesAccountSkus sem uma conta existente.

#### <a name="azurermcompute"></a>AzureRM.Compute
* Correção de Get-AzureRmVM -ResourceGroupName <rg> para devolver mais de 50 resultados, se necessário
* Adição de um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzureRmVmss.
* Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption

#### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* Atualização da versão do SDK .NET do ADF para a 2.3.0.

#### <a name="azurermnetwork"></a>AzureRM.Network
* Adição da funcionalidade NetworkProfile. novos cmdlets adicionados
    - Get-AzureRMNetworkProfile
    - New-AzureRMNetworkProfile
    - Remove-AzureRMNetworkProfile
    - Set-AzureRMNetworkProfile
    - New-AzureRMContainerNicConfig
    - New-AzureRmContainerNicConfigIpConfig
* Adição de uma ligação de associação do serviço no Modelo de Sub-rede
* Adição do cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap
* Adição do cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig

#### <a name="azurermrediscache"></a>AzureRM.RedisCache
* Permitir que qualquer cadeia como parâmetro Size permaneça. Adição de P5 no pop-up de PSArgumentCompleter

#### <a name="azurermresources"></a>AzureRM.Resources
* Adição do parâmetro -Mode em falta a Set-AzureRmPolicyDefinition
* Correção do erro de commandlet Get-AzureRmProviderOperation para as operações com uma Origem que contém o Utilizador

#### <a name="azurermsql"></a>AzureRM.Sql
* Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure

#### <a name="azurermstorage"></a>AzureRM.Storage
* Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.
    - Get-AzureRmStorageUsage

#### <a name="azurermwebsites"></a>AzureRM.Websites
* Novo Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor
* Novos Cmdlets New-AzureRMWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows

## <a name="690---september-2018"></a>6.9.0 - setembro de 2018
#### <a name="general"></a>Geral
* AzureRM.SignalR foi adicionado ao módulo de rollup AzureRM

#### <a name="azurermprofile"></a>AzureRM.Profile
* Alterações menores ao código comum do armazenamento
* Ficheiros de ajuda atualizados para incluírem todos os tipos de parâmetros.
* -ServicePrincipal alterado para non-mandatory no conjunto de parâmetros ServicePrincipalCertificateWithSubscriptionId 

#### <a name="azurestorage"></a>Azure.Storage
* Suporte para a criação de Contexto de Armazenamento com OAuth. 
    - New-AzureStorageContext

#### <a name="azurermcdn"></a>AzureRM.Cdn
* Standard_Microsoft adicionado ao sku de preços de Cdn. 

#### <a name="azurermcompute"></a>AzureRM.Compute
* Dependências no Cofre de Chaves e no Armazenamento movidas para as dependências comuns
* Adicionado suporte para mais tamanhos de máquinas virtuais para cmdlets do AEM
* Adicionado o parâmetro PublicIPPrefix a New-AzureRmVmssIpConfig
* Adicionado o parâmetro ResourceId ao cmdlet Invoke-AzureRmVMRunCommand
* Adicionado o cmdlet Invoke-AzureRmVmssVMRunCommand cmdlet

#### <a name="azurermdns"></a>AzureRM.Dns
* Suporte adicionado para registo de alias durante a criação de registo dns

#### <a name="azurerminsights"></a>AzureRM.Insights
* Corrigidos os problemas n.º 6833 e 7102 (Área Definições de Diagnóstico)
    - Problemas com o nome predefinido, ou seja, “serviço”, durante a criação e listagem/obtenção das definições de diagnóstico
    - Problemas ao criar definições de diagnóstico com categorias
* Adicionada mensagem de preterição aos parâmetros time grains das métricas
    - Os parâmetros timegrains ainda são aceites (esta não é uma alteração interruptiva), mas são ignorados no back-end, uma vez que apenas PT1M é válido

#### <a name="azurermnetwork"></a>AzureRM.Network
* Alterações aos cmdlets LoadBalancer
  - LoadBalancerInboundNatPoolConfig: parâmetros IdleTimeoutInMinutes, EnableFloatingIp e EnableTcpReset adicionados
  - LoadBalancerInboundNatRuleConfig: parâmetro EnableTcpReset adicionado
  - LoadBalancerRuleConfig: parâmetro EnableTcpReset adicionado
  - LoadBalancerProbeConfig: suporte para o valor "Https" para o parâmetro Protocol adicionado
* Adicionados comandos novos para o sub-recurso OutboundRule de LoadBalancer
  - Add-AzureRmLoadBalancerOutboundRuleConfig
  - Get-AzureRmLoadBalancerOutboundRuleConfig
  - New-AzureRmLoadBalancerOutboundRuleConfig
  - Set-AzureRmLoadBalancerOutboundRuleConfig
  - Remove-AzureRmLoadBalancerOutboundRuleConfig
* Adicionada propriedade HostedWorkloads nova para PSNetworkInterface
* Adicionados cmdlets novos para a funcionalidade: Azure Firewall através de ARM
  - Get-AzureRmFirewall adicionado
  - Set-AzureRmFirewall adicionado
  - New-AzureRmFirewall adicionado
  - Remove-AzureRmFirewall adicionado
  - New-AzureRmFirewallApplicationRuleCollection adicionado
  - New-AzureRmFirewallApplicationRule adicionado
  - New-AzureRmFirewallNatRuleCollection adicionado
  - New-AzureRmFirewallNatRule adicionado
  - New-AzureRmFirewallNetworkRuleCollection adicionado
  - New-AzureRmFirewallNetworkRule adicionado
* Adicionado suporte para o certificado de raiz fidedigna e configuração de dimensionamento automático no Gateway de Aplicação
  - Novos cmdlets adicionados:
      - Add-AzureRmApplicationGatewayTrustedRootCertificate
      - Get-AzureRmApplicationGatewayTrustedRootCertificate
      - New-AzureRmApplicationGatewayTrustedRootCertificate
      - Remove-AzureRmApplicationGatewayTrustedRootCertificate
      - Set-AzureRmApplicationGatewayTrustedRootCertificate
      - Get-AzureRmApplicationGatewayAutoscaleConfiguration
      - New-AzureRmApplicationGatewayAutoscaleConfiguration
      - Remove-AzureRmApplicationGatewayAutoscaleConfiguration
      - Set-AzureRmApplicationGatewayAutoscaleConfiguration
  - Cmdlets updated with optonal parameter -TrustedRootCertificate
      - New-AzureRmApplicationGateway
      - Set-AzureRmApplicationGateway
      - New-AzureRmApplicationGatewayBackendHttpSetting
      - Set-AzureRmApplicationGatewayBackendHttpSetting
  - Cmdlets atualizados com parâmetro opcional -AutoscaleConfiguration
      - New-AzureRmApplicationGateway
      - Set-AzureRmApplicationGateway
* Adicionado cmdlet para Ponto Final da Interface Get-AzureInterfaceEndpoint
* Adicionado suporte para vários prefixos de endereços numa sub-rede. cmdlets atualizados:
  - New-AzureRmVirtualNetworkSubnetConfig
  - Set-AzureRmVirtualNetworkSubnetConfig
  - Add-AzureRmVirtualNetworkSubnetConfig
  - Get-AzureRmVirtualNetworkSubnetConfig
  - Add-AzureRmApplicationGatewayAuthenticationCertificate
  - Add-AzureRmApplicationGatewayFrontendIPConfig
  - New-AzureRmApplicationGatewayFrontendIPConfig
  - Set-AzureRmApplicationGatewayFrontendIPConfig
  - Add-AzureRmApplicationGatewayIPConfiguration
  - New-AzureRmApplicationGatewayIPConfiguration
  - Set-AzureRmApplicationGatewayIPConfiguration
  - Add-AzureRmNetworkInterfaceIpConfig
  - New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig
  - New-AzureRmVirtualNetworkGatewayIpConfig
  - Add-AzureRmVirtualNetworkGatewayIpConfig
  - Set-AzureRmLoadBalancerFrontendIpConfig
  - Add-AzureRmLoadBalancerFrontendIpConfig
  - New-AzureRmLoadBalancerFrontendIpConfig
  - New-AzureRmNetworkInterface
* Adição de cmdlets para delegação de sub-rede
  - New-AzureRmDelegation: cria uma delegação nova, que pode ser adicionada a uma sub-rede
  - Remove-AzureRmDelegation: recebe uma sub-rede e remove o nome da delegação especificado dessa sub-rede
  - Add-AzureRmDelegation: recebe uma sub-rede e adiciona o nome de serviço especificado como delegação a essa sub-rede
  - Get-AzureRmDelegation
  - Get-AzureRmAvailableServiceDelegations

#### <a name="azurermrecoveryservicessiterecovery"></a>AzureRM.RecoveryServices.SiteRecovery
* Suporte para discos geridos

#### <a name="azurermrediscache"></a>AzureRM.RedisCache
* Dependência de informações atualizada

#### <a name="azurermresources"></a>AzureRM.Resources
* New-AzureRmResourceGroupDeployment atualizado com parâmetro novo RollbackAction
    - Adicionado suporte para OnErrorDeployment com o parâmetro novo.
* Suporte para identidades geridas nas atribuições de políticas.
* Os parâmetros com valores predefinidos já não são necessários ao atribuir uma política com “New-AzureRmPolicyAssignment”
* Adicionado cmdlet novo Get-AzureRmPolicyAlias para obter aliases de políticas

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* Problema n.º 7161 corrigido

#### <a name="azurermsignalr"></a>AzureRM.SignalR
* Nomes dos SKUs atualizados para Free_F1 e Standard_S1
* Adicionado campo de versão ao objeto PSSignalRResource e cadeia de ligação ao objeto PSSignalRKeys.

#### <a name="azurermstorage"></a>AzureRM.Storage
* Suporte para política Imutabilidade em AzureRm.Storage 
    - Remove-AzureRmStorageAccountNetworkRule
    - Get-AzureRmStorageContainer
    - Update-AzureRmStorageContainer
    - New-AzureRmStorageContainer
    - Remove-AzureRmStorageContainer
    - Add-AzureRmStorageContainerLegalHold
    - Remove-AzureRmStorageContainerLegalHold
    - Set-AzureRmStorageContainerImmutabilityPolicy
    - Get-AzureRmStorageContainerImmutabilityPolicy
    - Remove-AzureRmStorageContainerImmutabilityPolicy
    - Lock-AzureRmStorageContainerImmutabilityPolicy

#### <a name="azurermwebsites"></a>AzureRM.Websites
* Adicionados dois cmdlets novos: Get-AzureRmDeletedWebApp e Restore-AzureRmDeletedWebApp
* O comutador New-AzureRmAppServicePlan -HyperV é adicionado para criar o plano do serviço de aplicações com contentor do Windows
* New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - parâmetros novos (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) adicionados para criar e gerir a aplicação de contentor do Windows

## <a name="681---august-2018"></a>6.8.1 - Agosto de 2018
#### <a name="general"></a>Geral
* Foi corrigido o problema com os grupos de recursos predefinidos não definidos.
* Assemblagens de runtime comum atualizadas

#### <a name="azurermapimanagement"></a>AzureRM.ApiManagement
* Foi corrigido o problema com os grupos de recursos predefinidos não definidos.
* Problema https://github.com/Azure/azure-powershell/issues/6603 corrigido
    - Agora, os cmdlets Import-AzureRmApiManagementApi e *-AzureRmApiManagementCertificate identificam caminhos relativos
* Problema https://github.com/Azure/azure-powershell/issues/6879 corrigido
    - O CertificateInformation é uma propriedade definível que permite que o cmdlet Set-AzureRmApiManagement funcione corretamente. Corrigido com a atualização para 4.0.4-nuget de pré-visualização
* Problema https://github.com/Azure/azure-powershell/issues/6853 corrigido
    - Foi corrigido o filtro de Odata para procurar por nome de produto
* Problema https://github.com/Azure/azure-powershell/issues/6814 corrigido
    - Foi corrigido o filtro de Odata para procurar por nome na API
* Foi adicionado suporte para o logger de AzureMonitor


#### <a name="azurermcompute"></a>AzureRM.Compute
* Foi corrigido o problema em que o destino está em falta no resultado da saída.
* Foi corrigido o problema com o tipo de conta de armazenamento para a VM com disco gerido
* Foi corrigido o problema com os grupos de recursos predefinidos não definidos.
* Corrigir os cmdlets do AEM Extension para outros ambientes, por exemplo o Azure China

#### <a name="azurermnetwork"></a>AzureRM.Network
* Representação de saída de cmdlet predefinidos alterada para a vista de tabela

#### <a name="azurermpowerbiembedded"></a>AzureRM.PowerBIEmbedded
* Corrigida a falha em Update-AzureRmPowerBIEmbeddedCapacity ao tentar dimensionar a capacidade em pausa


#### <a name="azurermresources"></a>AzureRM.Resources
* Corrigido o erro ao criar a aplicações geridas a partir do Marketplace.

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* Problemas corrigidos
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a>AzureRM.TrafficManager
* Suporte adicionado para o método de encaminhamento de MultiValue
    - Novo parâmetro "MaxReturn" para encaminhamento MultiValue
* Suporte adicionado para o método de encaminhamento de Sub-rede
    - Suporte para intervalos de endereços IP (sub-redes) em pontos finais
* Suporte adicionado para Cabeçalhos Personalizados nos perfis
* Suporte adicionado para intervalos de código esperados nos perfis
* Suporte adicionado para Cabeçalhos Personalizados nos pontos finais

## <a name="680---august-2018"></a>6.8.0 - Agosto 2018
#### <a name="general"></a>Geral
* Foi corrigido o problema com os grupos de recursos predefinidos não definidos.

#### <a name="azurermprofile"></a>AzureRM.Profile
* Foi adicionada a propriedade de expiração aos tokens devolvidos durante o Connect-AzureRmAccount

#### <a name="azurermcompute"></a>AzureRM.Compute
* Foi corrigido o problema em que o destino está em falta no resultado da saída.
* Foi corrigido o problema com o tipo de conta de armazenamento para a VM com disco gerido
* Corrigir os cmdlets do AEM Extension para outros ambientes, por exemplo o Azure China

#### <a name="azurermiothub"></a>AzureRM.IotHub
* Corrigir exemplos para New-AzureRmIotHubExportDevices e New-AzureRmIotHubImportDevices

#### <a name="azurermnetwork"></a>AzureRM.Network
* Representação de modelos predefinidos alterada para a vista de tabela

#### <a name="azurermpowerbiembedded"></a>AzureRM.PowerBIEmbedded
* Corrigida a falha em Update-AzureRmPowerBIEmbeddedCapacity ao tentar dimensionar a capacidade em pausa

#### <a name="azurermresources"></a>AzureRM.Resources
* Corrigido o erro ao criar a aplicação gerida a partir do Marketplace.

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* Correção para problemas
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a>AzureRM.TrafficManager
* Suporte para o método de encaminhamento de MultiValue
    - Novo parâmetro "MaxReturn" para encaminhamento MultiValue
* Suporte para o método de encaminhamento de Sub-rede
    - Suporte para intervalos de endereços IP (sub-redes) em pontos finais
* Suporte para Cabeçalhos Personalizados nos perfis
* Suporte para Intervalos de código esperados nos perfis
* Suporte para Cabeçalhos Personalizados nos pontos finais

#### <a name="azurermwebsites"></a>AzureRM.Websites
* Foi corrigido o problema com os grupos de recursos predefinidos incorretamente.

## <a name="670---august-2018"></a>6.7.0 - Agosto 2018
#### <a name="azurermprofile"></a>AzureRM.Profile
* Atualizado para a versão mais recente do Azure ClientRuntime.
* Adicionado ID de utilizador ao nome de contexto predefinido para evitar conflito de contextos
    - https://github.com/Azure/azure-powershell/issues/6489
* Corrigidos os problemas com Clear-AzureRmContext que causavam problemas com a seleção de um contexto #6398
* Permissão para o domínio de inquilino passar para o parâmetro "-TenantId" para "Connect-AzureRmAccount"
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a>Azure.Storage
* Remoção da limitação de 5 TB da quota da Partilha de Ficheiros do Azure
* Set-AzureStorageShareQuota

#### <a name="azurermanalysisservices"></a>AzureRM.AnalysisServices
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azureanalysisservices"></a>Azure.AnalysisServices
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermapimanagement"></a>AzureRM.ApiManagement
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermapplicationinsights"></a>AzureRM.ApplicationInsights
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermautomation"></a>AzureRM.Automation
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermbackup"></a>AzureRM.Backup
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermbatch"></a>AzureRM.Batch
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermbilling"></a>AzureRM.Billing
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermcdn"></a>AzureRM.Cdn
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermcognitiveservices"></a>AzureRM.CognitiveServices
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermcompute"></a>AzureRM.Compute
* Atualizado para a versão mais recente do Azure ClientRuntime.
* Adicionado o parâmetro EvictionPolicy a New-AzureRmVmssConfig
* Utilização da localização predefinida em DiskFileParameterSet de New-AzureRmVm se não for especificada nenhuma Localização.
* Correção da descrição do parâmetro em Save-AzureRmVMImage
* Correção do cmdlet Get-AzureRmVMDiskEncryptionStatus para determinados cenários relacionados com passagem única

#### <a name="azurermconsumption"></a>AzureRM.Consumption
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermcontainerinstance"></a>AzureRM.ContainerInstance
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermcontainerregistry"></a>AzureRM.ContainerRegistry
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermdatafactories"></a>AzureRM.DataFactories
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermdatalakeanalytics"></a>AzureRM.DataLakeAnalytics
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* Correção da depuração quando DebugPreference é definida a partir da linha de comando do powershell
* Exemplo atualizado para Set-AzureRmDataLakeStoreItemAcl
* Atualizado para a versão mais recente do Azure ClientRuntime.
* Exemplo atualizado para Set-AzureRmDataLakeStoreItemAclEntry

#### <a name="azurermdevtestlabs"></a>AzureRM.DevTestLabs
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermdns"></a>AzureRM.Dns
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermeventgrid"></a>AzureRM.EventGrid
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermeventhub"></a>AzureRM.EventHub
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermhdinsight"></a>AzureRM.HDInsight
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurerminsights"></a>AzureRM.Insights
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermiothub"></a>AzureRM.IotHub
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermlogicapp"></a>AzureRM.LogicApp
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermmachinelearning"></a>AzureRM.MachineLearning
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermmachinelearningcompute"></a>AzureRM.MachineLearningCompute
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermmarketplaceordering"></a>AzureRM.MarketplaceOrdering
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermmedia"></a>AzureRM.Media
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermnetwork"></a>AzureRM.Network
* Exemplo adicionado para Set-AzureRmLocalNetworkGateway
* Exemplos e descrições atualizados para Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey e New-AzureRmVirtualNetworkGatewayConnection
* Exemplos adicionados para Remove-AzureRmVirtualNetworkGatewayIpConfig e Reset-AzureRmVirtualNetworkGateway
* Exemplo adicionado para Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey
* Exemplo adicionado para Set-AzureRmVirtualNetworkGatewayConnectionSharedKey
* Exemplo adicionado para Set-AzureRmVirtualNetworkGatewayConnection
* Cmdlets gerados novamente para ApplicationSecurityGroup, RouteTable e Usage com o gerador de códigos mais recente
* Esclarecida a mensagem de erro para Get-AzureRmVirtualNetworkSubnetConfig ao tentar obter uma sub-rede que não existe

#### <a name="azurermnotificationhubs"></a>AzureRM.NotificationHubs
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermoperationalinsights"></a>AzureRM.OperationalInsights
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermpolicyinsights"></a>AzureRM.PolicyInsights
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermpowerbiembedded"></a>AzureRM.PowerBIEmbedded
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermrecoveryservices"></a>AzureRM.RecoveryServices
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermrecoveryservicesbackup"></a>AzureRM.RecoveryServices.Backup
* Adicionado filtro de política ao cmdlet Get-AzureRmRecoveryServicesBackItem. O comando devolve a lista de itens de cópia de segurança protegidos pelo ID de política especificado.
* Atualizado Microsoft.Azure.Management.RecoveryServices.Backup para a versão 3.0.0-preview.
* Atualizado para a versão mais recente do Azure ClientRuntime.
* Adicionado o parâmetro TargetResourceGroupName a Restore-AzureRmRecoveryServicesBackupItem. O grupo de recursos para o qual os discos geridos são restaurados. Aplicável à cópia de segurança de VM com discos geridos.

#### <a name="azurermrecoveryservicessiterecovery"></a>AzureRM.RecoveryServices.SiteRecovery
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermrediscache"></a>AzureRM.RedisCache
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermrelay"></a>AzureRM.Relay
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermresources"></a>AzureRM.Resources
* Suporte para a implementação do modelo no âmbito da subscrição. Adicionados novos Cmdlets:
    - New-AzureRmDeployment
    - Get-AzureRmDeployment
    - Test-AzureRmDeployment
    - Remove-AzureRmDeployment
    - Stop-AzureRmDeployment
    - Save-AzureRmDeploymentTemplate
    - Get-AzureRmDeploymentOperation
* Corrigido o problema em que é apresentado um erro ao passar um contexto para Set-AzureRmResource
    - https://github.com/Azure/azure-powershell/issues/5705
* Corrigido o exemplo em New-AzureRmResourceGroupDeployment
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermscheduler"></a>AzureRM.Scheduler
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermsql"></a>AzureRM.Sql
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermstorage"></a>AzureRM.Storage
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermstreamanalytics"></a>AzureRM.StreamAnalytics
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermtags"></a>AzureRM.Tags
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermtrafficmanager"></a>AzureRM.TrafficManager
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermusageaggregates"></a>AzureRM.UsageAggregates
* Atualizado para a versão mais recente do Azure ClientRuntime.

#### <a name="azurermwebsites"></a>AzureRM.Websites
* Atualizado para a versão mais recente do Azure ClientRuntime.

## <a name="660---july-2018"></a>6.6.0 - Julho de 2018
#### <a name="general"></a>Geral
* Foram atualizados todos os ficheiros de ajuda para incluir tipos de parâmetros inteiros e tipos de entrada/saída corretos.

#### <a name="azurermprofile"></a>AzureRM.Profile
* A biblioteca Common.Strategy foi atualizada para poder validar que a configuração atual de um recurso é compatível com o recurso de destino.
* Foi adicionado ps1xml a Common.Storage

#### <a name="azurestorage"></a>Azure.Storage
* Adicionado suporte para obter o Contexto de Armazenamento de DefaultProfile
* Adicionado Ps1XmlAttribute a propriedades de tipos de saídas de cmdlets.

#### <a name="azurermapimanagement"></a>AzureRM.ApiManagement
* Problema https://github.com/Azure/azure-powershell/issues/6370 corrigido
    - Foi corrigido um erro no Automapper para traduzir PsApiManagementApi para ApiContract
* Problema https://github.com/Azure/azure-powershell/issues/6515 corrigido
    - Foi corrigido um erro em File.Save para não sobrecarregar com Tipo de Codificação
* Problema https://github.com/Azure/azure-powershell/issues/6560 corrigido
    - Atualizado para a versão 4.0.3 do Nuget, que corrige a exceção de padrão em apiId

#### <a name="azurermcompute"></a>AzureRM.Compute
* Corrigido problema com a falha na criação de uma vm com DiskFileParameterSet em New-AzureRmVm devido a mudança de nome do tipo de conta de armazenamento PremiumLRS.
* Foi corrigido o cmdlet Invoke-AzureRmVMRunCommand
* Foi atualizado Get-AzureRmAvailabilitySet para permitir a listagem de todos os conjuntos de disponibilidade numa subscrição.  (O parâmetro ResouceGroupName é agora opcional.)
* Atualização de SimpleParameterSet de “New-AzureRmVm” para permitir a Rede Acelerada em vms elegíveis.
* Atualização do conjunto de parâmetros simples New-AzureRmVmss para falhar a criação de vms quando um LB especificado por um utilizador já existir.
* Atualização de exemplo para New-AzureRmDisk
* Adição de exemplo para “New-AzureRmVM”
* Atualização da descrição para Set-AzureRmVMOSDisk
* Atualização do Exemplo 1 para Set-AzureRmVMBginfoExtension para corrigir a ortografia e o prefixo. 

#### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* Atualização da versão do SDK .NET do ADF para a 1.1.0.
* Suporte para partilha de runtime de integração autoalojado em várias fábricas de dados
     - Adicionado parâmetro novo -SharedIntegrationRuntimeResourceId ao cmdlet Set-AzureRmDataFactoryV2IntegrationRuntime.
     - Adicionado o parâmetro opcional novo -LinkedDataFactoryName ao cmdlet Remove-AzureRmDataFactoryV2IntegrationRuntime.

#### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* Atualizada a versão do SDK DataPlane (Microsoft.Azure.DataLake.Store) para a 1.1.9

#### <a name="azurermeventhub"></a>AzureRM.EventHub
* Atualização de piping para InputObject e ResourceId em cmdlets de remoção

#### <a name="azurerminsights"></a>AzureRM.Insights
* Correção da formatação de OutputType nos ficheiros de ajuda
* Utilização da pré-visualização do SDK Microsoft.Azure.Management.Monitor SDK 0.19.1

#### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Correção de problema em Set-AzureRmKeyVaultAccessPolicy

#### <a name="azurermnetwork"></a>AzureRM.Network
* Adicionados exemplos para os cmdlets LoadBalancerInboundNatPoolConfig.

#### <a name="azurermresources"></a>AzureRM.Resources
* Corrigido problema ao fornecer o nome e o valor da etiqueta para “Get-AzureRmResource”
    - https://github.com/Azure/azure-powershell/issues/6765
* Correção de cenário de piping com “Set-AzureRmResource”

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* Atualização de piping para InputObject e ResourceId em cmdlets de remoção
* corrigidos problemas novos
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a>AzureRM.Sql
* Adição de suporte para Proteção Avançada contra Ameaças do Servidor com os seguintes cmdlets:
    - Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy
* Adição de suporte para Avaliação de Vulnerabilidades com os seguintes cmdlets:
    - Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings
    - Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline
    - Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan
* Corrigido exemplo em Remove-AzureRmSqlServerFirewallRule
* Corrigido processamento incorreto de datetime para culturas base diferentes de eua em Get-AzureSqlSyncGroupLog

#### <a name="azurermstorage"></a>AzureRM.Storage
* Adição de Ps1XmlAttribute para propriedades de tipos de saídas de cmdlets
* Mostrar saída de cmdlet StorageAccount na vista de tabela
    - Get-AzureRmStorageAccount
    - New-AzureRmStorageAccount
    - Set-AzureRmStorageAccount

#### <a name="azurermtags"></a>AzureRM.Tags
* Remoção de declaração incorreta da ajuda do cmdlet Tag
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a>6.5.0 - Julho de 2018
#### <a name="azurermprofile"></a>AzureRM.Profile
* Ajuda atualizada para "Get-AzureRmContextAutosaveSetting"

#### <a name="azurestorage"></a>Azure.Storage
* Suporte de Carregamento de Blob ou Ficheiro com token Sas apenas de escrita
* Set-AzureStorageBlobContent
* Set-AzureStorageFileContent

#### <a name="azurermanalysisservices"></a>AzureRM.AnalysisServices
* Adicionar propriedade ResourceGroupName obrigatória ao AS.

#### <a name="azurermautomation"></a>AzureRM.Automation
* Atualizar ajuda e adicionar exemplo a "New-AzureRMAutomationSchedule"

#### <a name="azurermcompute"></a>AzureRM.Compute
* Adicionar parâmetro -Tag a Update/New-AzureRmAvailabilitySet
* Adicionar exemplo a "Add-AzureRmVmssExtension"
* Adicionar exemplos a "Remove-AzureRmVmssExtension"
* Atualizar ajuda para "Set-AzureRmVMAccessExtension"
* Atualizar SimpleParameterSet para New-AzureRmVmss para definir SinglePlacementGroup como falso por predefinição e adicionar parâmetro do comutador "SinglePlacementGroup" que permite ao utilizador criar a VMSS num único grupo de posicionamento.

#### <a name="azurermeventhub"></a>AzureRM.EventHub
* Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSEventHubDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso

#### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Atualizar mensagem de erro para Set-AzureRmKeyVaultAccessPolicy

#### <a name="azurermlogicapp"></a>AzureRM.LogicApp
* Erro "a definição do parâmetro não foi resolvida" corrigido no New-AzureRmLogicApp

#### <a name="azurermnetwork"></a>AzureRM.Network
* Ativar peering entre várias Redes Virtuais em vários Inquilinos para Set/Add-AzureRmVirtualNetworkPeering
* Cmdlets abaixo atualizados para Gateway de Aplicação
    - New-AzureRmApplicationGateway: Sinalizador EnableFIPS e suporte de Zonas adicionados
    - New-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados
    - Set-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados
* Cmdlets RouteTable regenerados com a versão do gerador mais recente

#### <a name="azurermrelay"></a>AzureRM.Relay
* Ficheiros de marcação atualizados, correção para o problema do nome do parâmetro no exemplo

#### <a name="azurermresources"></a>AzureRM.Resources
* Cmdlets Roleassignment e roledefinition atualizados:
    - Remover chamadas de roledefinition extra feitas como parte da paginação.
* Corrigir cmdlet Get-AzureRmRoleAssignment
    - Corrigir funcionalidade do parâmetro do comando -ExpandPrincipalGroups
* Corrigir problema com "Get-AzureRmResource" em que o parâmetro "-ResourceType" era sensível a maiúsculas e minúsculas

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* Parâmetro top e skip adicionados para listar os cmdlets
* Cmdlets de migração do Espaço de Nomes Standard a Premium:
    - Start-AzureRmServiceBusMigration
    - Get-AzureRmServiceBusMigration
    - Complete-AzureRmServiceBusMigration
    - Stop-AzureRmServiceBusMigration
    - Remove-AzureRmServiceBusMigration
* Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSServiceBusDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso

#### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* Exemplo de atualização para "New-AzureRmServiceFabricCluster"

#### <a name="azurermsql"></a>AzureRM.Sql
* Adicionar novos Cmdlets ao Management.Sql para permitir aos clientes adicionarem o Certificado TDE à instância do Sql Server ou uma Instância Gerida
    - Add-AzureRmSqlServerTransparentDataEncryptionCertificate
    - Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate

#### <a name="azurermwebsites"></a>AzureRM.Websites
* `Set-AzureRmWebApp -AssignIdentity` e  `Set-AzureRmWebAppSlot -AssignIdentity` quando definidos como falso também irão agora remover a propriedade de Identidade da etiqueta de pré-visualização object.Removing do site.
* `Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` exemplo atualizado
* `Set-AzureRmWebApp -PhpVersion` suporta como uma versão válida do PHP

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
* Apresentação de novos SKUs para VirtualNetworkGateways com redundância entre zonas
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
