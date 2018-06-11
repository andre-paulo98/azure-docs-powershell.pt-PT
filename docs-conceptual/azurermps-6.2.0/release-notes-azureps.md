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
ms.date: 5/1/2018
ms.openlocfilehash: f90c77d8c9cd78315264fb0a0a58e047aefc5041
ms.sourcegitcommit: 2eea03b7ac19ad6d7c8097743d33c7ddb9c4df77
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/06/2018
ms.locfileid: "34821875"
---
# <a name="release-notes"></a><span data-ttu-id="4a9fb-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="4a9fb-103">Release notes</span></span>

<span data-ttu-id="4a9fb-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="4a9fb-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="620---june-2018"></a><span data-ttu-id="4a9fb-105">6.2.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="4a9fb-105">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="4a9fb-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="4a9fb-106">AzureRM.Profile</span></span>
* <span data-ttu-id="4a9fb-107">Corrija o problema onde a versão 10.0.3 de Newtonsoft.Json não foi carregada na importação do módulo</span><span class="sxs-lookup"><span data-stu-id="4a9fb-107">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="4a9fb-108">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="4a9fb-108">AzureRM.Compute</span></span>
* <span data-ttu-id="4a9fb-109">Funcionalidade Atualização da VM VMSS</span><span class="sxs-lookup"><span data-stu-id="4a9fb-109">VMSS VM Update feature</span></span>
    - <span data-ttu-id="4a9fb-110">Cmdlets "Update-AzureRmVmssVM" e "New-AzureRmVMDataDisk" adicionados</span><span class="sxs-lookup"><span data-stu-id="4a9fb-110">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="4a9fb-111">Adicione o parâmetro VirtualMachineScaleSetVM ao cmdlet "Add-AzureRmVMDataDisk" para suportar a adição de um disco de dados à VM Vmss.</span><span class="sxs-lookup"><span data-stu-id="4a9fb-111">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="4a9fb-112">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="4a9fb-112">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="4a9fb-113">O SDK de .Net do ADF foi atualizado para a versão 0.8.0-preview que contém as seguintes alterações:</span><span class="sxs-lookup"><span data-stu-id="4a9fb-113">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="4a9fb-114">Foi adicionada a operação de Configuração de fábrica do repositório</span><span class="sxs-lookup"><span data-stu-id="4a9fb-114">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="4a9fb-115">QuickBooks LinkedService atualizado para expor as propriedades consumerKey e consumerSecret</span><span class="sxs-lookup"><span data-stu-id="4a9fb-115">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="4a9fb-116">Vários tipos de modelos Atualizados de SecretBase para Object</span><span class="sxs-lookup"><span data-stu-id="4a9fb-116">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="4a9fb-117">Acionador de Eventos de Blob adicionado</span><span class="sxs-lookup"><span data-stu-id="4a9fb-117">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="4a9fb-118">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="4a9fb-118">AzureRM.KeyVault</span></span>
