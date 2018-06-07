---
title: Registo de alterações do Azure PowerShell | Microsoft Docs
description: Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente.
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 07/26/2017
ms.openlocfilehash: 9237fe7ec75fd796a79714b6e098fa5546537cad
ms.sourcegitcommit: 2eea03b7ac19ad6d7c8097743d33c7ddb9c4df77
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/06/2018
ms.locfileid: "34821994"
---
# <a name="release-notes"></a>Notas de versão

Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.

## <a name="20170925---version-440"></a>25-09-2017 - Versão 4.4.0
* AnalysisServices
  * Foi adicionado um novo commandlet de plano de dados para permitir a sincronização de bases de dados, de instância de leitura/escrita para instâncias só de leitura
    - Foi incluído um ficheiro de ajuda para o commandlet
    - Foram adicionados testes dentro da memória e um cenário de teste (apenas em direto)
  * Foram corrigidos erros no commandlet Add-AzureAsAccount
* Automatização
  * Foram corrigidos documentos de ajuda para cmdlets corrigidos na versão anterior.
  * Foram adicionados 4 novos cmdlets para suportar a implementação faseada de configurações de nós DSC.
    - Start-AzureRmAutomationDscNodeConfigurationDeployment
    - Stop-AzureRmAutomationDscNodeConfigurationDeployment
    - Get-AzureRmAutomationDscNodeConfigurationDeployment
    - Get-AzureRmAutomationDscNodeConfigurationDeploymentSchedule
* CognitiveServices
  * Integração na versão 2.0.0 do SDK de Gestão dos Serviços Cognitivos.
  * Get-AzureRmCognitiveServicesAccount pode agora suportar corretamente a paginação.
* Computação
  * Funcionalidade Executar Comando:
    - Novo cmdlet: “Invoke-AzureRmVMRunCommand” invoca uma execução de comando numa VM
    - Novo cmdlet: “Get-AzureRmVMRunCommandDocument” mostra os documentos para a execução de comando disponíveis
  * Adição do parâmetro “StorageAccountType” a Set-AzureRmDataDisk
  * Suporte de Zona de Disponibilidade para a máquina virtual, o conjunto de dimensionamento de VMs e o disco
    - Novo parâmetro: “Zone” foi adicionado a New-AzureRmVM, New-AzureRmVMConfig, New-AzureRmVmssConfig, New-AzureRmDiskConfig
  * Funcionalidade de atualização sem interrupção do conjunto de dimensionamento de VMs:
    - Novo cmdlet: “Start-AzureRmVmssRollingOSUpgrade” invoca a atualização sem interrupção do SO do conjunto de dimensionamento de VMs
    - Novo cmdlet: “Set-AzureRmVmssRollingUpgradePolicy” define a política de atualização para a atualização sem interrupção do conjunto de dimensionamento de VMs.
    - Novo cmdlet: “Stop-AzureRmVmssRollingUpgrade” cancela a atualização sem interrupção do conjunto de dimensionamento de VMs
    - Novo cmdlet: “Get-AzureRmVmssRollingUpgrade” mostra o estado da atualização sem interrupção do conjunto de dimensionamento de VMs.
  * O parâmetro opcional AssignIdentity foi introduzido, para a identidade atribuída pelo sistema.
    - Novo parâmetro: “AssignIdentity” foi adicionado a New-AzureRmVMConfig, New-AzureRmVmssConfig e Update-AzureRmVM
  * Funcionalidade de encriptação de disco Vmss:
    - Novo cmdlet: “Set-AzureRmVmssDiskEncryptionExtension” ativa a encriptação de disco no conjunto de dimensionamento de VMs
    - Novo cmdlet: “Disable-AzureRmVmssDiskEncryption” desativa a encriptação de disco no conjunto de dimensionamento de VMs
    - Novo cmdlet: “Get-AzureRmVmssDiskEncryptionStatus” mostra o estado de encriptação de disco de um conjunto de dimensionamento de VMs
    - Novo cmdlet: “Get-AzureRmVmssVMDiskEncryptionStatus” mostra o estado de encriptação de disco de VMs num conjunto de dimensionamento de VMs
* ContainerInstance
  * Adição de cmdlets do PowerShell para Instância do Azure Container
    - New-AzureRmContainerGroup
    - Get-AzureRmContainerGroup
    - Remove-AzureRmContainerGroup
    - Get-AzureRmContainerInstanceLog
* Informações
  * Novo cmdlet Disable-AzureRmActivityLogAlert
    - Um novo cmdlet para desativar um alerta existente de registo de atividades.
    - Opcionalmente, as Etiquetas também são definíveis com este cmdlet.
  * Novo cmdlet Enable-AzureRmActivityLogAlert
    - Um novo cmdlet para ativar um alerta existente de registo de atividades.
    - Opcionalmente, as Etiquetas também são definíveis com este cmdlet.
  * Novo cmdlet Get-AzureRmActivityLogAlert
    - Um novo cmdlet para obter um ou mais alertas de registo de atividades.
    - Os alertas podem ser obtidos por nome, grupo de recursos ou subscrição.
  * Novo cmdlet New-AzureRmActionGroup
    - Um novo cmdlet para criar um objeto de ActionGroup na memória (nenhum pedido envolvido.)
  * Novo cmdlet New-AzureRmActivityLogAlertCondition
    - Um novo cmdlet para criar uma condição de folha de alerta de registo de atividades na memória (nenhum pedido envolvido.)
  * Novo cmdlet Set-AzureRmActivityLogAlert
    - Um novo cmdlet para criar ou atualizar um alerta de registo de atividades.
  * Novo cmdlet Remove-AzureRmActivityLogAlert
    - Um novo cmdlet para remover um alerta de registo de atividades.
  * Novo cmdlet Set-AzureRmActionGroup
    - Um novo cmdlet para criar um novo grupo de ação ou atualizar um existente.
  * Novo cmdlet Get-AzureRmActionGroup
    - Um novo cmdlet para obter um ou mais grupos de ação.
    - Os grupos de ação podem ser obtidos por nome, grupo de recursos ou subscrição.
  * Novo cmdlet Remove-AzureRmActionGroup
    - Um novo cmdlet para remover um grupo de ação.
  * Novo cmdlet New-AzureRmActionGroupReceiver
    - Um novo cmdlet para criar um novo recetor de grupo de ação na memória.
* KeyVault
  * Cmdlets novos/atualizados para suportar a eliminação de forma recuperável de certificados KeyVault
    * Get-AzureKeyVaultCertificate
    * Remove-AzureKeyVaultCertificate
    * Undo-AzureKeyVaultCertificateRemoval
