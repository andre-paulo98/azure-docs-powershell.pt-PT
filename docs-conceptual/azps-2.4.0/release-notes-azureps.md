---
ms.openlocfilehash: f357a17f698d68c1a29dcb78f83671973fd6ecad
ms.sourcegitcommit: 0b644bfecf4224b2ea83520d1a6a956734d9fba4
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/12/2019
ms.locfileid: "67863728"
---
## <a name="240---july-2019"></a><span data-ttu-id="bfa42-101">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="bfa42-101">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="bfa42-102">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="bfa42-102">Az.Accounts</span></span>
* <span data-ttu-id="bfa42-103">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="bfa42-103">Add support for profile cmdlets</span></span>
* <span data-ttu-id="bfa42-104">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="bfa42-104">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="bfa42-105">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="bfa42-105">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="bfa42-106">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="bfa42-106">Az.Advisor</span></span>
* <span data-ttu-id="bfa42-107">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="bfa42-107">GA release of Az.Advisor</span></span>
* <span data-ttu-id="bfa42-108">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="bfa42-108">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="bfa42-109">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="bfa42-109">Az.ApiManagement</span></span>
* <span data-ttu-id="bfa42-110">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="bfa42-110">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="bfa42-111">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="bfa42-111">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="bfa42-112">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="bfa42-112">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="bfa42-113">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="bfa42-113">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="bfa42-114">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="bfa42-114">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="bfa42-115">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="bfa42-115">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="bfa42-116">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="bfa42-116">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="bfa42-117">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="bfa42-117">Az.Automation</span></span>
* <span data-ttu-id="bfa42-118">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="bfa42-118">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="bfa42-119">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="bfa42-119">Az.Compute</span></span>
* <span data-ttu-id="bfa42-120">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="bfa42-120">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="bfa42-121">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="bfa42-121">Az.DataFactory</span></span>
* <span data-ttu-id="bfa42-122">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="bfa42-122">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="bfa42-123">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="bfa42-123">Az.EventGrid</span></span>
* <span data-ttu-id="bfa42-124">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="bfa42-124">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="bfa42-125">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="bfa42-125">Az.IotHub</span></span>
* <span data-ttu-id="bfa42-126">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="bfa42-126">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="bfa42-127">Az.Network</span><span class="sxs-lookup"><span data-stu-id="bfa42-127">Az.Network</span></span>
* <span data-ttu-id="bfa42-128">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="bfa42-128">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="bfa42-129">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="bfa42-129">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="bfa42-130">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="bfa42-130">Az.PolicyInsights</span></span>
* <span data-ttu-id="bfa42-131">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="bfa42-131">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="bfa42-132">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="bfa42-132">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="bfa42-133">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="bfa42-133">Az.OperationalInsights</span></span>
* <span data-ttu-id="bfa42-134">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="bfa42-134">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="bfa42-135">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="bfa42-135">Az.RecoveryServices</span></span>
* <span data-ttu-id="bfa42-136">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="bfa42-136">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="bfa42-137">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="bfa42-137">Az.Resources</span></span>
    - <span data-ttu-id="bfa42-138">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="bfa42-138">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="bfa42-139">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="bfa42-139">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="bfa42-140">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="bfa42-140">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="bfa42-141">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="bfa42-141">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="bfa42-142">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="bfa42-142">Az.ServiceBus</span></span>
* <span data-ttu-id="bfa42-143">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="bfa42-143">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="bfa42-144">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="bfa42-144">Az.Sql</span></span>
* <span data-ttu-id="bfa42-145">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="bfa42-145">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="bfa42-146">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="bfa42-146">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="bfa42-147">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="bfa42-147">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="bfa42-148">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="bfa42-148">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="bfa42-149">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="bfa42-149">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="bfa42-150">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="bfa42-150">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="bfa42-151">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="bfa42-151">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="bfa42-152">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="bfa42-152">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="bfa42-153">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="bfa42-153">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="bfa42-154">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="bfa42-154">Az.Storage</span></span>
* <span data-ttu-id="bfa42-155">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="bfa42-155">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="bfa42-156">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="bfa42-156">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="bfa42-157">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="bfa42-157">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="bfa42-158">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="bfa42-158">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="bfa42-159">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="bfa42-159">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="bfa42-160">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="bfa42-160">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="bfa42-161">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="bfa42-161">Set-AzStorageAccount</span></span>
* <span data-ttu-id="bfa42-162">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="bfa42-162">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="bfa42-163">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="bfa42-163">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="bfa42-164">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="bfa42-164">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="bfa42-165">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="bfa42-165">Az.StorageSync</span></span>
* <span data-ttu-id="bfa42-166">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="bfa42-166">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="bfa42-167">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="bfa42-167">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="bfa42-168">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="bfa42-168">Az.Accounts</span></span>
* <span data-ttu-id="bfa42-169">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="bfa42-169">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="bfa42-170">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="bfa42-170">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="bfa42-171">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="bfa42-171">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="bfa42-172">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="bfa42-172">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="bfa42-173">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="bfa42-173">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="bfa42-174">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="bfa42-174">Az.Compute</span></span>
* <span data-ttu-id="bfa42-175">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="bfa42-175">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="bfa42-176">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="bfa42-176">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="bfa42-177">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="bfa42-177">Az.Dns</span></span>
* <span data-ttu-id="bfa42-178">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="bfa42-178">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="bfa42-179">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="bfa42-179">Az.EventGrid</span></span>
* <span data-ttu-id="bfa42-180">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="bfa42-180">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="bfa42-181">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="bfa42-181">New cmdlets:</span></span>
    - <span data-ttu-id="bfa42-182">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="bfa42-182">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="bfa42-183">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="bfa42-183">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="bfa42-184">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="bfa42-184">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="bfa42-185">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="bfa42-185">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="bfa42-186">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="bfa42-186">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="bfa42-187">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="bfa42-187">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="bfa42-188">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="bfa42-188">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="bfa42-189">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="bfa42-189">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="bfa42-190">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="bfa42-190">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="bfa42-191">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="bfa42-191">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="bfa42-192">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="bfa42-192">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="bfa42-193">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="bfa42-193">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="bfa42-194">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="bfa42-194">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="bfa42-195">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="bfa42-195">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="bfa42-196">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="bfa42-196">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="bfa42-197">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="bfa42-197">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="bfa42-198">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="bfa42-198">Updated cmdlets:</span></span>
    - <span data-ttu-id="bfa42-199">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="bfa42-199">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="bfa42-200">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="bfa42-200">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="bfa42-201">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="bfa42-201">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="bfa42-202">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="bfa42-202">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="bfa42-203">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="bfa42-203">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="bfa42-204">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="bfa42-204">Event subscription expiration date,</span></span>
            - <span data-ttu-id="bfa42-205">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="bfa42-205">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="bfa42-206">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="bfa42-206">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="bfa42-207">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="bfa42-207">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="bfa42-208">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="bfa42-208">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="bfa42-209">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="bfa42-209">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="bfa42-210">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="bfa42-210">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="bfa42-211">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="bfa42-211">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="bfa42-212">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="bfa42-212">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="bfa42-213">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="bfa42-213">Az.FrontDoor</span></span>
