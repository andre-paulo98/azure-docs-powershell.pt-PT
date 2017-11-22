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
ms.date: 11/14/2017
ms.openlocfilehash: ab35cbc4ec1a0bd4e7ee40e1864bd7941f5bca87
ms.sourcegitcommit: 79dd3700b5cb4cb90b268778b482082052160093
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/14/2017
---
# <a name="release-notes"></a>Notas de versão

Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.

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