* <span data-ttu-id="4a9fb-119">Documentação de atualização com resultado de exemplo</span><span class="sxs-lookup"><span data-stu-id="4a9fb-119">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="4a9fb-120">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="4a9fb-120">AzureRM.Network</span></span>
* <span data-ttu-id="4a9fb-121">Ativar parâmetros da Análise de Tráfego em cmdlets do Observador de Rede</span><span class="sxs-lookup"><span data-stu-id="4a9fb-121">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="4a9fb-122">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="4a9fb-122">AzureRM.Resources</span></span>
* <span data-ttu-id="4a9fb-123">Corrija o problema com a propriedade "Propriedades" do(s) objeto(s) "PSResource" devolvidos por "Get-AzureRmResource"</span><span class="sxs-lookup"><span data-stu-id="4a9fb-123">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="4a9fb-124">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="4a9fb-124">AzureRM.Scheduler</span></span>
* <span data-ttu-id="4a9fb-125">Corrija o problema com a atualização ServiceBusQueueJob sem definir novos valores de Autenticação</span><span class="sxs-lookup"><span data-stu-id="4a9fb-125">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="4a9fb-126">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="4a9fb-126">AzureRM.Sql</span></span>
* <span data-ttu-id="4a9fb-127">Cmdlets seguintes atualizados com parâmetro opcional LicenseType</span><span class="sxs-lookup"><span data-stu-id="4a9fb-127">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="4a9fb-128">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="4a9fb-128">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="4a9fb-129">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="4a9fb-129">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="4a9fb-130">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="4a9fb-130">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="4a9fb-131">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="4a9fb-131">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="4a9fb-132">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="4a9fb-132">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="4a9fb-133">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="4a9fb-133">AzureRM.Websites</span></span>
* <span data-ttu-id="4a9fb-134">"New-AzureRMWebApp" está atualizado para utilizar algoritmos comuns da biblioteca Estratégia.</span><span class="sxs-lookup"><span data-stu-id="4a9fb-134">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="4a9fb-135">6.1.0 - Maio de 2018</span><span class="sxs-lookup"><span data-stu-id="4a9fb-135">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="4a9fb-136">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="4a9fb-136">AzureRM.Profile</span></span>
* <span data-ttu-id="4a9fb-137">Correção do problema em que a execução de "Clear-AzureRmContext" mantinha um contexto vazio com o nome do contexto predefinido anterior, o que impedia o utilizador de criar um novo contexto com o nome antigo</span><span class="sxs-lookup"><span data-stu-id="4a9fb-137">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="4a9fb-138">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="4a9fb-138">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="4a9fb-139">Permitir operações de associação/desassociação do Gateway no AS.</span><span class="sxs-lookup"><span data-stu-id="4a9fb-139">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="4a9fb-140">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="4a9fb-140">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="4a9fb-141">Foi adicionado suporte para ApiVersions, ApiReleases e ApiRevisions</span><span class="sxs-lookup"><span data-stu-id="4a9fb-141">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="4a9fb-142">Foi adicionado suporte para o Back-end do ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="4a9fb-142">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="4a9fb-143">Foi adicionado suporte para o Logger do Application Insights</span><span class="sxs-lookup"><span data-stu-id="4a9fb-143">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="4a9fb-144">Foi adicionado suporte para reconhecer o SKU "Básico" como um SKU válido do serviço Gestão de API</span><span class="sxs-lookup"><span data-stu-id="4a9fb-144">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="4a9fb-145">Foi adicionado suporte para instalar Certificados emitidos por AC privadas como Raiz ou AC</span><span class="sxs-lookup"><span data-stu-id="4a9fb-145">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="4a9fb-146">Foi adicionado suporte para aceitar Certificados SSL personalizados através do KeyVault e de vários nomes de anfitrião de proxy</span><span class="sxs-lookup"><span data-stu-id="4a9fb-146">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="4a9fb-147">Foi adicionado suporte para a identidade MSI</span><span class="sxs-lookup"><span data-stu-id="4a9fb-147">Added support for MSI identity</span></span>
* <span data-ttu-id="4a9fb-148">Foi adicionado suporte para aceitar políticas através de Url. NOTA: Os cmdlets seguintes serão preteridos numa versão futura</span><span class="sxs-lookup"><span data-stu-id="4a9fb-148">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="4a9fb-149">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="4a9fb-149">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="4a9fb-150">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="4a9fb-150">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="4a9fb-151">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="4a9fb-151">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="4a9fb-152">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="4a9fb-152">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="4a9fb-153">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="4a9fb-153">AzureRM.Batch</span></span>
* <span data-ttu-id="4a9fb-154">Lançamento do novo cmdlet Get-AzureBatchPoolNodeCounts</span><span class="sxs-lookup"><span data-stu-id="4a9fb-154">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="4a9fb-155">Lançamento do novo cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span><span class="sxs-lookup"><span data-stu-id="4a9fb-155">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="4a9fb-156">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="4a9fb-156">AzureRM.Consumption</span></span>
* <span data-ttu-id="4a9fb-157">Adição dos novos parâmetros Expand, ResourceGroup, InstanceName, InstanceId, Tags e Top no Cmdlet Get-AzureRmConsumptionUsageDetail</span><span class="sxs-lookup"><span data-stu-id="4a9fb-157">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="4a9fb-158">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="4a9fb-158">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="4a9fb-159">Correção do exemplo de Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="4a9fb-159">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="4a9fb-160">Correção da exceção do parâmetro nulo do caso Recursivo em Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="4a9fb-160">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="4a9fb-161">Correção dos ficheiros de ajuda de Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="4a9fb-161">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="4a9fb-162">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="4a9fb-162">AzureRM.Network</span></span>
* <span data-ttu-id="4a9fb-163">Aumento da versão do SDK de Rede de 18.0.0-preview para 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="4a9fb-163">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="4a9fb-164">Foi adicionado um cmdlet para criar a configuração de protocolo</span><span class="sxs-lookup"><span data-stu-id="4a9fb-164">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="4a9fb-165">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="4a9fb-165">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="4a9fb-166">Foi adicionado um cmdlet para adicionar uma nova ligação de circuito a um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="4a9fb-166">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="4a9fb-167">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="4a9fb-167">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="4a9fb-168">Foi adicionado um cmdlet para remover uma ligação de circuito de um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="4a9fb-168">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="4a9fb-169">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="4a9fb-169">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="4a9fb-170">Foi adicionado um cmdlet para obter uma ligação de circuito</span><span class="sxs-lookup"><span data-stu-id="4a9fb-170">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="4a9fb-171">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="4a9fb-171">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="4a9fb-172">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="4a9fb-172">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="4a9fb-173">Correção da utilização da autenticação de servidor com certificados gerados (Problema #5998)</span><span class="sxs-lookup"><span data-stu-id="4a9fb-173">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="4a9fb-174">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="4a9fb-174">AzureRM.Sql</span></span>
* <span data-ttu-id="4a9fb-175">Atualização dos cmdlets de Auditoria para permitir a remoção de AuditActions ou AuditActionGroups</span><span class="sxs-lookup"><span data-stu-id="4a9fb-175">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="4a9fb-176">Correção do problema de Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy ao definir uma nova política de retenção flexível em que o comando falhava com "Configurar a política de retenção de longo-prazo com o cofre e a política do serviço de recuperação do Azure já não é suportado.</span><span class="sxs-lookup"><span data-stu-id="4a9fb-176">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="4a9fb-177">Submeta um pedido com a nova política de retenção flexível".</span><span class="sxs-lookup"><span data-stu-id="4a9fb-177">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="4a9fb-178">Atualize todos os cmdlets relacionados com as Bases de Dados SQL do Azure/Criação de Conjuntos Elásticos/Atualização para utilizar a nova API de Base de Dados, que suporta a propriedade SKU para propriedades relacionadas com dimensionamento e escalão.</span><span class="sxs-lookup"><span data-stu-id="4a9fb-178">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="4a9fb-179">Os cmdlets atualizados, incluindo:</span><span class="sxs-lookup"><span data-stu-id="4a9fb-179">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="4a9fb-180">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="4a9fb-180">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="4a9fb-181">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="4a9fb-181">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="4a9fb-182">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="4a9fb-182">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="4a9fb-183">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="4a9fb-183">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="4a9fb-184">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="4a9fb-184">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="4a9fb-185">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="4a9fb-185">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="4a9fb-186">Atualize os parâmetros de "Get-AzureRmTrafficManagerProfile" para que o parâmetro -ResourceGroupName seja necessário ao utilizar o parâmetro -Name.</span><span class="sxs-lookup"><span data-stu-id="4a9fb-186">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>