* Rede
  * Foi adicionado suporte para serviços de ponto final para Sub-redes de Rede Virtual
    - Add-AzureRmVirtualSubnetConfig foi atualizado: foi adicionado o parâmetro opcional -ServiceEndpoint
    - New-AzureRmVirtualSubnetConfig foi atualizado: foi adicionado o parâmetro opcional -ServiceEndpoint
    - Set-AzureRmVirtualSubnetConfig foi atualizado: foi adicionado o parâmetro opcional -ServiceEndpoint
  * Foi adicionado um cmdlet para listar os serviços de ponto final disponíveis na localização
    - Get-AzureRmVirtualNetworkAvailableEndpointService
  * Foi adicionada a capacidade de configurar autenticação P2S baseada em radius externo aos seguintes commandlets
    - New-AzureVirtualNetworkGateway
    - Set-AzureVirtualNetworkGateway
    - Set-AzureRmVirtualNetworkGatewayVpnClientConfig
  * Foi adicionado um cmdlet para permitir gerar VpnProfiles para P2S baseado em radius externo
    - New-AzureRmVpnClientConfiguration
    - Get-AzureRmVpnClientConfiguration
  * Foi adicionado suporte para o parâmetro SKU, para Endereços IP Públicos e Balanceadores de Carga
    - New-AzureRMLoadBalancer foi atualizado: foi adicionado um parâmetro opcional -Sku
    - New-AzureRMPublicIpAddress foi atualizado: foi adicionado um parâmetro opcional -Sku
  * Foi adicionado suporte para DisableOutboundSNAT, para as Regras de Balanceador de Carga
    - New-AzureRMLoadBalancerRuleConfig foi atualizado: foi adicionado o parâmetro opcional DisableOutboundSNAT
    - Add-AzureRMLoadBalancerRuleConfig foi atualizado: foi adicionado o parâmetro opcional DisableOutboundSNAT
    - Set-AzureRMLoadBalancerRuleConfig foi atualizado: foi adicionado o parâmetro opcional DisableOutboundSNAT
  * Foi adicionado suporte para P2S IKEv2
    - New-AzureRmVirtualNetworkGateway foi atualizado: foi adicionado um parâmetro opcional -VpnClientProtocol, assume a predefinição [ “SSTP”, “IkeV2” ]
    - Set-AzureRmVirtualNetworkGateway foi atualizado: foi adicionado um parâmetro opcional -VpnClientProtocol
  * Foi adicionado suporte para regras MultiValued nas Regras de Segurança de Rede e Regras Eficazes de Segurança de Rede
    - Add-AzureRmNetworkSecurityRuleConfig foi atualizado: os parâmetros SourcePortRange, DestinationPortRange, SourceAddressPrefix foram atualizados para aceitarem uma lista de cadeias
    - New-AzureRmNetworkSecurityRuleConfig foi atualizado: os parâmetros SourcePortRange, DestinationPortRange, SourceAddressPrefix foram atualizados para aceitarem uma lista de cadeias
    - Set-AzureRmNetworkSecurityRuleConfig foi atualizado: os parâmetros SourcePortRange, DestinationPortRange, SourceAddressPrefix foram atualizados para aceitarem uma lista de cadeias
    - Add-AzureRmNetworkSecurityRuleConfig foi atualizado: os parâmetros SourcePortRange, DestinationPortRange, SourceAddressPrefix foram atualizados para aceitarem uma lista de cadeias
    - New-AzureRmNetworkSecurityGroup foi atualizado: o parâmetro SecurityRules foi atualizado para aceitar os parâmetros SourcePortRange, DestinationPortRange, SourceAddressPrefix, que são lista de cadeias no objeto PSSecurityRule
    - Get-AzureRmEffectiveNetworkSecurityGroup foi atualizado: o parâmetro TagMap foi adicionado
    - Get-AzureRmEffectiveNetworkSecurityGroup foi atualizado: o objeto PSEffectiveSecurityRule devolvido foi atualizado com os parâmetros SourcePortRange, DestinationPortRange, SourceAddressPrefix, que são lista de cadeias.
  * Foi adicionado suporte para proteção contra DDoS de redes virtuais
    - New-AzureRmVirtualNetwork foi atualizado: os parâmetros opcionais EnableDDoSProtection e EnableVmProtection foram adicionados
    - Foram adicionadas as propriedades EnableDDoSProtection e EnableVmProtection no objeto PSVirtualNetwork
  * Foi adicionado suporte para Balanceador de Carga Interno de Elevada Disponibilidade
    - Add-AzureRmLoadBalancerRuleConfig foi atualizado: Tudo foi adicionado como um valor aceitável para o parâmetro Protocol
    - New-AzureRmLoadBalancerRuleConfig foi atualizado: Tudo foi adicionado como um valor aceitável para o parâmetro Protocol
    - Set-AzureRmLoadBalancerRuleConfig foi atualizado: Tudo foi adicionado como um valor aceitável para o parâmetro Protocol
  * Foi adicionado suporte para os Grupos de Segurança de Aplicações
    - New-AzureRmApplicationSecurityGroup foi adicionado
    - Get-AzureRmApplicationSecurityGroup foi adicionado
    - Remove-AzureRmApplicationSecurityGroup foi adicionado
    - New-AzureRmNetworkInterface foi atualizado: os parâmetros opcionais ApplicationSecurityGroup e ApplicationSecurityGroupId foram adicionados
    - New-AzureRmNetworkInterfaceIpConfig foi atualizado: os parâmetros opcionais ApplicationSecurityGroup e ApplicationSecurityGroupId foram adicionados
    - Add-AzureRmNetworkInterfaceIpConfig foi atualizado: os parâmetros opcionais ApplicationSecurityGroup e ApplicationSecurityGroupId foram adicionados
    - Set-AzureRmNetworkInterfaceIpConfig foi atualizado: os parâmetros opcionais ApplicationSecurityGroup e ApplicationSecurityGroupId foram adicionados
    - New-AzureRmNetworkSecurityRuleConfig foi atualizado: os parâmetros opcionais SourceApplicationSecurityGroup, SourceApplicationSecurityGroupId, DestinationApplicationSecurityGroup e DestinationApplicationSecurityGroupId foram adicionados
    - Add-AzureRmNetworkSecurityRuleConfig foi atualizado: os parâmetros opcionais SourceApplicationSecurityGroup, SourceApplicationSecurityGroupId, DestinationApplicationSecurityGroup e DestinationApplicationSecurityGroupId foram adicionados
    - Set-AzureRmNetworkSecurityRuleConfig foi atualizado: os parâmetros opcionais SourceApplicationSecurityGroup, SourceApplicationSecurityGroupId, DestinationApplicationSecurityGroup e DestinationApplicationSecurityGroupId foram adicionados
  * Foram adicionados novos comandos para os Scripts de VpnDeviceConfiguration
    - Get-AzureRmVirtualNetworkGatewaySupportedVpnDevices
    - Get-AzureRmVirtualNetworkGatewayConnectionVpnDeviceConfigScript
* Perfil
  * Suporte de Tarefa de Início para cmdlets do AzureRm.
    * A todos os AzureRmCmdlets foi adicionado o parâmetro -AzureRmContext, que pode aceitar um contexto (saída de um cmdlet de Contexto).
      - Padrão comum para as tarefas com a persistência de contexto DESATIVADO:`Start-Job {param ($context) New-AzureRmVM -AzureRmContext $context [... other parameters]} -ArgumentList (Get-AzureRmContext)`
      - Padrão comum para as tarefas com a persistência de contexto ATIVADO:`Start-Job {New-AzureRmVM [... other parameters]}`
  * Manter as informações de início de sessão entre sessões, cmdlets novos:
    - Enable-AzureRmContextAutosave - ativar a persistência de início de sessão entre sessões.
    - Disable-AzureRmContextAutosave - desativar a persistência de início de sessão entre sessões.
  * Gerir informações de contexto, cmdlets novos
    - Select-AzureRmContext - selecionar o contexto nomeado ativo.
    - Rename-AzureRmContext - mudar o nome de um contexto existente para facilidade de referência.
    - Remove-AzureRmContext - remover um contexto existente.
    - Remove-AzureRmAccount - remover todas as credenciais, subscrições e os inquilinos associados a uma conta.
  * Gerir informações de contexto, alterações de cmdlet:
    - Foi adicionado o Âmbito = (Processo | CurrentUser) a todos os cmdlets que alteram credenciais
    - Get-AzureRmContext - o parâmetro ListAvailable foi adicionado para listar todos os contextos guardados
