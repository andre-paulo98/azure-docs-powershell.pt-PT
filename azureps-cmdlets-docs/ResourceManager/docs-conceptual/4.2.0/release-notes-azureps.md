---
title: "Registo de alterações do Azure PowerShell | Microsoft Docs"
description: "Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente."
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-resource-manager
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: 
ms.date: 05/18/2017
ms.openlocfilehash: 5c8fa2a5a8f94cd24b66f42c237749a7b89af3b3
ms.sourcegitcommit: ec0b3565264ff7c9f03315ded182f3d5cce534fc
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/13/2017
---
# <a name="release-notes"></a>Notas de versão

Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.

## <a name="version-400"></a>Versão 4.0.0

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
  - Os cmdlets que entraram em conflito com os cmdlets RDFE foram alterados no nome. Ver o problema https://github.com/Azure/azure-powershell/issues/2917 para obter mais detalhes
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
