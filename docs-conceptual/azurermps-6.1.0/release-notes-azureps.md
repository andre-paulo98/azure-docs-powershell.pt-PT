---
title: Registo de alterações do Azure PowerShell | Microsoft Docs
description: Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente.
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 5/1/2018
ms.openlocfilehash: 0b7902155c47f2e6355e9147c203867288caab81
ms.sourcegitcommit: 5971c92cb023bdd1d71fa2ad0a3b378abfbd092a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/23/2018
ms.locfileid: "34461900"
---
# <a name="release-notes"></a>Notas de versão

Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.

---
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