* Recursos
  * Adição de cmdlets PolicySetDefinition
    - Cmdlet New-AzureRmPolicySetDefinition para criar uma definição de conjunto de políticas
    - Cmdlet Get-AzureRmPolicySetDefinition para listar todas as definições de conjunto de políticas ou para obter uma definição de conjunto de políticas específica
    - Cmdlet Remove-AzureRmPolicySetDefinition para eliminar uma definição de conjunto de políticas
    - Cmdlet Set-AzureRmPolicySetDefinition para atualizar uma definição de conjunto de políticas existente
  * Adição dos parâmetros -PolicySetDefinition, -Sku e -NotScope aos cmdlets New-AzureRmPolicyAssignment e Set-AzureRmPolicyAssignment
  * Adição de suporte para passar o url de política para os cmdlets New-AzureRmPolicyDefinition e Set-AzureRmPolicyDefinition
  * Adição do parâmetro -Mode ao cmdlet New-AzureRmPolicyDefinition
  * Adição de Suporte para a remoção de roleassignment com o objeto de PSRoleAssignment
    - Os utilizadores podem agora utilizar o inputobject PSRoleassignmnet com o commandlet Remove-AzureRMRoleAssignment para remover o roleassignment.
  * Adição de cmdlets ManagedApplication
    - Cmdlet New-AzureRmManagedApplication para criar uma aplicação gerida
    - Cmdlet Get-AzureRmManagedApplication para listar todos as aplicações geridas numa subscrição ou para obter uma aplicação gerida específica
    - Cmdlet Remove-AzureRmManagedApplication para eliminar uma aplicação gerida
    - Cmdlet Set-AzureRmManagedApplication para atualizar uma aplicação gerida existente
  * Adição de cmdlets ManagedApplicationDefinition
    - Cmdlet New-AzureRmManagedApplicationDefinition para criar uma definição de aplicação gerida com um uri de ficheiro zip ou com ficheiros json mainTemplate e createUiDefinition
    - Cmdlet Get-AzureRmManagedApplicationDefinition para listar todas as definições de aplicação gerida num grupo de recursos ou para obter uma definição de aplicação gerida específica
    - Cmdlet Remove-AzureRmManagedApplicationDefinition para eliminar uma definição de aplicação gerida
    - Cmdlet Set-AzureRmManagedApplicationDefinition para atualizar uma definição de aplicação gerida existente
* SQL
  * Adicionar suporte para as Regras de Rede Virtual
    - Adicionar o cmdlet Get-AzureRmSqlServerVirtualNetworkRule, que obtém as regras de rede virtual através de um nome de regra específico ou uma lista de regras de rede virtual no servidor Sql do Azure.
    - Adicionar o cmdlet Set-AzureRmSqlServerVirtualNetworkRule, que altera a rede virtual para a qual a regra aponta.
    - Adicionar o cmdlet Remove-AzureRmSqlServerVirtualNetworkRule que remove uma regra de rede virtual para um servidor Sql do Azure.
    - Adicionar o cmdlet New-AzureRmSqlServerVirtualNetworkRule que cria uma nova regra de rede virtual para um servidor Sql do Azure.
* Sites
  * Adição do Escalão PremiumV2 para Planos do Serviço de Aplicações
* Azure.Storage
  * Atualizar para a Biblioteca de Clientes do Armazenamento do Microsoft Azure 8.4.0 e a Biblioteca do DataMovement de Armazenamento do Azure 0.6.1
  * Adição de Suporte PremiumPageBlobTier na API para Carregar e Copiar Blob
    - Set-AzureStorageBlobContent
    - Start-AzureStorageBlobCopy
  * Otimizar o Formato de Saída da Consola do AzureStorageContainer, AzureStorageBlob, AzureStorageQueue, AzureStorageTable
    - Get-AzureStorageContainer
    - Get-AzureStorageBlob
    - Get-AzureStorageQueue
    - Get-AzureStorageTable

## <a name="20170810---version-431"></a>10-08-2017 - Versão 4.3.1
  * Atualização para corrigir o problema de assinatura da assemblagem

## <a name="20170807---version-430"></a>07-08-2017 - Versão 4.3.0
* AnalysisServices
  * Erro corrigido em Set-AzureRmAnalysisServciesServer
    - Quando o administrador não é fornecido, o mesmo será removido.
  * BackupBlobContainerUri adicionado em New-AzureRmAnalysisServicesServer e Set-AzureRmAnalysisServicesServer
    - Pode definir/desativar o contentor de blobs de cópia de segurança para fazer a cópia de segurança ou o restauro do Servidor do Azure Analysis Services
  * Pesquisa de SKU atualizada em New-AzureRmAnalysisServicesServer e Set-AzureRmAnalysisServicesServer
    - SKU hard-coded alterado para pesquisa dinâmica.
  * Add-AzureAnalysisServicesAccount para suportar o início de sessão com o Principal de Serviço
* Automatização
  * Alterações aos cmdlets AutomationDSC* para extrair mais do que 100 registos
  * Resolvido o problema em que os fluxos Verbosos paravam de funcionar depois de chamar alguns cmdlets da Automatização (por exemplo, Get-AzureRmAutomationVariable, Get-AzureRmAutomationJob).
  * Adicionado o suporte para o controlo de versões da Compilação NodeConfiguration em StartAzureAutomationDscCompilationJob e ImportAzureAutomationDscNodeConfiguration
  * Correções de erros existentes - A correção do problema de alias é #3775 e do alias runOn e do suporte para HybridWorkers.
* Computação
  * Set-AzureRmVMAEMExtension: adiciona suporte para novos tamanhos de Disco Premium
  * Set-AzureRmVMAEMExtension: adiciona suporte para a série M
  * Adicionado o parâmetro ForceUpdateTag a Add-AzureRmVmssExtension
  * Adicionado o parâmetro Principal a New-AzureRmVmssIpConfig
  * Adicionado o parâmetro EnableAcceleratedNetworking a Add-AzureRmVmssNetworkInterfaceConfig
  * Adicionado o InstanceId a Set-AzureRmVmss
  * Exposição de MaintenanceRedeployStatus a Get-AzureRmVM -Saída do estado
  * Exposição da Restrição e Capacidade ao formato de tabela de Get-AzureRmComputeResourceSku
* DataLakeStore
  * Corrija o problema: https://github.com/Azure/azure-powershell/issues/4323
* EventHub
  * Adicionada a propriedade ResourceGroup a NamespaceAttributes
    - “ResourceGroup” obtém o nome do grupo de recursos em que se encontra o Espaço de Nomes
  * Atualizados os cmdlets com ParameterSets para o Espaço de Nomes e EventHub para o funcionamento de AuthorizationRule
    - New-AzureRmEventHubAuthorizationRule - Adiciona uma nova AuthorizationRule ao Espaço de Nomes ou EventHub existentes.
    - Get-AzureRmEventHubAuthorizationRule - Obtém a AuthorizationRule/Lista de AuthorizationRules do Espaço de Nomes ou EventHub existentes.
    - Set-AzureRmEventHubAuthorizationRule - Atualiza as propriedades da AuthorizationRule ou EventHub existentes.
    - Remove-AzureRmEventHubAuthorizationRule - Elimina a AuthorizationRule existente do Espaço de Nomes ou EventHub existentes.
    - New-AzureRmEventHubKey - Gera uma nova Chave Primária/Secundária da AuthorizationRule do Espaço de Nomes ou EventHub existentes.
    - Get-AzureRmEventHubKey - Obtém a Chave Primária/Secundária da AuthorizationRule do Espaço de Nomes ou EventHub existentes.