* <span data-ttu-id="bfa42-214">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="bfa42-214">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="bfa42-215">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="bfa42-215">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="bfa42-216">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="bfa42-216">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="bfa42-217">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="bfa42-217">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="bfa42-218">Az.Network</span><span class="sxs-lookup"><span data-stu-id="bfa42-218">Az.Network</span></span>
* <span data-ttu-id="bfa42-219">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="bfa42-219">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="bfa42-220">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="bfa42-220">New cmdlets</span></span>
        - <span data-ttu-id="bfa42-221">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="bfa42-221">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="bfa42-222">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="bfa42-222">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="bfa42-223">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="bfa42-223">New cmdlets</span></span> 
        - <span data-ttu-id="bfa42-224">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="bfa42-224">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="bfa42-225">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="bfa42-225">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="bfa42-226">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="bfa42-226">New cmdlets</span></span> 
        - <span data-ttu-id="bfa42-227">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="bfa42-227">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="bfa42-228">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="bfa42-228">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="bfa42-229">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="bfa42-229">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="bfa42-230">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="bfa42-230">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="bfa42-231">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="bfa42-231">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="bfa42-232">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="bfa42-232">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="bfa42-233">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="bfa42-233">New cmdlets</span></span>
        - <span data-ttu-id="bfa42-234">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="bfa42-234">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="bfa42-235">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="bfa42-235">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="bfa42-236">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="bfa42-236">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="bfa42-237">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="bfa42-237">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="bfa42-238">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="bfa42-238">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="bfa42-239">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="bfa42-239">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="bfa42-240">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="bfa42-240">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="bfa42-241">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="bfa42-241">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="bfa42-242">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="bfa42-242">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="bfa42-243">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="bfa42-243">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="bfa42-244">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="bfa42-244">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="bfa42-245">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="bfa42-245">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="bfa42-246">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="bfa42-246">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="bfa42-247">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="bfa42-247">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="bfa42-248">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="bfa42-248">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="bfa42-249">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="bfa42-249">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="bfa42-250">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="bfa42-250">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="bfa42-251">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="bfa42-251">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="bfa42-252">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="bfa42-252">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="bfa42-253">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="bfa42-253">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="bfa42-254">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="bfa42-254">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="bfa42-255">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="bfa42-255">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="bfa42-256">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="bfa42-256">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="bfa42-257">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="bfa42-257">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="bfa42-258">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="bfa42-258">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="bfa42-259">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="bfa42-259">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="bfa42-260">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="bfa42-260">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="bfa42-261">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="bfa42-261">Az.OperationalInsights</span></span>
* <span data-ttu-id="bfa42-262">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="bfa42-262">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="bfa42-263">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="bfa42-263">Az.Resources</span></span>
* <span data-ttu-id="bfa42-264">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="bfa42-264">Support for additional Template Export options</span></span>
    - <span data-ttu-id="bfa42-265">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="bfa42-265">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="bfa42-266">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="bfa42-266">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="bfa42-267">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="bfa42-267">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="bfa42-268">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="bfa42-268">Az.ServiceFabric</span></span>
* <span data-ttu-id="bfa42-269">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="bfa42-269">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="bfa42-270">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="bfa42-270">Az.Sql</span></span>
* <span data-ttu-id="bfa42-271">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="bfa42-271">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="bfa42-272">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="bfa42-272">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="bfa42-273">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="bfa42-273">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="bfa42-274">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="bfa42-274">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="bfa42-275">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="bfa42-275">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="bfa42-276">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="bfa42-276">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="bfa42-277">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="bfa42-277">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="bfa42-278">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="bfa42-278">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="bfa42-279">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="bfa42-279">Az.Storage</span></span>
* <span data-ttu-id="bfa42-280">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="bfa42-280">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="bfa42-281">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="bfa42-281">New-AzStorageAccount</span></span>
* <span data-ttu-id="bfa42-282">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="bfa42-282">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="bfa42-283">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="bfa42-283">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="bfa42-284">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="bfa42-284">Az.Websites</span></span>
* <span data-ttu-id="bfa42-285">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="bfa42-285">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="bfa42-286">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="bfa42-286">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="bfa42-287">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="bfa42-287">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="bfa42-288">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="bfa42-288">Az.Cdn</span></span>
* <span data-ttu-id="bfa42-289">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="bfa42-289">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="bfa42-290">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="bfa42-290">Az.Compute</span></span>
* <span data-ttu-id="bfa42-291">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="bfa42-291">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="bfa42-292">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="bfa42-292">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="bfa42-293">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="bfa42-293">Az.EventHub</span></span>
* <span data-ttu-id="bfa42-294">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="bfa42-294">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="bfa42-295">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="bfa42-295">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="bfa42-296">Az.Network</span><span class="sxs-lookup"><span data-stu-id="bfa42-296">Az.Network</span></span>
* <span data-ttu-id="bfa42-297">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="bfa42-297">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="bfa42-298">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="bfa42-298">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="bfa42-299">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="bfa42-299">Az.PolicyInsights</span></span>
* <span data-ttu-id="bfa42-300">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="bfa42-300">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="bfa42-301">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="bfa42-301">Az.RecoveryServices</span></span>
* <span data-ttu-id="bfa42-302">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="bfa42-302">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="bfa42-303">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="bfa42-303">Az.ServiceBus</span></span>
* <span data-ttu-id="bfa42-304">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="bfa42-304">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="bfa42-305">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="bfa42-305">Az.ServiceFabric</span></span>
* <span data-ttu-id="bfa42-306">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="bfa42-306">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="bfa42-307">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="bfa42-307">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="bfa42-308">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="bfa42-308">Az.Sql</span></span>
* <span data-ttu-id="bfa42-309">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="bfa42-309">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="bfa42-310">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="bfa42-310">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="bfa42-311">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="bfa42-311">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="bfa42-312">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="bfa42-312">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="bfa42-313">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="bfa42-313">Az.Websites</span></span>
* <span data-ttu-id="bfa42-314">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="bfa42-314">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="bfa42-315">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="bfa42-315">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="bfa42-316">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="bfa42-316">Az.ApiManagement</span></span>
* <span data-ttu-id="bfa42-317">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="bfa42-317">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="bfa42-318">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="bfa42-318">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="bfa42-319">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="bfa42-319">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="bfa42-320">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="bfa42-320">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="bfa42-321">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="bfa42-321">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="bfa42-322">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="bfa42-322">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="bfa42-323">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="bfa42-323">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="bfa42-324">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="bfa42-324">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="bfa42-325">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="bfa42-325">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="bfa42-326">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="bfa42-326">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="bfa42-327">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="bfa42-327">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="bfa42-328">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="bfa42-328">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="bfa42-329">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="bfa42-329">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="bfa42-330">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="bfa42-330">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="bfa42-331">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="bfa42-331">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="bfa42-332">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="bfa42-332">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="bfa42-333">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="bfa42-333">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="bfa42-334">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="bfa42-334">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="bfa42-335">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="bfa42-335">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="bfa42-336">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="bfa42-336">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="bfa42-337">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="bfa42-337">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="bfa42-338">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="bfa42-338">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="bfa42-339">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="bfa42-339">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="bfa42-340">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="bfa42-340">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="bfa42-341">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="bfa42-341">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="bfa42-342">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="bfa42-342">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="bfa42-343">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="bfa42-343">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="bfa42-344">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="bfa42-344">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="bfa42-345">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="bfa42-345">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="bfa42-346">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="bfa42-346">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="bfa42-347">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="bfa42-347">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="bfa42-348">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="bfa42-348">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="bfa42-349">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="bfa42-349">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="bfa42-350">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="bfa42-350">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="bfa42-351">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="bfa42-351">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="bfa42-352">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="bfa42-352">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="bfa42-353">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="bfa42-353">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="bfa42-354">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="bfa42-354">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="bfa42-355">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="bfa42-355">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="bfa42-356">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="bfa42-356">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="bfa42-357">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="bfa42-357">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="bfa42-358">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="bfa42-358">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="bfa42-359">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="bfa42-359">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="bfa42-360">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="bfa42-360">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="bfa42-361">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="bfa42-361">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="bfa42-362">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="bfa42-362">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="bfa42-363">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="bfa42-363">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="bfa42-364">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="bfa42-364">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="bfa42-365">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="bfa42-365">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="bfa42-366">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="bfa42-366">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="bfa42-367">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="bfa42-367">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="bfa42-368">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="bfa42-368">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="bfa42-369">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="bfa42-369">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="bfa42-370">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="bfa42-370">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="bfa42-371">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="bfa42-371">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="bfa42-372">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="bfa42-372">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="bfa42-373">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="bfa42-373">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="bfa42-374">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="bfa42-374">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="bfa42-375">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="bfa42-375">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="bfa42-376">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="bfa42-376">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="bfa42-377">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="bfa42-377">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="bfa42-378">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="bfa42-378">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="bfa42-379">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="bfa42-379">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="bfa42-380">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="bfa42-380">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="bfa42-381">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="bfa42-381">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="bfa42-382">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="bfa42-382">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="bfa42-383">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="bfa42-383">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="bfa42-384">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="bfa42-384">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="bfa42-385">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="bfa42-385">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="bfa42-386">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="bfa42-386">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="bfa42-387">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="bfa42-387">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="bfa42-388">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="bfa42-388">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="bfa42-389">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="bfa42-389">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="bfa42-390">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="bfa42-390">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="bfa42-391">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="bfa42-391">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="bfa42-392">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="bfa42-392">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="bfa42-393">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="bfa42-393">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="bfa42-394">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="bfa42-394">Az.Automation</span></span>
* <span data-ttu-id="bfa42-395">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="bfa42-395">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="bfa42-396">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="bfa42-396">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="bfa42-397">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="bfa42-397">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="bfa42-398">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="bfa42-398">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="bfa42-399">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="bfa42-399">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="bfa42-400">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="bfa42-400">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="bfa42-401">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="bfa42-401">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="bfa42-402">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="bfa42-402">Az.Compute</span></span>
* <span data-ttu-id="bfa42-403">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="bfa42-403">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="bfa42-404">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="bfa42-404">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="bfa42-405">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="bfa42-405">Az.DataLakeStore</span></span>
* <span data-ttu-id="bfa42-406">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="bfa42-406">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="bfa42-407">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="bfa42-407">Az.Monitor</span></span>
* <span data-ttu-id="bfa42-408">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="bfa42-408">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="bfa42-409">Az.Network</span><span class="sxs-lookup"><span data-stu-id="bfa42-409">Az.Network</span></span>
* <span data-ttu-id="bfa42-410">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="bfa42-410">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="bfa42-411">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="bfa42-411">Updated cmdlet:</span></span>
        - <span data-ttu-id="bfa42-412">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="bfa42-412">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="bfa42-413">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="bfa42-413">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="bfa42-414">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="bfa42-414">Az.Resources</span></span>
