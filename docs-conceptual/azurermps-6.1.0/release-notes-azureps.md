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
# <a name="release-notes"></a><span data-ttu-id="e6d05-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="e6d05-103">Release notes</span></span>

<span data-ttu-id="e6d05-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="e6d05-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="610---may-2018"></a><span data-ttu-id="e6d05-105">6.1.0 - Maio de 2018</span><span class="sxs-lookup"><span data-stu-id="e6d05-105">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="e6d05-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="e6d05-106">AzureRM.Profile</span></span>
* <span data-ttu-id="e6d05-107">Correção do problema em que a execução de "Clear-AzureRmContext" mantinha um contexto vazio com o nome do contexto predefinido anterior, o que impedia o utilizador de criar um novo contexto com o nome antigo</span><span class="sxs-lookup"><span data-stu-id="e6d05-107">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="e6d05-108">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="e6d05-108">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="e6d05-109">Permitir operações de associação/desassociação do Gateway no AS.</span><span class="sxs-lookup"><span data-stu-id="e6d05-109">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="e6d05-110">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="e6d05-110">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="e6d05-111">Foi adicionado suporte para ApiVersions, ApiReleases e ApiRevisions</span><span class="sxs-lookup"><span data-stu-id="e6d05-111">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="e6d05-112">Foi adicionado suporte para o Back-end do ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e6d05-112">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="e6d05-113">Foi adicionado suporte para o Logger do Application Insights</span><span class="sxs-lookup"><span data-stu-id="e6d05-113">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="e6d05-114">Foi adicionado suporte para reconhecer o SKU "Básico" como um SKU válido do serviço Gestão de API</span><span class="sxs-lookup"><span data-stu-id="e6d05-114">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="e6d05-115">Foi adicionado suporte para instalar Certificados emitidos por AC privadas como Raiz ou AC</span><span class="sxs-lookup"><span data-stu-id="e6d05-115">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="e6d05-116">Foi adicionado suporte para aceitar Certificados SSL personalizados através do KeyVault e de vários nomes de anfitrião de proxy</span><span class="sxs-lookup"><span data-stu-id="e6d05-116">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="e6d05-117">Foi adicionado suporte para a identidade MSI</span><span class="sxs-lookup"><span data-stu-id="e6d05-117">Added support for MSI identity</span></span>
* <span data-ttu-id="e6d05-118">Foi adicionado suporte para aceitar políticas através de Url. NOTA: Os cmdlets seguintes serão preteridos numa versão futura</span><span class="sxs-lookup"><span data-stu-id="e6d05-118">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="e6d05-119">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="e6d05-119">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="e6d05-120">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="e6d05-120">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="e6d05-121">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="e6d05-121">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="e6d05-122">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="e6d05-122">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="e6d05-123">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="e6d05-123">AzureRM.Batch</span></span>
* <span data-ttu-id="e6d05-124">Lançamento do novo cmdlet Get-AzureBatchPoolNodeCounts</span><span class="sxs-lookup"><span data-stu-id="e6d05-124">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="e6d05-125">Lançamento do novo cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span><span class="sxs-lookup"><span data-stu-id="e6d05-125">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="e6d05-126">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="e6d05-126">AzureRM.Consumption</span></span>
* <span data-ttu-id="e6d05-127">Adição dos novos parâmetros Expand, ResourceGroup, InstanceName, InstanceId, Tags e Top no Cmdlet Get-AzureRmConsumptionUsageDetail</span><span class="sxs-lookup"><span data-stu-id="e6d05-127">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="e6d05-128">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e6d05-128">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="e6d05-129">Correção do exemplo de Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="e6d05-129">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="e6d05-130">Correção da exceção do parâmetro nulo do caso Recursivo em Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="e6d05-130">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="e6d05-131">Correção dos ficheiros de ajuda de Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="e6d05-131">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="e6d05-132">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="e6d05-132">AzureRM.Network</span></span>
* <span data-ttu-id="e6d05-133">Aumento da versão do SDK de Rede de 18.0.0-preview para 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="e6d05-133">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="e6d05-134">Foi adicionado um cmdlet para criar a configuração de protocolo</span><span class="sxs-lookup"><span data-stu-id="e6d05-134">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="e6d05-135">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="e6d05-135">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="e6d05-136">Foi adicionado um cmdlet para adicionar uma nova ligação de circuito a um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="e6d05-136">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="e6d05-137">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="e6d05-137">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="e6d05-138">Foi adicionado um cmdlet para remover uma ligação de circuito de um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="e6d05-138">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="e6d05-139">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="e6d05-139">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="e6d05-140">Foi adicionado um cmdlet para obter uma ligação de circuito</span><span class="sxs-lookup"><span data-stu-id="e6d05-140">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="e6d05-141">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="e6d05-141">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="e6d05-142">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e6d05-142">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="e6d05-143">Correção da utilização da autenticação de servidor com certificados gerados (Problema #5998)</span><span class="sxs-lookup"><span data-stu-id="e6d05-143">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="e6d05-144">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="e6d05-144">AzureRM.Sql</span></span>
* <span data-ttu-id="e6d05-145">Atualização dos cmdlets de Auditoria para permitir a remoção de AuditActions ou AuditActionGroups</span><span class="sxs-lookup"><span data-stu-id="e6d05-145">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="e6d05-146">Correção do problema de Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy ao definir uma nova política de retenção flexível em que o comando falhava com "Configurar a política de retenção de longo-prazo com o cofre e a política do serviço de recuperação do Azure já não é suportado.</span><span class="sxs-lookup"><span data-stu-id="e6d05-146">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="e6d05-147">Submeta um pedido com a nova política de retenção flexível".</span><span class="sxs-lookup"><span data-stu-id="e6d05-147">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="e6d05-148">Atualize todos os cmdlets relacionados com as Bases de Dados SQL do Azure/Criação de Conjuntos Elásticos/Atualização para utilizar a nova API de Base de Dados, que suporta a propriedade SKU para propriedades relacionadas com dimensionamento e escalão.</span><span class="sxs-lookup"><span data-stu-id="e6d05-148">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="e6d05-149">Os cmdlets atualizados, incluindo:</span><span class="sxs-lookup"><span data-stu-id="e6d05-149">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="e6d05-150">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="e6d05-150">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="e6d05-151">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="e6d05-151">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="e6d05-152">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="e6d05-152">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="e6d05-153">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="e6d05-153">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="e6d05-154">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="e6d05-154">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="e6d05-155">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="e6d05-155">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="e6d05-156">Atualize os parâmetros de "Get-AzureRmTrafficManagerProfile" para que o parâmetro -ResourceGroupName seja necessário ao utilizar o parâmetro -Name.</span><span class="sxs-lookup"><span data-stu-id="e6d05-156">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>