* Rede
    * Adicionado suporte para IPv6 e o novo parâmetro opcional -PeerAddressType
      * New-AzureRmExpressRouteCircuitPeeringConfig:
      * Set-AzureRmExpressRouteCircuitPeeringConfig: adicionado suporte para IPv6. Novo parâmetro opcional adicionado
      * Remove-AzureRmExpressRouteCircuitPeeringConfig: adicionado suporte para IPv6. Novo parâmetro opcional adicionado
    * Parâmetro marcado -ProbeEnabled como obsoleto
      - Add-AzureRmApplicationGatewayBackendHttpSettings
      - New-AzureRmApplicationGatewayBackendHttpSettings
      - Set-AzureRmApplicationGatewayBackendHttpSettings
* Perfil
    * A recolha de dados foi ativada por predefinição. Os dados de utilização são recolhidos pela Microsoft para melhorar a experiência de utilizador. Os dados são anónimos e não incluem valores de argumento da linha de comandos.
      - Utilize o cmdlet Disable-AzureRmDataCollection para desativar a funcionalidade
      - Utilize o cmdlet Enable-AzureRmDataCollection para ativar a funcionalidade
* Recursos
    * Adicionado Suporte para a validação de âmbitos para os seguintes commandlets de roledefinition e roleassignment antes de enviar o pedido para o ARM
      - Get-AzureRMRoleAssignment
      - New-AzureRMRoleAssignment
      - Remove-AzureRMRoleAssignment
      - Get-AzureRMRoleDefinition
      - New-AzureRMRoleDefinition
      - Remove-AzureRMRoleDefinition
      - Set-AzureRMRoleDefinition
* ServiceBus
    * Adicionado abaixo novos commandlets para AuthorizationRules do Espaço de Nomes, Fila e Tópico. De acordo com o parâmetro definido, as operações da regra de autorização são realizadas.
     - New-AzureRmServiceBusAuthorizationRule - Adiciona uma nova AuthorizationRule ao Espaço de Nomes/Fila/Tópico existente do ServiceBus.
     - Get-AzureRmServiceBusAuthorizationRule - Obtém a AuthorizationRule/Lista de AuthorizationRules do Espaço de Nomes/Fila/Tópico existente do ServiceBus.
     - Set-AzureRmServiceBusAuthorizationRule - Atualiza as propriedades da AuthorizationRule existente do Espaço de Nomes/Fila/Tópico do ServiceBus.
     - New-AzureRmServiceBusKey - Gera uma nova Chave Primária/Secundária da AuthorizationRule do Espaço de Nomes/Fila/Tópico existente do ServiceBus.
     - Get-AzureRmServiceBusKey - Obtém a Chave Primária/Secundária da AuthorizationRule do Espaço de Nomes/Fila/Tópico existente do ServiceBus.
     - Remove-AzureRmServiceBusNamespaceAuthorizationRule - Elimina a AuthorizationRule existente do Espaço de Nomes/Fila/Tópico do ServiceBus.
    * Adicionada a propriedade ResourceGroup a NamespaceAttributes
* SQL
    * Atualização de Set-AzureRmSqlServerTransparentDataEncryptionProtector para apresentar um aviso e pedir confirmação se o Tipo de Protetor de Encriptação estiver definido para AzureKeyVault
    * A adicionar novos cmdlets atualizados para as definições de Auditoria
      - Cmdlet Get-AzureRmSqlDatabaseAuditing, o qual obtém as definições de auditoria de uma base de dados SQL do Azure.
      - Cmdlet Get-AzureRmSqlServerAuditing, o qual obtém as definições de auditoria de um servidor SQL do Azure.
      - Cmdlet Set-AzureRmSqlDatabaseAuditing, o qual altera as definições de auditoria de uma base de dados SQL do Azure.
      - Cmdlet Set-AzureRmSqlServerAuditing, o qual altera as definições de auditoria de um servidor SQL do Azure.
    * Descontinuar os cmdlets existentes da política de Auditoria
      - Get-AzureRmSqlDatabaseAuditingPolicy
      - Get-AzureRmSqlServerAuditingPolicy
      - Set-AzureRmSqlDatabaseAuditingPolicy
      - Set-AzureRmSqlServerAuditingPolicy
      - Use-AzureRmSqlServerAuditingPolicy
      - Remove-AzureRmSqlDatabaseAuditing
      - Remove-AzureRmSqlServerAuditing
    * A análise do ficheiro de esquema de Update-AzureRmSqlSyncGroup passa a ser não sensível às maiúsculas e minúsculas.
* Armazenamento
    * Adicionado suporte a NeworkRule para os cmdlets de conta de armazenamento do modo de recursos
      - New-AzureRmStorageAccount
      - Set-AzureRmStorageAccount
      - Get-AzureRmStorageAccountNetworkRuleSet
      - Update-AzureRmStorageAccountNetworkRuleSet
      - Add-AzureRmStorageAccountNetworkRule
      - Remove-AzureRmStorageAccountNetworkRule