* <span data-ttu-id="bfa42-415">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="bfa42-415">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="bfa42-416">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="bfa42-416">Az.Sql</span></span>
* <span data-ttu-id="bfa42-417">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="bfa42-417">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="bfa42-418">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="bfa42-418">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="bfa42-419">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="bfa42-419">Az.Accounts</span></span>
* <span data-ttu-id="bfa42-420">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="bfa42-420">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="bfa42-421">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="bfa42-421">Az.CognitiveServices</span></span>
* <span data-ttu-id="bfa42-422">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="bfa42-422">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="bfa42-423">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="bfa42-423">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="bfa42-424">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="bfa42-424">Az.Compute</span></span>
* <span data-ttu-id="bfa42-425">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="bfa42-425">Proximity placement group feature.</span></span>
    - <span data-ttu-id="bfa42-426">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="bfa42-426">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="bfa42-427">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="bfa42-427">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="bfa42-428">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="bfa42-428">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="bfa42-429">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="bfa42-429">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="bfa42-430">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="bfa42-430">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="bfa42-431">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="bfa42-431">Breaking changes</span></span>
    - <span data-ttu-id="bfa42-432">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="bfa42-432">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="bfa42-433">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="bfa42-433">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="bfa42-434">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="bfa42-434">Az.DeploymentManager</span></span>
* <span data-ttu-id="bfa42-435">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="bfa42-435">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="bfa42-436">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="bfa42-436">Az.Dns</span></span>
* <span data-ttu-id="bfa42-437">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="bfa42-437">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="bfa42-438">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="bfa42-438">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="bfa42-439">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="bfa42-439">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="bfa42-440">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="bfa42-440">Az.FrontDoor</span></span>
* <span data-ttu-id="bfa42-441">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="bfa42-441">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="bfa42-442">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="bfa42-442">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="bfa42-443">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="bfa42-443">Az.HDInsight</span></span>
* <span data-ttu-id="bfa42-444">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="bfa42-444">Removed two cmdlets:</span></span>
    - <span data-ttu-id="bfa42-445">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="bfa42-445">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="bfa42-446">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="bfa42-446">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="bfa42-447">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="bfa42-447">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="bfa42-448">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="bfa42-448">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="bfa42-449">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="bfa42-449">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="bfa42-450">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="bfa42-450">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="bfa42-451">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="bfa42-451">Az.Monitor</span></span>