## <a name="20170717---version-421"></a>17-07-2017 - Versão 4.2.1
* Computação
    - Correção do problema dos cmdlets de criação e atualização do Disco da VM e do instantâneo do Disco da VM, (ligação)[https://github.com/azure/azure-powershell/issues/4309]
      - New-AzureRmDisk
      - New-AzureRmSnapshot
      - Update-AzureRmDisk
      - Update-AzureRmSnapshot
* Perfil
    - Correção do problema com autenticação de utilizador não interativo em RDFE (ligação) [https://github.com/Azure/azure-powershell/issues/4299]
* ServiceManagement
    - Correção do problema com autenticação de utilizador não interativo (ligação) [https://github.com/Azure/azure-powershell/issues/4299]

## <a name="2017711---version-420"></a>11-07-2017 - Versão 4.2.0
* AnalysisServices
    * Adicionar nova API de plano de dados
        - Introdução de uma API para obter o registo do servidor AS, Export-AzureAnalysisServicesInstanceLog
* Automatização
    * Definição correta do valor TimeZone dos agendamentos Semanal e Mensal para New-AzureRmAutomationSchedule
        - Pode encontrar mais informações neste problema: https://github.com/Azure/azure-powershell/issues/3043
* AzureBatch
    - Adicionado o novo cmdlet Get-AzureBatchJobPreparationAndReleaseTaskStatus.
    - Adicionado o início e fim do intervalo de bytes aos parâmetros Get-AzureBatchNodeFileContent.
* CognitiveServices
    * Integração na versão 1.0.0 do SDK de Gestão dos Serviços Cognitivos.
    * Correção do erro de verificação do comprimento do nome da conta.
* Computação
    * Suporte do tipo de conta de armazenamento para disco de Imagem:
        - Adicionado o parâmetro “StorageAccountType” a Set-AzureRmImageOsDisk e Add-AzureRmImageDataDisk
    * Funcionalidade PrivateIP e PublicIP na Configuração de IP do VMSS:
        - Adicionados os nomes “PrivateIPAddressVersion”, “PublicIPAddressConfigurationName”, “PublicIPAddressConfigurationIdleTimeoutInMinutes” e “DnsSetting” a New-AzureRmVmssIpConfig
        - Adicionado o parâmetro “PrivateIPAddressVersion” para especificar IPv4 ou IPv6 a New-AzureRmVmssIpConfig
    * Funcionalidade de Manutenção do Desempenho:
        - Adicionado o parâmetro opcional “PerformMaintenance” a Restart-AzureRmVM.
        - Get-AzureRmVM -Status apresenta as informações de manutenção do desempenho da VM especificada
    * Funcionalidade de Identidade da Máquina Virtual:
        - Adicionado o parâmetro “IdentityType” a New-AzureRmVMConfig e UpdateAzureRmVM
        - Get-AzureRmVM apresenta as informações da identidade da VM especificada
    * Funcionalidade de Identidade do VMSS:
        - Adicionado o parâmetro “IdentityType” a New-AzureRmVmssConfig
        - Get-AzureRmVmss apresenta as informações da identidade do VMSS especificado
    * Funcionalidade de Diagnóstico de Arranque do VMSS:
        - Novo cmdlet para definir o diagnóstico de arranque do objeto VMSS: Set-AzureRmVmssBootDiagnostics
        - Adicionado o parâmetro “BootDiagnostic” a New-AzureRmVmssConfig
    * Funcionalidade LicenseType do VMSS:
        - Adicionado o parâmetro “LicenseType” a New-AzureRmVmssConfig
    * Suporte de RecoveryPolicyMode:
        - Adicionado o parâmetro “RecoveryPolicyMode” a New-AzureRmVmssConfig
    * Funcionalidade de SKU de Recursos de Computação:
        - Novo cmdlet “Get-AzureRmComputeResourceSku” lista todos os SKUs de recursos de computação
* DataFactories
    * New-AzureRmDataFactoryGatewayKey preterido
    * Introduza a funcionalidade de chave de autenticação de gateway ao adicionar New-AzureRmDataFactoryGatewayAuthKey e Get-AzureRmDataFactoryGatewayAuthKey
* DataLakeAnalytics
    * Adicione suporte para CRUD da Política de Computação com os seguintes comandos:
        - New-AzureRMDataLakeAnalyticsComputePolicy
        - Get-AzureRMDataLakeAnalyticsComputePolicy
        - Remove-AzureRMDataLakeAnalyticsComputePolicy
        - Update-AzureRMDataLakeAnalyticsComputePolicy
    * Adicione suporte para metadados de relação de tarefa para obter ajuda com tarefas periódicas e pipelines de tarefa. Os comandos seguintes foram atualizados ou adicionados:
        - Submit-AzureRMDataLakeAnalyticsJob
        - Get-AzureRMDataLakeAnalyticsJob
        - Get-AzureRMDataLakeAnalyticsJobRecurrence
        - Get-AzureRMDataLakeAnalyticsJobPipeline
    * Atualizada a audiência do token para tarefas e APIs de catálogo para utilizar a audiência específica do Data Lake correta em vez da audiência do Recurso do Azure.
* DataLakeStore
    * Adicionado suporte para rotações de chave do KeyVault gerido pelo utilizador no cmdlet Set-AzureRMDataLakeStoreAccount
    * Adicionada uma atualização de qualidade de vida para acionar automaticamente uma chamada `enableKeyVault` quando um KeyVault gerido pelo utilizador é adicionado ou uma chave é rodada.
    * Atualizada a audiência do token para tarefas e APIs de catálogo para utilizar a audiência específica do Data Lake correta em vez da audiência do Recurso do Azure.
    * Correção do erro que limitava o tamanho dos ficheiros criados/acrescentados com os seguintes cmdlets:
        - New-AzureRmDataLakeStoreItem
        - Add-AzureRmDataLakeStoreItemContent
* Dns
    * Correção do erro no cenário de tubagem para Get-AzureRmDnsZone
        - Pode encontrar mais informações aqui: https://github.com/Azure/azure-powershell/issues/4203
* HDInsight
    * Adicionado suporte para ativar/desativar o Operations Management Suite (OMS)
    * Novos cmdlets
        - Enable-AzureRmHDInsightOperationsManagementSuite
        - Disable-AzureRmHDInsightOperationsManagementSuite
        - Get-AzureRmHDInsightOperationsManagementSuite
    * Adicione novos parâmetros para definir configurações personalizadas do Spark a Add-AzureRmHDInsightConfigValues
        - Parâmetros SparkDefaults e SparkThriftConf para o Spark 1.6
        - Parâmetros Spark2Defaults e Spark2ThriftConf para o Spark 2.0
* Informações
    * Problema #4215 (pedido de alteração) remove o limite de 15 dias na janela de tempo para o cmdlet Get-AzureRmLog. Também foram realizadas pequenas alterações aos nomes do teste de unidades.
    * Problema #3957 corrigido para Get-AzureRmLog
        - Problema #1: o back-end devolve os registos em páginas de 200 registos cada, ligados pelo token de continuação para a página seguinte. Os clientes viam o cmdlet devolver apenas 200 registos quando sabiam que existiam mais. Este problema ocorria independentemente do valor configurado para MaxEvents, a menos que o valor fosse inferior a 200.
        - Problema #2: a documentação continha dados incorretos sobre este cmdlet. Por exemplo: a timewindow predefinida era 1 hora.
        - Correção #1: agora, o cmdlet segue o token de continuação devolvido pelo back-end até atingir MaxEvents ou o fim do conjunto.<br>O valor predefinido para MaxEvents é 1000 e o máximo é 100000. Qualquer valor em MaxEvents inferior a 1 é ignorado sendo utilizada a predefinição. Estes valores e o comportamento não mudaram, mas agora estão documentados corretamente.<br>Foi adicionado um alias para MaxEvents - MaxRecords - uma vez que o nome do cmdlet já não se refere a eventos, mas apenas a Registos.
        - Correção #2: a documentação contém informações corretas e mais detalhadas: novo alias, janela de tempo correta, predefinição correta e valores mínimos e máximos.
* KeyVault
    * Remova o endereço de e-mail da consulta de diretório quando -UserPrincipalName está especificado para os cmdlets Set-AzureRMKeyVaultAccessPolicy e Remove-AzureRMKeyVaultAccessPolicy.
      - Agora, ambos os Cmdlets têm um parâmetro -EmailAddress que pode ser utilizado em vez do parâmetro -UserPrincipalName quando é adequado consultar o endereço de e-mail.  Se existir mais do que uma correspondência de endereços de e-mail no diretório, o Cmdlet irá falhar.
* Rede
    * New-AzureRmIpsecPolicy: SALifeTimeSeconds e SADataSizeKilobytes já não são parâmetros obrigatórios
        - A predefinição de SALifeTimeSeconds é 27000 segundos
        - A predefinição de SADataSizeKilobytes é 102400000 KB
    * Adicionado suporte para a configuração personalizada do conjunto de cifras através da política SSL e ao listar todas as APIs de opções de SSL no Gateway de Aplicação
        - Adicionados os parâmetros opcionais -PolicyType, -PolicyName, -MinProtocolVersion, -Ciphersuite
            - Add-AzureRmApplicationGatewaySslPolicy
            - New-AzureRmApplicationGatewaySslPolicy
            - Set-AzureRmApplicationGatewaySslPolicy
        - Adicionado Get-AzureRmApplicationGatewayAvailableSslOptions (Alias: List-AzureRmApplicationGatewayAvailableSslOptions)
        - Adicionado Get-AzureRmApplicationGatewaySslPredefinedPolicy (Alias: List-AzureRmApplicationGatewaySslPredefinedPolicy)
    * Adicionado suporte de redirecionamento no Gateway de Aplicação
        - Adicionado Add-AzureRmApplicationGatewayRedirectConfiguration
        - Adicionado Get-AzureRmApplicationGatewayRedirectConfiguration
        - Adicionado New-AzureRmApplicationGatewayRedirectConfiguration
        - Adicionado Remove-AzureRmApplicationGatewayRedirectConfiguration
        - Adicionado Set-AzureRmApplicationGatewayRedirectConfiguration
        - Adicionado o parâmetro opcional - RedirectConfiguration
            - Add-AzureRmApplicationGatewayRequestRoutingRule
            - New-AzureRmApplicationGatewayRequestRoutingRule
            - Set-AzureRmApplicationGatewayRequestRoutingRule
        - Adicionado o parâmetro opcional -DefaultRedirectConfiguration
            - Add-AzureRmApplicationGatewayUrlPathMapConfig
            - New-AzureRmApplicationGatewayUrlPathMapConfig
            - Set-AzureRmApplicationGatewayUrlPathMapConfig
        - Adicionado o parâmetro opcional - RedirectConfiguration
            - Add-AzureRmApplicationGatewayPathRuleConfig
            - New-AzureRmApplicationGatewayPathRuleConfig
            - Set-AzureRmApplicationGatewayPathRuleConfig
        - Adicionado o parâmetro opcional -RedirectConfigurations
            - New-AzureRmApplicationGateway
            - Set-AzureRmApplicationGateway
    * Adicionado suporte para sites do Azure no Gateway de Aplicação
        - Adicionado New-AzureRmApplicationGatewayProbeHealthResponseMatch
        - Adicionados os parâmetros opcionais -PickHostNameFromBackendHttpSettings, -MinServers, -Match
            - Add-AzureRmApplicationGatewayProbeConfig
            - New-AzureRmApplicationGatewayProbeConfig
            - Set-AzureRmApplicationGatewayProbeConfig
        - Adicionados os parâmetros opcionais -PickHostNameFromBackendAddress, -AffinityCookieName, -ProbeEnabled, -Path
            - Add-AzureRmApplicationGatewayBackendHttpSettings
            - New-AzureRmApplicationGatewayBackendHttpSettings
            - Set-AzureRmApplicationGatewayBackendHttpSettings
    * Atualizar Get-AzureRmPublicIPaddress para obter recursos publicipaddress criados através do Conjunto de Dimensionamento de VM
    * Adicionado um cmdlet para obter a utilização atual da rede virtual
        - Get-AzureRmVirtualNetworkUsageList
* Perfil
    * Correção do erro que ocorria ao utilizar Import-AzureRmContext ou Save-AzureRmContext
        - Pode encontrar mais informações neste problema: https://github.com/Azure/azure-powershell/issues/3954
* RecoveryServices.SiteRecovery
    * Introdução de um novo módulo para as operações do Azure Site Recovery.
        - Todos os cmdlets começam por AzureRmRecoveryServicesAsr*
* SQL
    * Adicionados Cmdlets do PowerShell de Sincronização de Dados a AzureRM.Sql
    * Atualizados os cmdlets AzureRmSqlServer para utilizar a nova versão da API REST que evita limites de tempo durante a criação de um servidor.
    * Cmdlets de atualização do servidor preteridos porque a versão antiga do servidor (2.0) já não existe.
    * Adicione um novo parâmetro opcional "AssignIdentity" aos cmdlets New-AzureRmSqlServer e Set-AzureRmSqlServer para suportar o aprovisionamento de uma identidade de recurso para o recurso do servidor SQL
    * O parâmetro ResourceGroupName é agora opcional para Get-AzureRmSqlServer
        - Pode encontrar mais informações no seguinte problema: https://github.com/Azure/azure-powershell/issues/635
* ServiceManagement   Para o ExpressRoute:
    * Atualizado o cmdlet New-AzureBgpPeering para adicionar as novas opções seguintes:
        - PeerAddressType : os valores de "IPv4" ou "IPv6" podem ser especificados para criar um Peering de BGP do tipo de família de endereços correspondente
    * Atualizado o cmdlet Set-AzureBgpPeering para adicionar as novas opções seguintes:
        - PeerAddressType : os valores de "IPv4" ou "IPv6" podem ser especificados para atualizar um Peering de BGP do tipo de família de endereços correspondente
    * Atualizado o cmdlet Remove-AzureBgpPeering para adicionar as novas opções seguintes:
        - PeerAddressType : os valores de "IPv4", "IPv6" ou Todos podem ser especificados para remover um Peering de BGP do tipo de família de endereços correspondente ou todos

## <a name="20170607---version-410"></a>07-06-2017 - Versão 4.1.0
* AnalysisServices
    * Novos SKUs adicionados: B1, B2, S0
    * Adicionado suporte para aumento/redução vertical
* CognitiveServices
    * Atualizada a apresentação detalhada de contratos de licença ao criar recursos dos Serviços Cognitivos
* Computação
    * Correção de Test-AzureRmVMAEMExtension para máquinas virtuais com vários discos geridos
    * Atualizado o Set-AzureRmVMAEMExtension: adicionar informações de cache para discos geridos Premium
    * Add-AzureRmVhd: o tamanho limite no VHD foi aumentado para 4 TB.
    * Stop-AzureRmVM: documentação de esclarecimento do parâmetro STayProvisioned
    * New-AzureRmDiskUpdateConfig
      * Parâmetros preteridos: CreateOption, StorageAccountId, ImageReference, SourceUri, SourceResourceId
    * Set-AzureRmDiskUpdateImageReference: cmdlet preterido
    * New-AzureRmSnapshotUpdateConfig
      * Parâmetros preteridos: CreateOption, StorageAccountId, ImageReference, SourceUri, SourceResourceId
    * Set-AzureRmSnapshotUpdateImageReference: cmdlet preterido
* DataLakeStore
    * Enable-AzureRmDataLakeStoreKeyVault (Enable-AdlStoreKeyVault)
      * Ativar a encriptação gerida pelo KeyVault para um DataLake Store
* DevTestLabs
    * Atualização de cmdlets para funcionar com a versão de API do DevTest Labs atual e atualizada.
* IotHub
    * Adicionado suporte de Encaminhamento para os cmdlets do IoTHub
* KeyVault
  * Novos Cmdlets para suportar as Chaves de Conta de Armazenamento Geridas pelo KeyVault
    * Get-AzureKeyVaultManagedStorageAccount
    * Add-AzureKeyVaultManagedStorageAccount
    * Remove-AzureKeyVaultManagedStorageAccount
    * Update-AzureKeyVaultManagedStorageAccount
    * Update-AzureKeyVaultManagedStorageAccountKey
    * Get-AzureKeyVaultManagedStorageSasDefinition
    * Set-AzureKeyVaultManagedStorageSasDefinition
    * Remove-AzureKeyVaultManagedStorageSasDefinition
* Rede
    * Get-AzureRmNetworkUsage: novo cmdlet que mostra os detalhes da utilização e da capacidade da rede
    * Adicionadas novas opções de GatewaySku para VirtualNetworkGateways
        * VpnGw1, VpnGw2 e VpnGw3 são os novos SKUs adicionados para gateways de VPN
    * Set-AzureRmNetworkWatcherConfigFlowLog
      * Exemplos de ajuda de correção
* NotificationHubs
    * Atualização Transparente para os cmdlets do NotificationHubs para a nova API
* Perfil
    * Resolve-AzureRmError
      * Novo cmdlet para mostrar detalhes de erros e exceções acionadas por cmdlets, incluindo pedidos de servidor/dados de resposta
    * Send-Feedback
      * Ativado o envio de comentários sem iniciar sessão
    * Get-AzureRmSubscription
      * Correção do erro que ocorria ao obter subscrições de CSP
* Recursos
    * Correção do problema em que Get-AzureRMRoleAssignment resultava num Pedido Inválido se o número de roleassignments fosse superior a 1000
        * Agora, os utilizadores podem utilizar Get-AzureRMRoleAssignment mesmo que as roleassignments a ser devolvidas sejam superiores a 1000
* SQL
    * Restore-AzureRmSqlDatabase: exemplo de documentação de atualização
* Armazenamento
    * Adicionado suporte da definição de AssignIdentity aos cmdlets de conta de armazenamento do modo de recursos
        * New-AzureRmStorageAccount
        * Set-AzureRmStorageAccount
    * Adicionado Suporte à Chave de Cliente aos cmdlets de conta de armazenamento do modo de recursos
        * Set-AzureRmStorageAccount
        * New-AzureRmStorageAccountEncryptionKeySource
* TrafficManager

    * Novas definições de Monitorização “MonitorIntervalInSeconds”, “MonitorTimeoutInSeconds”, “MonitorToleratedNumberOfFailures”
    * Novo protocolo de Monitorização “TCP”
* ServiceManagement
    * Add-AzureVhd: o tamanho limite no VHD foi aumentado para 4 TB.
    * New-AzureBGPPeering: Suporte para LegacyMode
* Azure.Storage
    * Atualização da ajuda para parâmetros que aceitam carateres universais e atualizam o tipo StorageContext

## <a name="20170523---version-402"></a>23-05-2017 - Versão 4.0.2
* Perfil
    * Add-AzureRmAccount
      * Adicionado o parâmetro de alias `-EnvironmentName` para retrocompatibilidade com as versões 2.x do AzureRM.profile

## <a name="20170512---version-401"></a>12-05-2017 - Versão 4.0.1
 * Correção do problema com New-AzureStorageContext em cenários offline: https://github.com/Azure/azure-powershell/issues/3939

## <a name="20170510---version-400"></a>10-05-2017 - Versão 4.0.0


* Esta versão contém alterações recentes. Veja [o guia de migração](https://aka.ms/azps-migration-guide) para detalhes de alteração e o impacto em scripts existentes.
* ApiManagement
  - Foi adicionado suporte para a configuração de grupos externos no New-AzureRmApiManagementGroup.
* Faturação
  - Novo Cmdlet Get-AzureRmBillingPeriod
    + cmdlet para obter os períodos de faturação do azure da subscrição.
  - Atualizar Cmdlet Get-AzureRmBillingInvoice
  - nova propriedade BillingPeriodNames
  - saída na vista de lista
* Computação
  - Set-AzureRmVMAEMExtension atualizado e cmdlets Test-AzureRmVMAEMExtension para suportar os discos geridos Premium
  - Definições de encriptação de cópias de segurança de VMs de IaaS e o restauro em caso de falha
  - A opção de ChefServiceInterval é agora alterada para ChefDaemonInterval. No entanto o antigo continuará a funcionar.
  - Remover DataDiskNames duplicados e propriedades NetworkInterfaceIDs do objeto de PS VM.
  - Tornar os parâmetros DataDiskNames e NetworkInterfaceIDs opcionais em Remove-AzureRmVMDataDisk e Remove-AzureRmVMNetworkInterface, respetivamente.
  - Corrigir o problema de suportes de tubagem dos Get cmdlets quando os cmdlets Get devolvem um objeto de lista.
  - Os cmdlets que entraram em conflito com os cmdlets RDFE foram alterados no nome. Veja o problema https://github.com/Azure/azure-powershell/issues/2917 para obter mais detalhes
    + `New-AzureVMSqlServerAutoBackupConfig` mudou de nome para `New-AzureRmVMSqlServerAutoBackupConfig`
    + `New-AzureVMSqlServerAutoPatchingConfig` mudou de nome para `New-AzureRmVMSqlServerAutoPatchingConfig`
    + `New-AzureVMSqlServerKeyVaultCredentialConfig` mudou de nome para `New-AzureRmVMSqlServerKeyVaultCredentialConfig`
* Consumo
  - Novo Cmdlet Get-AzureRmConsumptionUsageDetail
    + cmdlet para obter detalhes de utilização da subscrição.
* ContainerRegistry
  - Adicionar os cmdlets do PowerShell para o Azure Container Registry
    + New-AzureRmContainerRegistry
    + Get-AzureRmContainerRegistry
    + Update-AzureRmContainerRegistry
    + Remove-AzureRmContainerRegistry
    + Get-AzureRmContainerRegistryCredential
    + Update-AzureRmContainerRegistryCredential
    + Test-AzureRmContainerRegistryNameAvailability
* DataLakeAnalytics
  - Adicionar suporte obter o pacote de catálogo e a lista
  - Adicionar suporte para listar os seguintes itens de catálogo de predecessores mais profundos:
    + Tabela
    + TVF
    + Vista
    + Estatísticas
* DataLakeStore
  - Para `Import-AzureRMDataLakeStoreItem` e `Export-AzureRMDataLakeStoreItem` o registo de controlo foi desativado por predefinição, para melhorar o desempenho. Se o registo de controlo for pretendido, utilize os parâmetros `-DiagnosticLogLevel` e `-DiagnosticLogPath`
  - Corrigir um erro que fará com que, por vezes, PowerShell falhe ao carregar grandes quantidades de ficheiro pequeno para ADLS.
* EventHub
  - Correção de erros:
    + Corrigir para erro de cmdlet Set-AzureRmEventHubNamespace  - "escalão" não pode ser nulo, onde deveria ser "SkuName"
    + Set-AzureRmEventHub - corrigir referência de objeto não definida para uma instância de um erro de objeto ao atualizar o EventHub
* Informações
  - Add-AzureRm*AlertRule
    + Devolve um único objeto: newResource, statusCode, requestId
  - Get-AzureRmAlertRule
    + O resultado é agora enumerado em vez de considerado um único objeto. Não foi alterado o respetivo tipo, ainda é uma lista.
  - Remove-AzureRmAlertRule
    + O statusCode segue o código de estado devolvido pelo pedido, antes foi sempre OK.
  - Add-AzureRmAutoscaleSetting
    + Devolve agora um único objeto (não uma lista como anteriormente), contendo o statusCode, requestId e o recurso recentemente criado/atualizado.
    + O código de estado segue o estado devolvido pelo pedido, antes foi sempre OK.
  - New-AzureRmAutoscaleRule
    + O parâmetro ScaleActionType foi expandido e recebe os seguintes valores agora: ChangeCount, PercentChangeCount, ExactCount.
  - Remove-AzureRmAutoscaleSetting
    + O statusCode no resultado segue o statusCode devolvido pelo pedido. Antes foi sempre Ok.
  - Get-AzureRmLogProfile
    + O resultado é agora enumerado. Antes foi considerado um único objeto. O tipo de saída do mantém-se uma lista como antes.
  - Remove-AzureRmLogProfile
    + O parâmetro PassThru foi implementado.
  - API de métricas
    + O SDK agora obtém as métricas de MDM.
  - Get-AzureRmMetricDefinition
    + A saída ainda é uma lista, mas a estrutura da lista foi alterada.
  - Get-AzureRmMetric
    + A chamada foi alterada. Esta é a nova sintaxe: Get-AzureRmMetric ResourceId [MetricNames [TimeGrain] [AggregationType] [StartTime] [EndTime]] [DetailedOutput]
    + O resultado é uma lista e a estrutura dos respetivos elementos foi alterada.
* KeyVault
  - Adicionar suporte de cópia de segurança/restauro para os segredos de KeyVault
    + Os segredos podem ter cópia de segurança e serem restaurados, correspondendo à funcionalidade atual suportada para Chaves

  - Cmdlets de cópia de segurança de Chaves e Segredos aceitam agora um objeto correspondente como um parâmetro de entrada
    + O autor da chamada pode encadear operações de obtenção e cópia de segurança: Get-AzureKeyVaultKey -VaultName myVault -Name myKey | Backup-AzureKeyVaultKey

  - Os cmdlets de cópia de segurança suportam agora uma troca forçada para substituir um ficheiro existente
    + Tenha em atenção que ao tentar substituir o ficheiro existente já não irá gerar e, em vez disso, pedirá ao utilizador para que escolha sobre como proceder.
* LogicApp
  - Novos parâmetros para cmdlets de recuperação de desastres de Intercâmbio de Número de Controlo:
    + Parâmetro - AgreementType opcional ("X12" ou "Edifact") para especificar os números de controlo relevantes
* MachineLearning
  - Consumir nova versão do SDK .NET do Azure Machine Learning e adicionar um novo cmdlet
    + Add-AzureRmMlWebServiceRegionalProperty
  - Correções secundárias de palavras no texto de ajuda.
* Rede
  - Adicionado o cmdlet Test-AzureRmNetworkWatcherConnectivity
    + Devolve as informações de conectividade para uma VM de origem especificada e um destino
    + Se a conectividade entre a origem e o destino não for estabelecida, o cmdlet devolve os detalhes sobre o problema
* Perfil
  - Adicionado o cmdlet "Send-Feedback": permite que um utilizador inicie um conjunto de pedidos que enviam comentários para a equipa do Azure PowerShell.
  - Os aliases seguintes foram removidos uma vez que entraram em conflito com nomes de cmdlet existentes no módulo Azure:
    + `Enable-AzureDataCollection` (suportado por `Enable-AzureRmDataCollection`)
    + `Disable-AzureDataCollection` (suportado por `Disable-AzureRmDataCollection`)
* Reencaminhamento
  - Adiciona os cmdlets para o Reencaminhamento do Azure que permite aos utilizadores criar e gerir todos os recursos de Reencaminhamento do Azure.
    + `New-AzureRmRelayNamespace`
    + `Get-AzureRmRelayNamespace`
    + `Set-AzureRmRelayNamespace`
    + `Remove-AzureRmRelayNamespace`
    + `New-AzureRmWcfRelay`
    + `Get-AzureRmWcfRelay`
    + `Set-AzureRmWcfRelay`
    + `Remove-AzureRmWcfRelay`
    + `New-AzureRmRelayHybridConnection`
    + `Get-AzureRmRelayHybridConnection`
    + `Set-AzureRmRelayHybridConnection`
    + `Remove-AzureRmRelayHybridConnection`
    + `Test-AzureRmRelayName`
    + `Get-AzureRmRelayOperation`
    + `New-AzureRmRelayKey`
    + `Get-AzureRmRelayKey`
    + `New-AzureRmRelayAuthorizationRule`
    + `Get-AzureRmRelayAuthorizationRule`
    + `Set-AzureRmRelayAuthorizationRule`
    + `Remove-AzureRmRelayAuthorizationRule`
* Recursos
  - Suportar implementações de grupo entre recursos para New-AzureRmResourceGroupDeployment
    + Os utilizadores podem agora utilizar implementações aninhadas para implementar em grupos de recursos diferentes.
* ServiceBus

  - Correção de erros: os valores de propriedade do objeto de ServiceBus foram definidos como nulos; o objeto é utilizado como parâmetro de entrada no cmdlet Set-AzureRmServiceBusQueue para atualizar a Fila.
   - As propriedades afetadas são LockDuration, EntityAvailabilityStatus, DuplicateDetectionHistoryTimeWindow, MaxDeliveryCount e MessageCount
* ServiceFabric

  - Cmdlets adicionados ao Service Fabric
    + Add-AzureRmServiceFabricApplicationCertificate        Adicionar um certificado que será utilizado como certificado de aplicação
    + Add-AzureRmServiceFabricClientCertificate       Adicionar um nome comum ou thumbprint para as definições do cluster para autenticação de cliente
    + Add-AzureRmServiceFabricClusterCertificate       Adicionar um certificado de cluster secundário ao cluster para efetuar o rollover no certificado existente
    + Add-AzureRmServiceFabricNodes       Adicionar nós/VMs de um tipo de nó específico a um cluster
    + Add-AzureRmServiceFabricNodeType       Adicionar um tipo de nó/VMs a um cluster existente
    + Get-AzureRmServiceFabricCluster       Obter os detalhes do recurso do cluster
    + New-AzureRmServiceFabricCluster Criar um novo cluster do ServiceFabric. Este comando tem muitas sobrecargas para abranger vários cenários
    + Remove-AzureRmServiceFabricClientCertificate       Impedir que um certificado de cliente seja utilizado para aceder a um cluster
    + Remove-AzureRmServiceFabricClusterCertificate       Impedir que um certificado de cluster seja utilizado para segurança do cluster
    + Remove-AzureRmServiceFabricNodes       Remover os nós de um tipo de nó específico de um cluster
    + Remove-AzureRmServiceFabricNodeType       Remover um tipo de nó de um cluster
    + Remove-AzureRmServiceFabricSettings       Remover uma ou mais definições do ServiceFabric de um cluster
    + Set-AzureRmServiceFabricSettings       Adicionar ou atualizar uma ou mais definições do ServiceFabric de um cluster
    + Set-AzureRmServiceFabricUpgradeType       Alterar o tipo de atualização do ServiceFabric de um cluster
    + Update-AzureRmServiceFabricDurability       Alterar o escalão de durabilidade de um cluster
    + Update-AzureRmServiceFabricReliability       Alterar o escalão de fiabilidade de um cluster
* SQL
  - Foi adicionado o parâmetro -SampleName a New-AzureRmSqlDatabase
  - Atualizações dos cmdlets do Grupo de Ativação Pós-falha
  - Remova os parâmetros "Tag"
  - Remova os parâmetros "PartnerResourceGroupName" e "PartnerServerName" do cmdlet Remove-AzureRmSqlDatabaseFailoverGroup
  - Adicione o parâmetro "GracePeriodWithDataLossHours" aos cmdlets New- e Set-, que no fim devem substituir "GracePeriodWithDataLossHour"
  - A documentação foi desenvolvida e atualizada
  - Altere a formatação dos objetos devolvidos e corrija alguns erros onde os campos não foram sempre preenchidos
  - Adicionar as propriedades "DatabaseNames" e "PartnerLocation" ao objeto do Grupo de Ativação Pós-falha
  - Corrija o erro que faz com que o cmdlet Switch- seja devolvido imediatamente, em vez de aguardar a conclusão da operação
  - Corrija o erro de capacidade excedida do número inteiro quando são utilizados valores do período de tolerância elevada
  - Ajuste o período de tolerância para um mínimo de 1 hora se for fornecido um inferior
  - Remova "Usage_Anomaly" dos valores aceites para o parâmetro de "ExcludedDetectionType" do cmdlet Set-AzureRmSqlDatabaseThreatDetectionPolicy e o cmdlet Set-AzureRmSqlServerThreatDetectionPolicy.
* Armazenamento
  - Atualizar SRP SDK para 6.3.0
  - New/Set-AzureRmStorageAccount: adicionar um novo parâmetro para suportar EnableHttpsTrafficOnly
  - New/Set/Get-AzureRmStorageAccount: a conta de armazenamento devolvida contém um novo atributo de EnableHttpsTrafficOnly
* Azure.Storage
  - Atualizar para a Biblioteca de Clientes de Armazenamento do Azure 8.1.1 e Biblioteca do DataMovement de Armazenamento do Azure 0.5.1
  - Adicionar um novo cmdlet para suportar a funcionalidade de Cópia Incremental de blob