* <span data-ttu-id="bfa42-452">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="bfa42-452">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="bfa42-453">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="bfa42-453">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="bfa42-454">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="bfa42-454">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="bfa42-455">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="bfa42-455">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="bfa42-456">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="bfa42-456">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="bfa42-457">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="bfa42-457">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="bfa42-458">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="bfa42-458">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="bfa42-459">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="bfa42-459">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="bfa42-460">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="bfa42-460">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="bfa42-461">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="bfa42-461">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="bfa42-462">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="bfa42-462">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="bfa42-463">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="bfa42-463">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="bfa42-464">[Mais](https://docs.microsoft.com/en-us/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="bfa42-464">[More](https://docs.microsoft.com/en-us/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="bfa42-465">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="bfa42-465">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="bfa42-466">Az.Network</span><span class="sxs-lookup"><span data-stu-id="bfa42-466">Az.Network</span></span>
* <span data-ttu-id="bfa42-467">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="bfa42-467">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="bfa42-468">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="bfa42-468">New cmdlets</span></span>
        - <span data-ttu-id="bfa42-469">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="bfa42-469">New-AzNatGateway</span></span>
        - <span data-ttu-id="bfa42-470">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="bfa42-470">Get-AzNatGateway</span></span>
        - <span data-ttu-id="bfa42-471">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="bfa42-471">Set-AzNatGateway</span></span>
        - <span data-ttu-id="bfa42-472">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="bfa42-472">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="bfa42-473">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="bfa42-473">Updated cmdlets</span></span>
        - <span data-ttu-id="bfa42-474">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="bfa42-474">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="bfa42-475">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="bfa42-475">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="bfa42-476">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="bfa42-476">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="bfa42-477">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="bfa42-477">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="bfa42-478">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="bfa42-478">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="bfa42-479">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="bfa42-479">Az.PolicyInsights</span></span>
* <span data-ttu-id="bfa42-480">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="bfa42-480">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="bfa42-481">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="bfa42-481">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="bfa42-482">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="bfa42-482">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="bfa42-483">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="bfa42-483">Az.RecoveryServices</span></span>
* <span data-ttu-id="bfa42-484">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="bfa42-484">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="bfa42-485">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="bfa42-485">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="bfa42-486">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="bfa42-486">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="bfa42-487">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="bfa42-487">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="bfa42-488">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="bfa42-488">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="bfa42-489">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="bfa42-489">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="bfa42-490">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="bfa42-490">Az.Relay</span></span>
* <span data-ttu-id="bfa42-491">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="bfa42-491">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="bfa42-492">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="bfa42-492">Az.ServiceBus</span></span>
* <span data-ttu-id="bfa42-493">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="bfa42-493">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="bfa42-494">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="bfa42-494">Az.Storage</span></span>
* <span data-ttu-id="bfa42-495">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="bfa42-495">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="bfa42-496">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="bfa42-496">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="bfa42-497">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="bfa42-497">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="bfa42-498">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="bfa42-498">New-AzStorageAccount</span></span>
* <span data-ttu-id="bfa42-499">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="bfa42-499">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="bfa42-500">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="bfa42-500">New-AzStorageAccount</span></span>
    - <span data-ttu-id="bfa42-501">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="bfa42-501">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="bfa42-502">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="bfa42-502">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="bfa42-503">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="bfa42-503">Az.Websites</span></span>
* <span data-ttu-id="bfa42-504">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="bfa42-504">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="bfa42-505">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="bfa42-505">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="bfa42-506">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="bfa42-506">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="bfa42-507">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="bfa42-507">Highlights since the last major release</span></span>
* <span data-ttu-id="bfa42-508">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="bfa42-508">General availability of `Az` module</span></span>
* <span data-ttu-id="bfa42-509">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="bfa42-509">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="bfa42-510">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="bfa42-510">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="bfa42-511">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="bfa42-511">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="bfa42-512">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="bfa42-512">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="bfa42-513">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="bfa42-513">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="bfa42-514">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="bfa42-514">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="bfa42-515">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="bfa42-515">Az.Accounts</span></span>
* <span data-ttu-id="bfa42-516">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="bfa42-516">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="bfa42-517">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="bfa42-517">Az.Batch</span></span>
* <span data-ttu-id="bfa42-518">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="bfa42-518">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="bfa42-519">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="bfa42-519">Az.Cdn</span></span>
* <span data-ttu-id="bfa42-520">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="bfa42-520">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="bfa42-521">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="bfa42-521">Az.CognitiveServices</span></span>
* <span data-ttu-id="bfa42-522">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="bfa42-522">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="bfa42-523">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="bfa42-523">Az.Compute</span></span>
* <span data-ttu-id="bfa42-524">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="bfa42-524">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="bfa42-525">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="bfa42-525">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="bfa42-526">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="bfa42-526">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="bfa42-527">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="bfa42-527">Az.DataFactory</span></span>
* <span data-ttu-id="bfa42-528">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="bfa42-528">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="bfa42-529">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="bfa42-529">Az.DataLakeStore</span></span>
* <span data-ttu-id="bfa42-530">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="bfa42-530">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="bfa42-531">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="bfa42-531">Az.EventGrid</span></span>
* <span data-ttu-id="bfa42-532">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="bfa42-532">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="bfa42-533">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="bfa42-533">Az.EventHub</span></span>
* <span data-ttu-id="bfa42-534">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="bfa42-534">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="bfa42-535">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="bfa42-535">Az.HDInsight</span></span>
* <span data-ttu-id="bfa42-536">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="bfa42-536">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="bfa42-537">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="bfa42-537">Az.IotHub</span></span>
* <span data-ttu-id="bfa42-538">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="bfa42-538">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="bfa42-539">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="bfa42-539">Az.KeyVault</span></span>
* <span data-ttu-id="bfa42-540">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="bfa42-540">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="bfa42-541">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="bfa42-541">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="bfa42-542">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="bfa42-542">Az.MachineLearning</span></span>
* <span data-ttu-id="bfa42-543">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="bfa42-543">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="bfa42-544">Az.Media</span><span class="sxs-lookup"><span data-stu-id="bfa42-544">Az.Media</span></span>
* <span data-ttu-id="bfa42-545">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="bfa42-545">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="bfa42-546">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="bfa42-546">Az.Monitor</span></span>
  * <span data-ttu-id="bfa42-547">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="bfa42-547">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="bfa42-548">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="bfa42-548">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="bfa42-549">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="bfa42-549">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="bfa42-550">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="bfa42-550">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="bfa42-551">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="bfa42-551">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="bfa42-552">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="bfa42-552">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="bfa42-553">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="bfa42-553">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="bfa42-554">Az.Network</span><span class="sxs-lookup"><span data-stu-id="bfa42-554">Az.Network</span></span>
* <span data-ttu-id="bfa42-555">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="bfa42-555">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="bfa42-556">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="bfa42-556">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="bfa42-557">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="bfa42-557">Az.NotificationHubs</span></span>
* <span data-ttu-id="bfa42-558">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="bfa42-558">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="bfa42-559">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="bfa42-559">Az.OperationalInsights</span></span>
* <span data-ttu-id="bfa42-560">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="bfa42-560">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="bfa42-561">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="bfa42-561">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="bfa42-562">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="bfa42-562">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="bfa42-563">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="bfa42-563">Az.RecoveryServices</span></span>
* <span data-ttu-id="bfa42-564">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="bfa42-564">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="bfa42-565">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="bfa42-565">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="bfa42-566">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="bfa42-566">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="bfa42-567">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="bfa42-567">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="bfa42-568">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="bfa42-568">Az.RedisCache</span></span>
* <span data-ttu-id="bfa42-569">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="bfa42-569">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="bfa42-570">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="bfa42-570">Az.Resources</span></span>
* <span data-ttu-id="bfa42-571">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="bfa42-571">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="bfa42-572">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="bfa42-572">Az.Sql</span></span>
* <span data-ttu-id="bfa42-573">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="bfa42-573">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="bfa42-574">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="bfa42-574">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="bfa42-575">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="bfa42-575">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="bfa42-576">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="bfa42-576">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="bfa42-577">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="bfa42-577">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="bfa42-578">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="bfa42-578">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="bfa42-579">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="bfa42-579">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="bfa42-580">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="bfa42-580">Az.Websites</span></span>
* <span data-ttu-id="bfa42-581">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="bfa42-581">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="bfa42-582">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="bfa42-582">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="bfa42-583">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="bfa42-583">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="bfa42-584">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="bfa42-584">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="bfa42-585">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="bfa42-585">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="bfa42-586">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="bfa42-586">Highlights since the last major release</span></span>
* <span data-ttu-id="bfa42-587">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="bfa42-587">General availability of `Az` module</span></span>
* <span data-ttu-id="bfa42-588">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="bfa42-588">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="bfa42-589">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="bfa42-589">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="bfa42-590">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="bfa42-590">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="bfa42-591">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="bfa42-591">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="bfa42-592">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="bfa42-592">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="bfa42-593">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="bfa42-593">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="bfa42-594">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="bfa42-594">Az.Accounts</span></span>
* <span data-ttu-id="bfa42-595">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="bfa42-595">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="bfa42-596">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="bfa42-596">Az.AnalysisServices</span></span>
* <span data-ttu-id="bfa42-597">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="bfa42-597">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="bfa42-598">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="bfa42-598">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="bfa42-599">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="bfa42-599">Az.Automation</span></span>
* <span data-ttu-id="bfa42-600">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="bfa42-600">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="bfa42-601">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="bfa42-601">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="bfa42-602">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="bfa42-602">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="bfa42-603">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="bfa42-603">Az.Compute</span></span>
* <span data-ttu-id="bfa42-604">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="bfa42-604">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="bfa42-605">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="bfa42-605">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="bfa42-606">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="bfa42-606">Az.ContainerInstance</span></span>
* <span data-ttu-id="bfa42-607">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="bfa42-607">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="bfa42-608">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="bfa42-608">Az.DataFactory</span></span>
* <span data-ttu-id="bfa42-609">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="bfa42-609">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="bfa42-610">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bfa42-610">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="bfa42-611">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="bfa42-611">Az.Resources</span></span>
* <span data-ttu-id="bfa42-612">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="bfa42-612">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="bfa42-613">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="bfa42-613">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="bfa42-614">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="bfa42-614">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="bfa42-615">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="bfa42-615">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="bfa42-616">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="bfa42-616">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="bfa42-617">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="bfa42-617">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="bfa42-618">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="bfa42-618">Az.Sql</span></span>
* <span data-ttu-id="bfa42-619">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="bfa42-619">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="bfa42-620">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="bfa42-620">Az.Storage</span></span>
* <span data-ttu-id="bfa42-621">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="bfa42-621">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="bfa42-622">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="bfa42-622">New-AzStorageContext</span></span>
* <span data-ttu-id="bfa42-623">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="bfa42-623">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="bfa42-624">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="bfa42-624">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="bfa42-625">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="bfa42-625">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="bfa42-626">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="bfa42-626">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="bfa42-627">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="bfa42-627">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="bfa42-628">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="bfa42-628">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="bfa42-629">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="bfa42-629">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="bfa42-630">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="bfa42-630">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="bfa42-631">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="bfa42-631">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="bfa42-632">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="bfa42-632">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="bfa42-633">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="bfa42-633">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="bfa42-634">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="bfa42-634">Highlights since the last major release</span></span>
* <span data-ttu-id="bfa42-635">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="bfa42-635">General availability of `Az` module</span></span>
* <span data-ttu-id="bfa42-636">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="bfa42-636">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="bfa42-637">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="bfa42-637">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="bfa42-638">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="bfa42-638">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="bfa42-639">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="bfa42-639">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="bfa42-640">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="bfa42-640">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="bfa42-641">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="bfa42-641">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="bfa42-642">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="bfa42-642">Az.Automation</span></span>
* <span data-ttu-id="bfa42-643">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="bfa42-643">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="bfa42-644">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="bfa42-644">Dynamic grouping</span></span>
    * <span data-ttu-id="bfa42-645">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="bfa42-645">Pre-Post script</span></span>
    * <span data-ttu-id="bfa42-646">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="bfa42-646">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="bfa42-647">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="bfa42-647">Az.Compute</span></span>
* <span data-ttu-id="bfa42-648">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="bfa42-648">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="bfa42-649">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="bfa42-649">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="bfa42-650">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="bfa42-650">Az.KeyVault</span></span>
* <span data-ttu-id="bfa42-651">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="bfa42-651">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="bfa42-652">Az.Network</span><span class="sxs-lookup"><span data-stu-id="bfa42-652">Az.Network</span></span>
* <span data-ttu-id="bfa42-653">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="bfa42-653">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="bfa42-654">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="bfa42-654">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="bfa42-655">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="bfa42-655">Az.RecoveryServices</span></span>
* <span data-ttu-id="bfa42-656">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="bfa42-656">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="bfa42-657">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="bfa42-657">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="bfa42-658">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="bfa42-658">Az.Resources</span></span>
* <span data-ttu-id="bfa42-659">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="bfa42-659">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="bfa42-660">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="bfa42-660">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="bfa42-661">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="bfa42-661">Az.Sql</span></span>
* <span data-ttu-id="bfa42-662">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="bfa42-662">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="bfa42-663">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="bfa42-663">Az.Storage</span></span>
* <span data-ttu-id="bfa42-664">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="bfa42-664">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="bfa42-665">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="bfa42-665">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="bfa42-666">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="bfa42-666">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="bfa42-667">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="bfa42-667">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="bfa42-668">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="bfa42-668">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="bfa42-669">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="bfa42-669">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="bfa42-670">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="bfa42-670">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="bfa42-671">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="bfa42-671">Az.Websites</span></span>
* <span data-ttu-id="bfa42-672">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="bfa42-672">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="bfa42-673">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="bfa42-673">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="bfa42-674">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="bfa42-674">Az.Accounts</span></span>
* <span data-ttu-id="bfa42-675">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="bfa42-675">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="bfa42-676">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="bfa42-676">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="bfa42-677">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="bfa42-677">Az.Automation</span></span>
* <span data-ttu-id="bfa42-678">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="bfa42-678">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="bfa42-679">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="bfa42-679">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="bfa42-680">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="bfa42-680">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="bfa42-681">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="bfa42-681">Az.Cdn</span></span>
* <span data-ttu-id="bfa42-682">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="bfa42-682">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="bfa42-683">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="bfa42-683">Az.Compute</span></span>
* <span data-ttu-id="bfa42-684">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="bfa42-684">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="bfa42-685">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="bfa42-685">Az.DataFactory</span></span>
* <span data-ttu-id="bfa42-686">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="bfa42-686">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="bfa42-687">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="bfa42-687">Az.LogicApp</span></span>
* <span data-ttu-id="bfa42-688">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="bfa42-688">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="bfa42-689">Az.Network</span><span class="sxs-lookup"><span data-stu-id="bfa42-689">Az.Network</span></span>
* <span data-ttu-id="bfa42-690">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="bfa42-690">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="bfa42-691">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="bfa42-691">Az.RecoveryServices</span></span>
* <span data-ttu-id="bfa42-692">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="bfa42-692">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="bfa42-693">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="bfa42-693">SDK Update</span></span>
* <span data-ttu-id="bfa42-694">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="bfa42-694">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="bfa42-695">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="bfa42-695">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="bfa42-696">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="bfa42-696">Az.Resources</span></span>
* <span data-ttu-id="bfa42-697">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="bfa42-697">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="bfa42-698">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="bfa42-698">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="bfa42-699">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="bfa42-699">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="bfa42-700">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="bfa42-700">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="bfa42-701">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="bfa42-701">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="bfa42-702">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="bfa42-702">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="bfa42-703">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="bfa42-703">Az.Sql</span></span>
* <span data-ttu-id="bfa42-704">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="bfa42-704">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="bfa42-705">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="bfa42-705">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="bfa42-706">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="bfa42-706">Az.Storage</span></span>
* <span data-ttu-id="bfa42-707">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="bfa42-707">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="bfa42-708">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="bfa42-708">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="bfa42-709">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="bfa42-709">Az.AnalysisServices</span></span>
* <span data-ttu-id="bfa42-710">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="bfa42-710">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="bfa42-711">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="bfa42-711">Az.Automation</span></span>
* <span data-ttu-id="bfa42-712">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="bfa42-712">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="bfa42-713">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="bfa42-713">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="bfa42-714">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="bfa42-714">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="bfa42-715">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="bfa42-715">Az.CognitiveServices</span></span>
* <span data-ttu-id="bfa42-716">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="bfa42-716">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="bfa42-717">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="bfa42-717">Az.Compute</span></span>
* <span data-ttu-id="bfa42-718">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="bfa42-718">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="bfa42-719">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="bfa42-719">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="bfa42-720">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="bfa42-720">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="bfa42-721">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="bfa42-721">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="bfa42-722">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="bfa42-722">Az.DataLakeStore</span></span>
* <span data-ttu-id="bfa42-723">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="bfa42-723">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="bfa42-724">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="bfa42-724">Az.EventHub</span></span>
* <span data-ttu-id="bfa42-725">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="bfa42-725">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="bfa42-726">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="bfa42-726">Az.KeyVault</span></span>
* <span data-ttu-id="bfa42-727">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="bfa42-727">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="bfa42-728">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="bfa42-728">Az.LogicApp</span></span>
* <span data-ttu-id="bfa42-729">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="bfa42-729">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="bfa42-730">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="bfa42-730">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="bfa42-731">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="bfa42-731">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="bfa42-732">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="bfa42-732">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="bfa42-733">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="bfa42-733">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="bfa42-734">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="bfa42-734">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="bfa42-735">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="bfa42-735">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="bfa42-736">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="bfa42-736">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="bfa42-737">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="bfa42-737">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="bfa42-738">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="bfa42-738">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="bfa42-739">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="bfa42-739">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="bfa42-740">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="bfa42-740">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="bfa42-741">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="bfa42-741">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="bfa42-742">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="bfa42-742">Az.Monitor</span></span>
* <span data-ttu-id="bfa42-743">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="bfa42-743">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="bfa42-744">Az.Network</span><span class="sxs-lookup"><span data-stu-id="bfa42-744">Az.Network</span></span>
* <span data-ttu-id="bfa42-745">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="bfa42-745">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="bfa42-746">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="bfa42-746">Az.OperationalInsights</span></span>
* <span data-ttu-id="bfa42-747">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="bfa42-747">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="bfa42-748">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="bfa42-748">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="bfa42-749">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="bfa42-749">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="bfa42-750">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="bfa42-750">Az.Resources</span></span>
* <span data-ttu-id="bfa42-751">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="bfa42-751">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="bfa42-752">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="bfa42-752">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="bfa42-753">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="bfa42-753">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="bfa42-754">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="bfa42-754">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="bfa42-755">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="bfa42-755">Az.Sql</span></span>
* <span data-ttu-id="bfa42-756">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="bfa42-756">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="bfa42-757">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="bfa42-757">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="bfa42-758">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="bfa42-758">Az.Websites</span></span>
* <span data-ttu-id="bfa42-759">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="bfa42-759">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="bfa42-760">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="bfa42-760">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="bfa42-761">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="bfa42-761">Az.Accounts</span></span>
* <span data-ttu-id="bfa42-762">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="bfa42-762">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="bfa42-763">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="bfa42-763">Az.AnalysisServices</span></span>
<span data-ttu-id="bfa42-764">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="bfa42-764">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="bfa42-765">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="bfa42-765">Az.Compute</span></span>
* <span data-ttu-id="bfa42-766">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="bfa42-766">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="bfa42-767">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="bfa42-767">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="bfa42-768">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="bfa42-768">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="bfa42-769">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="bfa42-769">Az.RecoveryServices</span></span>
<span data-ttu-id="bfa42-770">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="bfa42-770">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="bfa42-771">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="bfa42-771">Az.Resources</span></span>
* <span data-ttu-id="bfa42-772">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="bfa42-772">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="bfa42-773">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="bfa42-773">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="bfa42-774">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="bfa42-774">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="bfa42-775">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="bfa42-775">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="bfa42-776">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="bfa42-776">Az.Sql</span></span>
* <span data-ttu-id="bfa42-777">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="bfa42-777">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="bfa42-778">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="bfa42-778">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="bfa42-779">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="bfa42-779">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="bfa42-780">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="bfa42-780">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="bfa42-781">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="bfa42-781">Az.Accounts</span></span>
* <span data-ttu-id="bfa42-782">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="bfa42-782">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="bfa42-783">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="bfa42-783">Az.AnalysisServices</span></span>
* <span data-ttu-id="bfa42-784">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="bfa42-784">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="bfa42-785">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="bfa42-785">Az.RecoveryServices</span></span>
* <span data-ttu-id="bfa42-786">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="bfa42-786">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="bfa42-787">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="bfa42-787">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="bfa42-788">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="bfa42-788">Az.Accounts</span></span>
* <span data-ttu-id="bfa42-789">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="bfa42-789">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="bfa42-790">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="bfa42-790">Update incorrect online help URLs</span></span>
* <span data-ttu-id="bfa42-791">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="bfa42-791">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="bfa42-792">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="bfa42-792">Az.Aks</span></span>
* <span data-ttu-id="bfa42-793">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="bfa42-793">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="bfa42-794">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="bfa42-794">Az.Automation</span></span>
* <span data-ttu-id="bfa42-795">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="bfa42-795">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="bfa42-796">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="bfa42-796">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="bfa42-797">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="bfa42-797">Az.Cdn</span></span>
* <span data-ttu-id="bfa42-798">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="bfa42-798">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="bfa42-799">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="bfa42-799">Az.Compute</span></span>
* <span data-ttu-id="bfa42-800">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="bfa42-800">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="bfa42-801">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="bfa42-801">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="bfa42-802">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="bfa42-802">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="bfa42-803">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="bfa42-803">Az.ContainerRegistry</span></span>
* <span data-ttu-id="bfa42-804">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="bfa42-804">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="bfa42-805">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="bfa42-805">Az.DataFactory</span></span>
* <span data-ttu-id="bfa42-806">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="bfa42-806">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="bfa42-807">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="bfa42-807">Az.DataLakeStore</span></span>
* <span data-ttu-id="bfa42-808">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="bfa42-808">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="bfa42-809">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="bfa42-809">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="bfa42-810">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="bfa42-810">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="bfa42-811">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="bfa42-811">Az.IotHub</span></span>
* <span data-ttu-id="bfa42-812">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="bfa42-812">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="bfa42-813">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="bfa42-813">Az.KeyVault</span></span>
* <span data-ttu-id="bfa42-814">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="bfa42-814">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="bfa42-815">Az.Network</span><span class="sxs-lookup"><span data-stu-id="bfa42-815">Az.Network</span></span>
* <span data-ttu-id="bfa42-816">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="bfa42-816">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="bfa42-817">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="bfa42-817">Az.Resources</span></span>
* <span data-ttu-id="bfa42-818">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="bfa42-818">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="bfa42-819">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="bfa42-819">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="bfa42-820">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="bfa42-820">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="bfa42-821">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="bfa42-821">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="bfa42-822">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="bfa42-822">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="bfa42-823">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="bfa42-823">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="bfa42-824">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="bfa42-824">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="bfa42-825">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="bfa42-825">Az.ServiceFabric</span></span>
* <span data-ttu-id="bfa42-826">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="bfa42-826">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="bfa42-827">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="bfa42-827">Fix some error messages.</span></span>
* <span data-ttu-id="bfa42-828">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="bfa42-828">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="bfa42-829">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="bfa42-829">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="bfa42-830">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="bfa42-830">Az.SignalR</span></span>
* <span data-ttu-id="bfa42-831">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="bfa42-831">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="bfa42-832">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="bfa42-832">Az.Sql</span></span>
* <span data-ttu-id="bfa42-833">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="bfa42-833">Update incorrect online help URLs</span></span>
* <span data-ttu-id="bfa42-834">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="bfa42-834">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="bfa42-835">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="bfa42-835">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="bfa42-836">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="bfa42-836">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="bfa42-837">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="bfa42-837">Az.Storage</span></span>
* <span data-ttu-id="bfa42-838">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="bfa42-838">Update incorrect online help URLs</span></span>
* <span data-ttu-id="bfa42-839">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="bfa42-839">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="bfa42-840">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="bfa42-840">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="bfa42-841">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="bfa42-841">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="bfa42-842">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="bfa42-842">Az.TrafficManager</span></span>
* <span data-ttu-id="bfa42-843">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="bfa42-843">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="bfa42-844">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="bfa42-844">Az.Websites</span></span>
* <span data-ttu-id="bfa42-845">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="bfa42-845">Update incorrect online help URLs</span></span>
* <span data-ttu-id="bfa42-846">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="bfa42-846">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="bfa42-847">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="bfa42-847">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="bfa42-848">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="bfa42-848">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="bfa42-849">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="bfa42-849">Az.Accounts</span></span>
* <span data-ttu-id="bfa42-850">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="bfa42-850">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="bfa42-851">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="bfa42-851">Az.Compute</span></span>
* <span data-ttu-id="bfa42-852">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="bfa42-852">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="bfa42-853">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="bfa42-853">Updated the description of ID in help files</span></span>
* <span data-ttu-id="bfa42-854">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="bfa42-854">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="bfa42-855">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="bfa42-855">Az.DataLakeStore</span></span>
* <span data-ttu-id="bfa42-856">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="bfa42-856">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="bfa42-857">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="bfa42-857">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="bfa42-858">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="bfa42-858">Az.EventGrid</span></span>
* <span data-ttu-id="bfa42-859">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="bfa42-859">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="bfa42-860">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="bfa42-860">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="bfa42-861">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="bfa42-861">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="bfa42-862">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="bfa42-862">Event Time-To-Live,</span></span>
        - <span data-ttu-id="bfa42-863">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="bfa42-863">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="bfa42-864">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="bfa42-864">Dead letter endpoint.</span></span>
    - <span data-ttu-id="bfa42-865">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="bfa42-865">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="bfa42-866">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="bfa42-866">Event Time-To-Live,</span></span>
        - <span data-ttu-id="bfa42-867">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="bfa42-867">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="bfa42-868">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="bfa42-868">Dead letter endpoint.</span></span>
* <span data-ttu-id="bfa42-869">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="bfa42-869">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="bfa42-870">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="bfa42-870">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="bfa42-871">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="bfa42-871">Az.IotHub</span></span>
* <span data-ttu-id="bfa42-872">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="bfa42-872">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="bfa42-873">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="bfa42-873">Az.LogicApp</span></span>
* <span data-ttu-id="bfa42-874">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="bfa42-874">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="bfa42-875">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="bfa42-875">Az.Resources</span></span>
* <span data-ttu-id="bfa42-876">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="bfa42-876">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="bfa42-877">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="bfa42-877">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="bfa42-878">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="bfa42-878">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="bfa42-879">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="bfa42-879">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="bfa42-880">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="bfa42-880">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="bfa42-881">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="bfa42-881">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="bfa42-882">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="bfa42-882">Az.SignalR</span></span>
* <span data-ttu-id="bfa42-883">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="bfa42-883">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="bfa42-884">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="bfa42-884">Az.Sql</span></span>
* <span data-ttu-id="bfa42-885">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="bfa42-885">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="bfa42-886">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="bfa42-886">Az.Storage</span></span>
* <span data-ttu-id="bfa42-887">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="bfa42-887">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="bfa42-888">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="bfa42-888">New-AzStorageContext</span></span>
* <span data-ttu-id="bfa42-889">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="bfa42-889">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="bfa42-890">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="bfa42-890">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="bfa42-891">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="bfa42-891">Az.Websites</span></span>
* <span data-ttu-id="bfa42-892">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="bfa42-892">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="bfa42-893">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="bfa42-893">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="bfa42-894">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="bfa42-894">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="bfa42-895">Geral</span><span class="sxs-lookup"><span data-stu-id="bfa42-895">General</span></span>

- <span data-ttu-id="bfa42-896">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="bfa42-896">General Availability of Az Module</span></span>
- <span data-ttu-id="bfa42-897">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="bfa42-897">Online help for each module</span></span>
- <span data-ttu-id="bfa42-898">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="bfa42-898">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="bfa42-899">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="bfa42-899">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="bfa42-900">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="bfa42-900">Az.Accounts</span></span>
- <span data-ttu-id="bfa42-901">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="bfa42-901">Changed from Az.Profile</span></span>
- <span data-ttu-id="bfa42-902">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="bfa42-902">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="bfa42-903">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="bfa42-903">Az.ApiManagement</span></span>
- <span data-ttu-id="bfa42-904">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="bfa42-904">Fixes for #7002</span></span>
- <span data-ttu-id="bfa42-905">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="bfa42-905">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="bfa42-906">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="bfa42-906">Az.Batch</span></span>
- <span data-ttu-id="bfa42-907">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="bfa42-907">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="bfa42-908">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="bfa42-908">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="bfa42-909">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="bfa42-909">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="bfa42-910">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="bfa42-910">Az.Billing</span></span>
- <span data-ttu-id="bfa42-911">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="bfa42-911">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="bfa42-912">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="bfa42-912">Az.CognitivServices</span></span>
- <span data-ttu-id="bfa42-913">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="bfa42-913">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="bfa42-914">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="bfa42-914">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="bfa42-915">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="bfa42-915">Az.ContainerInstance</span></span>
- <span data-ttu-id="bfa42-916">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="bfa42-916">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="bfa42-917">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="bfa42-917">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="bfa42-918">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="bfa42-918">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="bfa42-919">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="bfa42-919">Az.DataLakeStore</span></span>
- <span data-ttu-id="bfa42-920">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="bfa42-920">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="bfa42-921">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="bfa42-921">Az.Monitor</span></span>
- <span data-ttu-id="bfa42-922">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="bfa42-922">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="bfa42-923">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="bfa42-923">Az.KeyVault</span></span>
- <span data-ttu-id="bfa42-924">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="bfa42-924">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="bfa42-925">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="bfa42-925">Az.MachineLearning</span></span>
- <span data-ttu-id="bfa42-926">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="bfa42-926">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="bfa42-927">Az.Media</span><span class="sxs-lookup"><span data-stu-id="bfa42-927">Az.Media</span></span>
- <span data-ttu-id="bfa42-928">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="bfa42-928">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="bfa42-929">Az.Network</span><span class="sxs-lookup"><span data-stu-id="bfa42-929">Az.Network</span></span>
<span data-ttu-id="bfa42-930">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="bfa42-930">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="bfa42-931">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="bfa42-931">New cmdlets added:</span></span>
        - <span data-ttu-id="bfa42-932">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="bfa42-932">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="bfa42-933">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="bfa42-933">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="bfa42-934">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="bfa42-934">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="bfa42-935">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="bfa42-935">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="bfa42-936">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="bfa42-936">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="bfa42-937">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="bfa42-937">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="bfa42-938">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="bfa42-938">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="bfa42-939">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="bfa42-939">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="bfa42-940">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="bfa42-940">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="bfa42-941">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="bfa42-941">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="bfa42-942">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="bfa42-942">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="bfa42-943">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="bfa42-943">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="bfa42-944">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="bfa42-944">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="bfa42-945">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="bfa42-945">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="bfa42-946">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="bfa42-946">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="bfa42-947">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="bfa42-947">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="bfa42-948">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="bfa42-948">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="bfa42-949">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="bfa42-949">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="bfa42-950">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="bfa42-950">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="bfa42-951">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="bfa42-951">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="bfa42-952">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="bfa42-952">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="bfa42-953">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="bfa42-953">Az.OperationalInsights</span></span>
- <span data-ttu-id="bfa42-954">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="bfa42-954">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="bfa42-955">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="bfa42-955">Az.Profile</span></span>
- <span data-ttu-id="bfa42-956">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="bfa42-956">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="bfa42-957">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="bfa42-957">Az.RecoveryServices</span></span>
- <span data-ttu-id="bfa42-958">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="bfa42-958">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="bfa42-959">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="bfa42-959">Az.Resources</span></span>
- <span data-ttu-id="bfa42-960">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="bfa42-960">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="bfa42-961">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="bfa42-961">Az.ServiceFabric</span></span>
- <span data-ttu-id="bfa42-962">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="bfa42-962">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="bfa42-963">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="bfa42-963">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="bfa42-964">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="bfa42-964">Az.SIgnalR</span></span>
- <span data-ttu-id="bfa42-965">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="bfa42-965">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="bfa42-966">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="bfa42-966">Az.Sql</span></span>
- <span data-ttu-id="bfa42-967">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="bfa42-967">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="bfa42-968">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="bfa42-968">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="bfa42-969">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="bfa42-969">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="bfa42-970">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="bfa42-970">Az.Storage</span></span>
- <span data-ttu-id="bfa42-971">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="bfa42-971">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="bfa42-972">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="bfa42-972">Az.Websites</span></span>
- <span data-ttu-id="bfa42-973">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="bfa42-973">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="bfa42-974">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="bfa42-974">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="bfa42-975">Geral</span><span class="sxs-lookup"><span data-stu-id="bfa42-975">General</span></span>

* <span data-ttu-id="bfa42-976">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="bfa42-976">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="bfa42-977">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="bfa42-977">Az.Compute</span></span>

* <span data-ttu-id="bfa42-978">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="bfa42-978">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="bfa42-979">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="bfa42-979">Az.DataLakeStore</span></span>

* <span data-ttu-id="bfa42-980">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="bfa42-980">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="bfa42-981">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="bfa42-981">Az.FrontDoor</span></span>

* <span data-ttu-id="bfa42-982">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="bfa42-982">Fixed some broken links</span></span>
    - <span data-ttu-id="bfa42-983">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="bfa42-983">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="bfa42-984">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="bfa42-984">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="bfa42-985">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="bfa42-985">Az.RecoveryServices</span></span>

* <span data-ttu-id="bfa42-986">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="bfa42-986">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="bfa42-987">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="bfa42-987">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="bfa42-988">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="bfa42-988">Az.Resources</span></span>

* <span data-ttu-id="bfa42-989">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="bfa42-989">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="bfa42-990">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="bfa42-990">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="bfa42-991">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="bfa42-991">Az.Sql</span></span>

* <span data-ttu-id="bfa42-992">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="bfa42-992">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="bfa42-993">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="bfa42-993">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="bfa42-994">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="bfa42-994">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="bfa42-995">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="bfa42-995">Az.Storage</span></span>

* <span data-ttu-id="bfa42-996">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="bfa42-996">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="bfa42-997">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="bfa42-997">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="bfa42-998">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="bfa42-998">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="bfa42-999">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="bfa42-999">Support Static Website configuration</span></span>
    - <span data-ttu-id="bfa42-1000">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="bfa42-1000">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="bfa42-1001">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="bfa42-1001">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="bfa42-1002">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="bfa42-1002">Az.Websites</span></span>

* <span data-ttu-id="bfa42-1003">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="bfa42-1003">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="bfa42-1004">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1004">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="bfa42-1005">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1005">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="bfa42-1006">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="bfa42-1006">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="bfa42-1007">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="bfa42-1007">Az.ApiManagement</span></span>
* <span data-ttu-id="bfa42-1008">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="bfa42-1008">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="bfa42-1009">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="bfa42-1009">Az.Automation</span></span>
* <span data-ttu-id="bfa42-1010">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="bfa42-1010">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="bfa42-1011">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="bfa42-1011">Added Update Management cmdlets</span></span>
* <span data-ttu-id="bfa42-1012">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="bfa42-1012">Added Source Control cmdlets</span></span>
* <span data-ttu-id="bfa42-1013">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="bfa42-1013">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="bfa42-1014">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="bfa42-1014">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="bfa42-1015">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="bfa42-1015">Az.Compute</span></span>
* <span data-ttu-id="bfa42-1016">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="bfa42-1016">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="bfa42-1017">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="bfa42-1017">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="bfa42-1018">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="bfa42-1018">Az.ContainerInstance</span></span>
* <span data-ttu-id="bfa42-1019">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="bfa42-1019">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="bfa42-1020">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="bfa42-1020">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="bfa42-1021">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="bfa42-1021">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="bfa42-1022">Az.Network</span><span class="sxs-lookup"><span data-stu-id="bfa42-1022">Az.Network</span></span>
* <span data-ttu-id="bfa42-1023">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="bfa42-1023">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="bfa42-1024">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="bfa42-1024">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="bfa42-1025">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1025">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="bfa42-1026">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="bfa42-1026">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="bfa42-1027">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="bfa42-1027">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="bfa42-1028">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1028">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="bfa42-1029">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1029">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="bfa42-1030">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="bfa42-1030">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="bfa42-1031">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="bfa42-1031">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="bfa42-1032">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="bfa42-1032">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="bfa42-1033">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="bfa42-1033">Az.Relay</span></span>
* <span data-ttu-id="bfa42-1034">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1034">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="bfa42-1035">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="bfa42-1035">Az.Resources</span></span>
* <span data-ttu-id="bfa42-1036">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="bfa42-1036">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="bfa42-1037">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="bfa42-1037">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="bfa42-1038">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="bfa42-1038">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="bfa42-1039">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="bfa42-1039">Az.ServiceFabric</span></span>
* <span data-ttu-id="bfa42-1040">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="bfa42-1040">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="bfa42-1041">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="bfa42-1041">Az.Sql</span></span>
* <span data-ttu-id="bfa42-1042">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="bfa42-1042">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="bfa42-1043">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="bfa42-1043">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="bfa42-1044">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="bfa42-1044">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="bfa42-1045">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="bfa42-1045">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="bfa42-1046">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="bfa42-1046">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="bfa42-1047">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="bfa42-1047">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="bfa42-1048">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="bfa42-1048">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="bfa42-1049">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="bfa42-1049">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="bfa42-1050">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="bfa42-1050">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="bfa42-1051">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1051">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="bfa42-1052">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1052">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="bfa42-1053">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1053">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="bfa42-1054">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1054">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="bfa42-1055">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1055">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="bfa42-1056">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1056">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="bfa42-1057">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1057">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="bfa42-1058">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="bfa42-1058">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="bfa42-1059">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="bfa42-1059">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="bfa42-1060">Geral</span><span class="sxs-lookup"><span data-stu-id="bfa42-1060">General</span></span>
* <span data-ttu-id="bfa42-1061">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="bfa42-1061">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="bfa42-1062">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="bfa42-1062">Az.Profile</span></span>
* <span data-ttu-id="bfa42-1063">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="bfa42-1063">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="bfa42-1064">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="bfa42-1064">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="bfa42-1065">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="bfa42-1065">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="bfa42-1066">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="bfa42-1066">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="bfa42-1067">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="bfa42-1067">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="bfa42-1068">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="bfa42-1068">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="bfa42-1069">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="bfa42-1069">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="bfa42-1070">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="bfa42-1070">Az.CognitiveServices</span></span>
* <span data-ttu-id="bfa42-1071">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1071">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="bfa42-1072">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="bfa42-1072">Az.Compute</span></span>
* <span data-ttu-id="bfa42-1073">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="bfa42-1073">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="bfa42-1074">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="bfa42-1074">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="bfa42-1075">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1075">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="bfa42-1076">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="bfa42-1076">Az.DataLakeStore</span></span>
* <span data-ttu-id="bfa42-1077">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1077">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="bfa42-1078">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1078">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="bfa42-1079">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="bfa42-1079">Az.Insights</span></span>
* <span data-ttu-id="bfa42-1080">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="bfa42-1080">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="bfa42-1081">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="bfa42-1081">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="bfa42-1082">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="bfa42-1082">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="bfa42-1083">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="bfa42-1083">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="bfa42-1084">Az.Network</span><span class="sxs-lookup"><span data-stu-id="bfa42-1084">Az.Network</span></span>
* <span data-ttu-id="bfa42-1085">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="bfa42-1085">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="bfa42-1086">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="bfa42-1086">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="bfa42-1087">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="bfa42-1087">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="bfa42-1088">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="bfa42-1088">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="bfa42-1089">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="bfa42-1089">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="bfa42-1090">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="bfa42-1090">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="bfa42-1091">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="bfa42-1091">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="bfa42-1092">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="bfa42-1092">Az.PolicyInsights</span></span>
* <span data-ttu-id="bfa42-1093">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="bfa42-1093">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="bfa42-1094">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="bfa42-1094">Az.Resources</span></span>
* <span data-ttu-id="bfa42-1095">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="bfa42-1095">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="bfa42-1096">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="bfa42-1096">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="bfa42-1097">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="bfa42-1097">Az.ServiceBus</span></span>
* <span data-ttu-id="bfa42-1098">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1098">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="bfa42-1099">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="bfa42-1099">Az.ServiceFabric</span></span>
* <span data-ttu-id="bfa42-1100">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1100">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="bfa42-1101">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="bfa42-1101">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="bfa42-1102">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="bfa42-1102">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="bfa42-1103">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="bfa42-1103">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="bfa42-1104">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1104">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="bfa42-1105">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="bfa42-1105">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="bfa42-1106">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="bfa42-1106">Az.Profile</span></span>
* <span data-ttu-id="bfa42-1107">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="bfa42-1107">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="bfa42-1108">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="bfa42-1108">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="bfa42-1109">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="bfa42-1109">Az.Compute</span></span>
* <span data-ttu-id="bfa42-1110">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="bfa42-1110">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="bfa42-1111">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1111">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="bfa42-1112">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="bfa42-1112">Az.DataLakeStore</span></span>
* <span data-ttu-id="bfa42-1113">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="bfa42-1113">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="bfa42-1114">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1114">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="bfa42-1115">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1115">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="bfa42-1116">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1116">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="bfa42-1117">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1117">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="bfa42-1118">Az.Network</span><span class="sxs-lookup"><span data-stu-id="bfa42-1118">Az.Network</span></span>
* <span data-ttu-id="bfa42-1119">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1119">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="bfa42-1120">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1120">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="bfa42-1121">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="bfa42-1121">Az.Resources</span></span>
* <span data-ttu-id="bfa42-1122">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1122">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="bfa42-1123">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="bfa42-1123">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="bfa42-1124">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="bfa42-1124">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="bfa42-1125">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="bfa42-1125">Azure.Storage</span></span>
* <span data-ttu-id="bfa42-1126">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="bfa42-1126">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="bfa42-1127">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="bfa42-1127">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="bfa42-1128">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="bfa42-1128">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="bfa42-1129">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1129">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="bfa42-1130">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="bfa42-1130">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="bfa42-1131">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="bfa42-1131">Az.CognitiveServices</span></span>
* <span data-ttu-id="bfa42-1132">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1132">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="bfa42-1133">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="bfa42-1133">Az.Compute</span></span>
* <span data-ttu-id="bfa42-1134">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="bfa42-1134">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="bfa42-1135">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1135">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="bfa42-1136">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="bfa42-1136">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="bfa42-1137">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="bfa42-1137">Az.DataFactoryV2</span></span>
* <span data-ttu-id="bfa42-1138">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1138">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="bfa42-1139">Az.Network</span><span class="sxs-lookup"><span data-stu-id="bfa42-1139">Az.Network</span></span>
* <span data-ttu-id="bfa42-1140">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1140">Added NetworkProfile functionality.</span></span> <span data-ttu-id="bfa42-1141">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="bfa42-1141">new cmdlets added</span></span>
    - <span data-ttu-id="bfa42-1142">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="bfa42-1142">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="bfa42-1143">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="bfa42-1143">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="bfa42-1144">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="bfa42-1144">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="bfa42-1145">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="bfa42-1145">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="bfa42-1146">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="bfa42-1146">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="bfa42-1147">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="bfa42-1147">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="bfa42-1148">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="bfa42-1148">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="bfa42-1149">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="bfa42-1149">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="bfa42-1150">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="bfa42-1150">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="bfa42-1151">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="bfa42-1151">Az.RedisCache</span></span>
* <span data-ttu-id="bfa42-1152">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="bfa42-1152">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="bfa42-1153">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="bfa42-1153">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="bfa42-1154">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="bfa42-1154">Az.Resources</span></span>
* <span data-ttu-id="bfa42-1155">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="bfa42-1155">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="bfa42-1156">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="bfa42-1156">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="bfa42-1157">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="bfa42-1157">Az.Sql</span></span>
* <span data-ttu-id="bfa42-1158">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="bfa42-1158">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="bfa42-1159">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="bfa42-1159">Az.Websites</span></span>
* <span data-ttu-id="bfa42-1160">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="bfa42-1160">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="bfa42-1161">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="bfa42-1161">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="bfa42-1162">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="bfa42-1162">0.2.0 - September 2018</span></span>
 <span data-ttu-id="bfa42-1163">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="bfa42-1163">Initial Release</span></span>