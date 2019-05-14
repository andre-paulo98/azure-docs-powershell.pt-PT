---
ms.openlocfilehash: 3848f7fb8e298d137c747405f32a0776c1a8f029
ms.sourcegitcommit: accff0c2cd6035fcda2d917f6051a5b509eb6255
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/06/2019
ms.locfileid: "65048636"
---
## <a name="200---may-2019"></a><span data-ttu-id="965b8-101">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="965b8-101">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="965b8-102">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="965b8-102">Az.Accounts</span></span>
* <span data-ttu-id="965b8-103">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="965b8-103">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="965b8-104">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="965b8-104">Az.CognitiveServices</span></span>
* <span data-ttu-id="965b8-105">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="965b8-105">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="965b8-106">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="965b8-106">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="965b8-107">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="965b8-107">Az.Compute</span></span>
* <span data-ttu-id="965b8-108">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="965b8-108">Proximity placement group feature.</span></span>
    - <span data-ttu-id="965b8-109">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="965b8-109">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="965b8-110">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="965b8-110">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="965b8-111">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="965b8-111">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="965b8-112">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="965b8-112">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="965b8-113">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="965b8-113">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="965b8-114">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="965b8-114">Breaking changes</span></span>
    - <span data-ttu-id="965b8-115">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="965b8-115">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="965b8-116">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="965b8-116">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="965b8-117">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="965b8-117">Az.DeploymentManager</span></span>
* <span data-ttu-id="965b8-118">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="965b8-118">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="965b8-119">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="965b8-119">Az.Dns</span></span>
* <span data-ttu-id="965b8-120">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="965b8-120">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="965b8-121">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="965b8-121">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="965b8-122">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="965b8-122">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="965b8-123">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="965b8-123">Az.FrontDoor</span></span>
* <span data-ttu-id="965b8-124">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="965b8-124">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="965b8-125">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="965b8-125">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="965b8-126">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="965b8-126">Az.HDInsight</span></span>
* <span data-ttu-id="965b8-127">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="965b8-127">Removed two cmdlets:</span></span>
    - <span data-ttu-id="965b8-128">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="965b8-128">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="965b8-129">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="965b8-129">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="965b8-130">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="965b8-130">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="965b8-131">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="965b8-131">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="965b8-132">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="965b8-132">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="965b8-133">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="965b8-133">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="965b8-134">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="965b8-134">Az.Monitor</span></span>
* <span data-ttu-id="965b8-135">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="965b8-135">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="965b8-136">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="965b8-136">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="965b8-137">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="965b8-137">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="965b8-138">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="965b8-138">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="965b8-139">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="965b8-139">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="965b8-140">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="965b8-140">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="965b8-141">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="965b8-141">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="965b8-142">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="965b8-142">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="965b8-143">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="965b8-143">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="965b8-144">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="965b8-144">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="965b8-145">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="965b8-145">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="965b8-146">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="965b8-146">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="965b8-147">[Mais](https://docs.microsoft.com/en-us/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="965b8-147">[More](https://docs.microsoft.com/en-us/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="965b8-148">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="965b8-148">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="965b8-149">Az.Network</span><span class="sxs-lookup"><span data-stu-id="965b8-149">Az.Network</span></span>
* <span data-ttu-id="965b8-150">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="965b8-150">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="965b8-151">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="965b8-151">New cmdlets</span></span>
        - <span data-ttu-id="965b8-152">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="965b8-152">New-AzNatGateway</span></span>
        - <span data-ttu-id="965b8-153">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="965b8-153">Get-AzNatGateway</span></span>
        - <span data-ttu-id="965b8-154">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="965b8-154">Set-AzNatGateway</span></span>
        - <span data-ttu-id="965b8-155">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="965b8-155">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="965b8-156">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="965b8-156">Updated cmdlets</span></span>
        - <span data-ttu-id="965b8-157">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="965b8-157">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="965b8-158">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="965b8-158">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="965b8-159">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="965b8-159">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="965b8-160">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="965b8-160">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="965b8-161">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="965b8-161">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="965b8-162">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="965b8-162">Az.PolicyInsights</span></span>
* <span data-ttu-id="965b8-163">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="965b8-163">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="965b8-164">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="965b8-164">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="965b8-165">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="965b8-165">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="965b8-166">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="965b8-166">Az.RecoveryServices</span></span>
* <span data-ttu-id="965b8-167">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="965b8-167">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="965b8-168">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="965b8-168">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="965b8-169">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="965b8-169">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="965b8-170">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="965b8-170">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="965b8-171">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="965b8-171">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="965b8-172">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="965b8-172">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="965b8-173">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="965b8-173">Az.Relay</span></span>
* <span data-ttu-id="965b8-174">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="965b8-174">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="965b8-175">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="965b8-175">Az.ServiceBus</span></span>
* <span data-ttu-id="965b8-176">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="965b8-176">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="965b8-177">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="965b8-177">Az.Storage</span></span>
* <span data-ttu-id="965b8-178">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage.*" para "Microsoft.Azure.Storage.*")</span><span class="sxs-lookup"><span data-stu-id="965b8-178">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="965b8-179">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="965b8-179">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="965b8-180">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="965b8-180">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="965b8-181">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="965b8-181">New-AzStorageAccount</span></span>
* <span data-ttu-id="965b8-182">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="965b8-182">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="965b8-183">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="965b8-183">New-AzStorageAccount</span></span>
    - <span data-ttu-id="965b8-184">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="965b8-184">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="965b8-185">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="965b8-185">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="965b8-186">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="965b8-186">Az.Websites</span></span>
* <span data-ttu-id="965b8-187">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="965b8-187">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="965b8-188">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="965b8-188">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="965b8-189">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="965b8-189">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="965b8-190">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="965b8-190">Highlights since the last major release</span></span>
* <span data-ttu-id="965b8-191">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="965b8-191">General availability of `Az` module</span></span>
* <span data-ttu-id="965b8-192">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="965b8-192">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="965b8-193">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="965b8-193">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="965b8-194">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="965b8-194">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="965b8-195">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="965b8-195">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="965b8-196">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="965b8-196">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="965b8-197">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="965b8-197">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="965b8-198">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="965b8-198">Az.Accounts</span></span>
* <span data-ttu-id="965b8-199">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="965b8-199">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="965b8-200">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="965b8-200">Az.Batch</span></span>
* <span data-ttu-id="965b8-201">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="965b8-201">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="965b8-202">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="965b8-202">Az.Cdn</span></span>
* <span data-ttu-id="965b8-203">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="965b8-203">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="965b8-204">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="965b8-204">Az.CognitiveServices</span></span>
* <span data-ttu-id="965b8-205">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="965b8-205">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="965b8-206">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="965b8-206">Az.Compute</span></span>
* <span data-ttu-id="965b8-207">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="965b8-207">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="965b8-208">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="965b8-208">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="965b8-209">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="965b8-209">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="965b8-210">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="965b8-210">Az.DataFactory</span></span>
* <span data-ttu-id="965b8-211">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="965b8-211">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="965b8-212">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="965b8-212">Az.DataLakeStore</span></span>
* <span data-ttu-id="965b8-213">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="965b8-213">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="965b8-214">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="965b8-214">Az.EventGrid</span></span>
* <span data-ttu-id="965b8-215">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="965b8-215">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="965b8-216">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="965b8-216">Az.EventHub</span></span>
* <span data-ttu-id="965b8-217">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="965b8-217">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="965b8-218">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="965b8-218">Az.HDInsight</span></span>
* <span data-ttu-id="965b8-219">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="965b8-219">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="965b8-220">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="965b8-220">Az.IotHub</span></span>
* <span data-ttu-id="965b8-221">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="965b8-221">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="965b8-222">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="965b8-222">Az.KeyVault</span></span>
* <span data-ttu-id="965b8-223">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="965b8-223">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="965b8-224">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="965b8-224">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="965b8-225">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="965b8-225">Az.MachineLearning</span></span>
* <span data-ttu-id="965b8-226">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="965b8-226">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="965b8-227">Az.Media</span><span class="sxs-lookup"><span data-stu-id="965b8-227">Az.Media</span></span>
* <span data-ttu-id="965b8-228">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="965b8-228">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="965b8-229">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="965b8-229">Az.Monitor</span></span>
  * <span data-ttu-id="965b8-230">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="965b8-230">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="965b8-231">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="965b8-231">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="965b8-232">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="965b8-232">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="965b8-233">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="965b8-233">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="965b8-234">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="965b8-234">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="965b8-235">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="965b8-235">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="965b8-236">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="965b8-236">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="965b8-237">Az.Network</span><span class="sxs-lookup"><span data-stu-id="965b8-237">Az.Network</span></span>
* <span data-ttu-id="965b8-238">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="965b8-238">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="965b8-239">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="965b8-239">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="965b8-240">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="965b8-240">Az.NotificationHubs</span></span>
* <span data-ttu-id="965b8-241">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="965b8-241">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="965b8-242">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="965b8-242">Az.OperationalInsights</span></span>
* <span data-ttu-id="965b8-243">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="965b8-243">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="965b8-244">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="965b8-244">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="965b8-245">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="965b8-245">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="965b8-246">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="965b8-246">Az.RecoveryServices</span></span>
* <span data-ttu-id="965b8-247">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="965b8-247">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="965b8-248">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="965b8-248">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="965b8-249">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="965b8-249">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="965b8-250">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="965b8-250">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="965b8-251">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="965b8-251">Az.RedisCache</span></span>
* <span data-ttu-id="965b8-252">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="965b8-252">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="965b8-253">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="965b8-253">Az.Resources</span></span>
* <span data-ttu-id="965b8-254">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="965b8-254">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="965b8-255">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="965b8-255">Az.Sql</span></span>
* <span data-ttu-id="965b8-256">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="965b8-256">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="965b8-257">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="965b8-257">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="965b8-258">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="965b8-258">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="965b8-259">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="965b8-259">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="965b8-260">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="965b8-260">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="965b8-261">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="965b8-261">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="965b8-262">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="965b8-262">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="965b8-263">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="965b8-263">Az.Websites</span></span>
* <span data-ttu-id="965b8-264">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="965b8-264">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="965b8-265">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="965b8-265">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="965b8-266">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="965b8-266">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="965b8-267">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="965b8-267">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="965b8-268">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="965b8-268">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="965b8-269">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="965b8-269">Highlights since the last major release</span></span>
* <span data-ttu-id="965b8-270">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="965b8-270">General availability of `Az` module</span></span>
* <span data-ttu-id="965b8-271">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="965b8-271">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="965b8-272">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="965b8-272">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="965b8-273">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="965b8-273">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="965b8-274">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="965b8-274">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="965b8-275">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="965b8-275">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="965b8-276">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="965b8-276">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="965b8-277">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="965b8-277">Az.Accounts</span></span>
* <span data-ttu-id="965b8-278">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="965b8-278">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="965b8-279">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="965b8-279">Az.AnalysisServices</span></span>
* <span data-ttu-id="965b8-280">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="965b8-280">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="965b8-281">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="965b8-281">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="965b8-282">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="965b8-282">Az.Automation</span></span>
* <span data-ttu-id="965b8-283">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="965b8-283">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="965b8-284">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="965b8-284">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="965b8-285">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="965b8-285">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="965b8-286">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="965b8-286">Az.Compute</span></span>
* <span data-ttu-id="965b8-287">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="965b8-287">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="965b8-288">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="965b8-288">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="965b8-289">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="965b8-289">Az.ContainerInstance</span></span>
* <span data-ttu-id="965b8-290">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="965b8-290">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="965b8-291">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="965b8-291">Az.DataFactory</span></span>
* <span data-ttu-id="965b8-292">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="965b8-292">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="965b8-293">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="965b8-293">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="965b8-294">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="965b8-294">Az.Resources</span></span>
* <span data-ttu-id="965b8-295">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="965b8-295">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="965b8-296">Melhor processamento de erros de "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="965b8-296">Improve error handling for for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="965b8-297">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="965b8-297">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="965b8-298">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="965b8-298">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="965b8-299">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="965b8-299">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="965b8-300">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="965b8-300">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="965b8-301">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="965b8-301">Az.Sql</span></span>
* <span data-ttu-id="965b8-302">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="965b8-302">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="965b8-303">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="965b8-303">Az.Storage</span></span>
* <span data-ttu-id="965b8-304">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="965b8-304">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="965b8-305">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="965b8-305">New-AzStorageContext</span></span>
* <span data-ttu-id="965b8-306">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="965b8-306">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="965b8-307">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="965b8-307">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="965b8-308">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="965b8-308">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="965b8-309">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="965b8-309">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="965b8-310">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="965b8-310">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="965b8-311">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="965b8-311">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="965b8-312">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="965b8-312">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="965b8-313">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="965b8-313">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="965b8-314">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="965b8-314">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="965b8-315">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="965b8-315">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="965b8-316">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="965b8-316">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="965b8-317">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="965b8-317">Highlights since the last major release</span></span>
* <span data-ttu-id="965b8-318">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="965b8-318">General availability of `Az` module</span></span>
* <span data-ttu-id="965b8-319">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="965b8-319">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="965b8-320">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="965b8-320">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="965b8-321">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="965b8-321">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="965b8-322">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="965b8-322">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="965b8-323">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="965b8-323">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="965b8-324">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="965b8-324">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="965b8-325">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="965b8-325">Az.Automation</span></span>
* <span data-ttu-id="965b8-326">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="965b8-326">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="965b8-327">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="965b8-327">Dynamic grouping</span></span>
    * <span data-ttu-id="965b8-328">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="965b8-328">Pre-Post script</span></span>
    * <span data-ttu-id="965b8-329">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="965b8-329">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="965b8-330">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="965b8-330">Az.Compute</span></span>
* <span data-ttu-id="965b8-331">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="965b8-331">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="965b8-332">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="965b8-332">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="965b8-333">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="965b8-333">Az.KeyVault</span></span>
* <span data-ttu-id="965b8-334">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="965b8-334">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="965b8-335">Az.Network</span><span class="sxs-lookup"><span data-stu-id="965b8-335">Az.Network</span></span>
* <span data-ttu-id="965b8-336">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="965b8-336">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="965b8-337">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="965b8-337">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="965b8-338">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="965b8-338">Az.RecoveryServices</span></span>
* <span data-ttu-id="965b8-339">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="965b8-339">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="965b8-340">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="965b8-340">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="965b8-341">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="965b8-341">Az.Resources</span></span>
* <span data-ttu-id="965b8-342">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="965b8-342">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="965b8-343">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="965b8-343">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="965b8-344">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="965b8-344">Az.Sql</span></span>
* <span data-ttu-id="965b8-345">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="965b8-345">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="965b8-346">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="965b8-346">Az.Storage</span></span>
* <span data-ttu-id="965b8-347">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="965b8-347">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="965b8-348">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="965b8-348">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="965b8-349">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="965b8-349">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="965b8-350">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="965b8-350">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="965b8-351">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="965b8-351">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="965b8-352">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="965b8-352">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="965b8-353">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="965b8-353">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="965b8-354">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="965b8-354">Az.Websites</span></span>
* <span data-ttu-id="965b8-355">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="965b8-355">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="965b8-356">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="965b8-356">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="965b8-357">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="965b8-357">Az.Accounts</span></span>
* <span data-ttu-id="965b8-358">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="965b8-358">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="965b8-359">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="965b8-359">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="965b8-360">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="965b8-360">Az.Automation</span></span>
* <span data-ttu-id="965b8-361">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="965b8-361">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="965b8-362">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="965b8-362">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="965b8-363">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="965b8-363">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="965b8-364">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="965b8-364">Az.Cdn</span></span>
* <span data-ttu-id="965b8-365">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="965b8-365">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="965b8-366">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="965b8-366">Az.Compute</span></span>
* <span data-ttu-id="965b8-367">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="965b8-367">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="965b8-368">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="965b8-368">Az.DataFactory</span></span>
* <span data-ttu-id="965b8-369">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="965b8-369">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="965b8-370">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="965b8-370">Az.LogicApp</span></span>
* <span data-ttu-id="965b8-371">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="965b8-371">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="965b8-372">Az.Network</span><span class="sxs-lookup"><span data-stu-id="965b8-372">Az.Network</span></span>
* <span data-ttu-id="965b8-373">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="965b8-373">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="965b8-374">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="965b8-374">Az.RecoveryServices</span></span>
* <span data-ttu-id="965b8-375">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="965b8-375">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="965b8-376">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="965b8-376">SDK Update</span></span>
* <span data-ttu-id="965b8-377">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="965b8-377">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="965b8-378">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="965b8-378">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="965b8-379">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="965b8-379">Az.Resources</span></span>
* <span data-ttu-id="965b8-380">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="965b8-380">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="965b8-381">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="965b8-381">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="965b8-382">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="965b8-382">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="965b8-383">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="965b8-383">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="965b8-384">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="965b8-384">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="965b8-385">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="965b8-385">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="965b8-386">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="965b8-386">Az.Sql</span></span>
* <span data-ttu-id="965b8-387">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="965b8-387">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="965b8-388">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="965b8-388">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="965b8-389">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="965b8-389">Az.Storage</span></span>
* <span data-ttu-id="965b8-390">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="965b8-390">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="965b8-391">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="965b8-391">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="965b8-392">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="965b8-392">Az.AnalysisServices</span></span>
* <span data-ttu-id="965b8-393">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="965b8-393">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="965b8-394">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="965b8-394">Az.Automation</span></span>
* <span data-ttu-id="965b8-395">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="965b8-395">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="965b8-396">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="965b8-396">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="965b8-397">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="965b8-397">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="965b8-398">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="965b8-398">Az.CognitiveServices</span></span>
* <span data-ttu-id="965b8-399">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="965b8-399">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="965b8-400">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="965b8-400">Az.Compute</span></span>
* <span data-ttu-id="965b8-401">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="965b8-401">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="965b8-402">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="965b8-402">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="965b8-403">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="965b8-403">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="965b8-404">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="965b8-404">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="965b8-405">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="965b8-405">Az.DataLakeStore</span></span>
* <span data-ttu-id="965b8-406">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="965b8-406">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="965b8-407">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="965b8-407">Az.EventHub</span></span>
* <span data-ttu-id="965b8-408">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="965b8-408">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="965b8-409">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="965b8-409">Az.KeyVault</span></span>
* <span data-ttu-id="965b8-410">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="965b8-410">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="965b8-411">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="965b8-411">Az.LogicApp</span></span>
* <span data-ttu-id="965b8-412">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="965b8-412">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="965b8-413">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="965b8-413">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="965b8-414">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="965b8-414">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="965b8-415">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="965b8-415">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="965b8-416">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="965b8-416">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="965b8-417">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="965b8-417">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="965b8-418">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="965b8-418">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="965b8-419">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="965b8-419">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="965b8-420">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="965b8-420">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="965b8-421">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="965b8-421">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="965b8-422">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="965b8-422">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="965b8-423">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="965b8-423">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="965b8-424">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="965b8-424">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="965b8-425">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="965b8-425">Az.Monitor</span></span>
* <span data-ttu-id="965b8-426">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="965b8-426">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="965b8-427">Az.Network</span><span class="sxs-lookup"><span data-stu-id="965b8-427">Az.Network</span></span>
* <span data-ttu-id="965b8-428">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="965b8-428">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="965b8-429">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="965b8-429">Az.OperationalInsights</span></span>
* <span data-ttu-id="965b8-430">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="965b8-430">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="965b8-431">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="965b8-431">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="965b8-432">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="965b8-432">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="965b8-433">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="965b8-433">Az.Resources</span></span>
* <span data-ttu-id="965b8-434">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="965b8-434">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="965b8-435">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="965b8-435">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="965b8-436">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="965b8-436">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="965b8-437">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="965b8-437">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="965b8-438">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="965b8-438">Az.Sql</span></span>
* <span data-ttu-id="965b8-439">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="965b8-439">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="965b8-440">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="965b8-440">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="965b8-441">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="965b8-441">Az.Websites</span></span>
* <span data-ttu-id="965b8-442">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="965b8-442">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="965b8-443">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="965b8-443">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="965b8-444">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="965b8-444">Az.Accounts</span></span>
* <span data-ttu-id="965b8-445">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="965b8-445">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="965b8-446">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="965b8-446">Az.AnalysisServices</span></span>
<span data-ttu-id="965b8-447">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="965b8-447">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="965b8-448">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="965b8-448">Az.Compute</span></span>
* <span data-ttu-id="965b8-449">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="965b8-449">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="965b8-450">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="965b8-450">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="965b8-451">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="965b8-451">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="965b8-452">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="965b8-452">Az.RecoveryServices</span></span>
<span data-ttu-id="965b8-453">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="965b8-453">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="965b8-454">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="965b8-454">Az.Resources</span></span>
* <span data-ttu-id="965b8-455">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="965b8-455">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="965b8-456">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="965b8-456">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="965b8-457">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="965b8-457">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="965b8-458">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="965b8-458">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="965b8-459">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="965b8-459">Az.Sql</span></span>
* <span data-ttu-id="965b8-460">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="965b8-460">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="965b8-461">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="965b8-461">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="965b8-462">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="965b8-462">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="965b8-463">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="965b8-463">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="965b8-464">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="965b8-464">Az.Accounts</span></span>
* <span data-ttu-id="965b8-465">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="965b8-465">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="965b8-466">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="965b8-466">Az.AnalysisServices</span></span>
* <span data-ttu-id="965b8-467">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="965b8-467">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="965b8-468">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="965b8-468">Az.RecoveryServices</span></span>
* <span data-ttu-id="965b8-469">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="965b8-469">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="965b8-470">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="965b8-470">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="965b8-471">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="965b8-471">Az.Accounts</span></span>
* <span data-ttu-id="965b8-472">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="965b8-472">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="965b8-473">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="965b8-473">Update incorrect online help URLs</span></span>
* <span data-ttu-id="965b8-474">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="965b8-474">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="965b8-475">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="965b8-475">Az.Aks</span></span>
* <span data-ttu-id="965b8-476">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="965b8-476">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="965b8-477">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="965b8-477">Az.Automation</span></span>
* <span data-ttu-id="965b8-478">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="965b8-478">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="965b8-479">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="965b8-479">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="965b8-480">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="965b8-480">Az.Cdn</span></span>
* <span data-ttu-id="965b8-481">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="965b8-481">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="965b8-482">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="965b8-482">Az.Compute</span></span>
* <span data-ttu-id="965b8-483">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="965b8-483">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="965b8-484">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="965b8-484">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="965b8-485">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="965b8-485">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="965b8-486">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="965b8-486">Az.ContainerRegistry</span></span>
* <span data-ttu-id="965b8-487">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="965b8-487">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="965b8-488">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="965b8-488">Az.DataFactory</span></span>
* <span data-ttu-id="965b8-489">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="965b8-489">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="965b8-490">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="965b8-490">Az.DataLakeStore</span></span>
* <span data-ttu-id="965b8-491">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="965b8-491">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="965b8-492">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="965b8-492">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="965b8-493">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="965b8-493">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="965b8-494">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="965b8-494">Az.IotHub</span></span>
* <span data-ttu-id="965b8-495">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="965b8-495">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="965b8-496">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="965b8-496">Az.KeyVault</span></span>
* <span data-ttu-id="965b8-497">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="965b8-497">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="965b8-498">Az.Network</span><span class="sxs-lookup"><span data-stu-id="965b8-498">Az.Network</span></span>
* <span data-ttu-id="965b8-499">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="965b8-499">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="965b8-500">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="965b8-500">Az.Resources</span></span>
* <span data-ttu-id="965b8-501">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="965b8-501">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="965b8-502">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="965b8-502">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="965b8-503">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="965b8-503">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="965b8-504">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="965b8-504">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="965b8-505">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="965b8-505">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="965b8-506">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="965b8-506">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="965b8-507">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="965b8-507">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="965b8-508">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="965b8-508">Az.ServiceFabric</span></span>
* <span data-ttu-id="965b8-509">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="965b8-509">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="965b8-510">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="965b8-510">Fix some error messages.</span></span>
* <span data-ttu-id="965b8-511">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="965b8-511">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="965b8-512">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="965b8-512">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="965b8-513">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="965b8-513">Az.SignalR</span></span>
* <span data-ttu-id="965b8-514">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="965b8-514">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="965b8-515">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="965b8-515">Az.Sql</span></span>
* <span data-ttu-id="965b8-516">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="965b8-516">Update incorrect online help URLs</span></span>
* <span data-ttu-id="965b8-517">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="965b8-517">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="965b8-518">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="965b8-518">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="965b8-519">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="965b8-519">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="965b8-520">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="965b8-520">Az.Storage</span></span>
* <span data-ttu-id="965b8-521">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="965b8-521">Update incorrect online help URLs</span></span>
* <span data-ttu-id="965b8-522">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="965b8-522">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="965b8-523">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="965b8-523">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="965b8-524">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="965b8-524">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="965b8-525">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="965b8-525">Az.TrafficManager</span></span>
* <span data-ttu-id="965b8-526">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="965b8-526">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="965b8-527">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="965b8-527">Az.Websites</span></span>
* <span data-ttu-id="965b8-528">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="965b8-528">Update incorrect online help URLs</span></span>
* <span data-ttu-id="965b8-529">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="965b8-529">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="965b8-530">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="965b8-530">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="965b8-531">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="965b8-531">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="965b8-532">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="965b8-532">Az.Accounts</span></span>
* <span data-ttu-id="965b8-533">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="965b8-533">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="965b8-534">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="965b8-534">Az.Compute</span></span>
* <span data-ttu-id="965b8-535">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="965b8-535">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="965b8-536">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="965b8-536">Updated the description of ID in help files</span></span>
* <span data-ttu-id="965b8-537">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="965b8-537">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="965b8-538">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="965b8-538">Az.DataLakeStore</span></span>
* <span data-ttu-id="965b8-539">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="965b8-539">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="965b8-540">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="965b8-540">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="965b8-541">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="965b8-541">Az.EventGrid</span></span>
* <span data-ttu-id="965b8-542">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="965b8-542">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="965b8-543">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="965b8-543">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="965b8-544">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="965b8-544">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="965b8-545">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="965b8-545">Event Time-To-Live,</span></span>
        - <span data-ttu-id="965b8-546">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="965b8-546">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="965b8-547">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="965b8-547">Dead letter endpoint.</span></span>
    - <span data-ttu-id="965b8-548">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="965b8-548">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="965b8-549">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="965b8-549">Event Time-To-Live,</span></span>
        - <span data-ttu-id="965b8-550">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="965b8-550">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="965b8-551">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="965b8-551">Dead letter endpoint.</span></span>
* <span data-ttu-id="965b8-552">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="965b8-552">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="965b8-553">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="965b8-553">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="965b8-554">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="965b8-554">Az.IotHub</span></span>
* <span data-ttu-id="965b8-555">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="965b8-555">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="965b8-556">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="965b8-556">Az.LogicApp</span></span>
* <span data-ttu-id="965b8-557">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="965b8-557">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="965b8-558">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="965b8-558">Az.Resources</span></span>
* <span data-ttu-id="965b8-559">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="965b8-559">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="965b8-560">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="965b8-560">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="965b8-561">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="965b8-561">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="965b8-562">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="965b8-562">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="965b8-563">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="965b8-563">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="965b8-564">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="965b8-564">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="965b8-565">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="965b8-565">Az.SignalR</span></span>
* <span data-ttu-id="965b8-566">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="965b8-566">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="965b8-567">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="965b8-567">Az.Sql</span></span>
* <span data-ttu-id="965b8-568">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="965b8-568">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="965b8-569">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="965b8-569">Az.Storage</span></span>
* <span data-ttu-id="965b8-570">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="965b8-570">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="965b8-571">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="965b8-571">New-AzStorageContext</span></span>
* <span data-ttu-id="965b8-572">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="965b8-572">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="965b8-573">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="965b8-573">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="965b8-574">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="965b8-574">Az.Websites</span></span>
* <span data-ttu-id="965b8-575">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="965b8-575">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="965b8-576">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="965b8-576">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="965b8-577">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="965b8-577">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="965b8-578">Geral</span><span class="sxs-lookup"><span data-stu-id="965b8-578">General</span></span>

- <span data-ttu-id="965b8-579">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="965b8-579">General Availability of Az Module</span></span>
- <span data-ttu-id="965b8-580">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="965b8-580">Online help for each module</span></span>
- <span data-ttu-id="965b8-581">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="965b8-581">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="965b8-582">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="965b8-582">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="965b8-583">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="965b8-583">Az.Accounts</span></span>
- <span data-ttu-id="965b8-584">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="965b8-584">Changed from Az.Profile</span></span>
- <span data-ttu-id="965b8-585">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="965b8-585">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="965b8-586">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="965b8-586">Az.ApiManagement</span></span>
- <span data-ttu-id="965b8-587">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="965b8-587">Fixes for #7002</span></span>
- <span data-ttu-id="965b8-588">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="965b8-588">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="965b8-589">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="965b8-589">Az.Batch</span></span>
- <span data-ttu-id="965b8-590">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="965b8-590">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="965b8-591">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="965b8-591">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="965b8-592">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="965b8-592">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="965b8-593">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="965b8-593">Az.Billing</span></span>
- <span data-ttu-id="965b8-594">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="965b8-594">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="965b8-595">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="965b8-595">Az.CognitivServices</span></span>
- <span data-ttu-id="965b8-596">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="965b8-596">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="965b8-597">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="965b8-597">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="965b8-598">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="965b8-598">Az.ContainerInstance</span></span>
- <span data-ttu-id="965b8-599">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="965b8-599">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="965b8-600">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="965b8-600">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="965b8-601">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="965b8-601">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="965b8-602">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="965b8-602">Az.DataLakeStore</span></span>
- <span data-ttu-id="965b8-603">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="965b8-603">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="965b8-604">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="965b8-604">Az.Monitor</span></span>
- <span data-ttu-id="965b8-605">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="965b8-605">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="965b8-606">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="965b8-606">Az.KeyVault</span></span>
- <span data-ttu-id="965b8-607">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="965b8-607">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="965b8-608">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="965b8-608">Az.MachineLearning</span></span>
- <span data-ttu-id="965b8-609">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="965b8-609">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="965b8-610">Az.Media</span><span class="sxs-lookup"><span data-stu-id="965b8-610">Az.Media</span></span>
- <span data-ttu-id="965b8-611">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="965b8-611">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="965b8-612">Az.Network</span><span class="sxs-lookup"><span data-stu-id="965b8-612">Az.Network</span></span>
<span data-ttu-id="965b8-613">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="965b8-613">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="965b8-614">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="965b8-614">New cmdlets added:</span></span>
        - <span data-ttu-id="965b8-615">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="965b8-615">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="965b8-616">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="965b8-616">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="965b8-617">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="965b8-617">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="965b8-618">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="965b8-618">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="965b8-619">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="965b8-619">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="965b8-620">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="965b8-620">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="965b8-621">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="965b8-621">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="965b8-622">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="965b8-622">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="965b8-623">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="965b8-623">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="965b8-624">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="965b8-624">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="965b8-625">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="965b8-625">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="965b8-626">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="965b8-626">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="965b8-627">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="965b8-627">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="965b8-628">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="965b8-628">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="965b8-629">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="965b8-629">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="965b8-630">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="965b8-630">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="965b8-631">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="965b8-631">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="965b8-632">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="965b8-632">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="965b8-633">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="965b8-633">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="965b8-634">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="965b8-634">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="965b8-635">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="965b8-635">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="965b8-636">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="965b8-636">Az.OperationalInsights</span></span>
- <span data-ttu-id="965b8-637">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="965b8-637">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="965b8-638">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="965b8-638">Az.Profile</span></span>
- <span data-ttu-id="965b8-639">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="965b8-639">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="965b8-640">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="965b8-640">Az.RecoveryServices</span></span>
- <span data-ttu-id="965b8-641">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="965b8-641">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="965b8-642">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="965b8-642">Az.Resources</span></span>
- <span data-ttu-id="965b8-643">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="965b8-643">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="965b8-644">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="965b8-644">Az.ServiceFabric</span></span>
- <span data-ttu-id="965b8-645">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="965b8-645">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="965b8-646">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="965b8-646">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="965b8-647">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="965b8-647">Az.SIgnalR</span></span>
- <span data-ttu-id="965b8-648">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="965b8-648">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="965b8-649">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="965b8-649">Az.Sql</span></span>
- <span data-ttu-id="965b8-650">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="965b8-650">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="965b8-651">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="965b8-651">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="965b8-652">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="965b8-652">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="965b8-653">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="965b8-653">Az.Storage</span></span>
- <span data-ttu-id="965b8-654">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="965b8-654">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="965b8-655">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="965b8-655">Az.Websites</span></span>
- <span data-ttu-id="965b8-656">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="965b8-656">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="965b8-657">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="965b8-657">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="965b8-658">Geral</span><span class="sxs-lookup"><span data-stu-id="965b8-658">General</span></span>

* <span data-ttu-id="965b8-659">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="965b8-659">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="965b8-660">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="965b8-660">Az.Compute</span></span>

* <span data-ttu-id="965b8-661">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="965b8-661">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="965b8-662">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="965b8-662">Az.DataLakeStore</span></span>

* <span data-ttu-id="965b8-663">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="965b8-663">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="965b8-664">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="965b8-664">Az.FrontDoor</span></span>

* <span data-ttu-id="965b8-665">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="965b8-665">Fixed some broken links</span></span>
    - <span data-ttu-id="965b8-666">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="965b8-666">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="965b8-667">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="965b8-667">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="965b8-668">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="965b8-668">Az.RecoveryServices</span></span>

* <span data-ttu-id="965b8-669">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="965b8-669">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="965b8-670">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="965b8-670">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="965b8-671">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="965b8-671">Az.Resources</span></span>

* <span data-ttu-id="965b8-672">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="965b8-672">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="965b8-673">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="965b8-673">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="965b8-674">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="965b8-674">Az.Sql</span></span>

* <span data-ttu-id="965b8-675">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="965b8-675">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="965b8-676">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="965b8-676">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="965b8-677">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="965b8-677">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="965b8-678">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="965b8-678">Az.Storage</span></span>

* <span data-ttu-id="965b8-679">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="965b8-679">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="965b8-680">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="965b8-680">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="965b8-681">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="965b8-681">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="965b8-682">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="965b8-682">Support Static Website configuration</span></span>
    - <span data-ttu-id="965b8-683">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="965b8-683">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="965b8-684">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="965b8-684">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="965b8-685">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="965b8-685">Az.Websites</span></span>

* <span data-ttu-id="965b8-686">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="965b8-686">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="965b8-687">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="965b8-687">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="965b8-688">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="965b8-688">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="965b8-689">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="965b8-689">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="965b8-690">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="965b8-690">Az.ApiManagement</span></span>
* <span data-ttu-id="965b8-691">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="965b8-691">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="965b8-692">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="965b8-692">Az.Automation</span></span>
* <span data-ttu-id="965b8-693">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="965b8-693">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="965b8-694">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="965b8-694">Added Update Management cmdlets</span></span>
* <span data-ttu-id="965b8-695">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="965b8-695">Added Source Control cmdlets</span></span>
* <span data-ttu-id="965b8-696">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="965b8-696">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="965b8-697">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="965b8-697">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="965b8-698">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="965b8-698">Az.Compute</span></span>
* <span data-ttu-id="965b8-699">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="965b8-699">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="965b8-700">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="965b8-700">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="965b8-701">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="965b8-701">Az.ContainerInstance</span></span>
* <span data-ttu-id="965b8-702">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="965b8-702">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="965b8-703">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="965b8-703">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="965b8-704">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="965b8-704">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="965b8-705">Az.Network</span><span class="sxs-lookup"><span data-stu-id="965b8-705">Az.Network</span></span>
* <span data-ttu-id="965b8-706">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="965b8-706">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="965b8-707">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="965b8-707">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="965b8-708">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="965b8-708">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="965b8-709">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="965b8-709">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="965b8-710">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="965b8-710">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="965b8-711">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="965b8-711">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="965b8-712">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="965b8-712">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="965b8-713">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="965b8-713">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="965b8-714">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="965b8-714">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="965b8-715">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="965b8-715">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="965b8-716">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="965b8-716">Az.Relay</span></span>
* <span data-ttu-id="965b8-717">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="965b8-717">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="965b8-718">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="965b8-718">Az.Resources</span></span>
* <span data-ttu-id="965b8-719">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="965b8-719">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="965b8-720">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="965b8-720">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="965b8-721">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="965b8-721">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="965b8-722">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="965b8-722">Az.ServiceFabric</span></span>
* <span data-ttu-id="965b8-723">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="965b8-723">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="965b8-724">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="965b8-724">Az.Sql</span></span>
* <span data-ttu-id="965b8-725">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="965b8-725">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="965b8-726">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="965b8-726">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="965b8-727">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="965b8-727">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="965b8-728">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="965b8-728">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="965b8-729">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="965b8-729">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="965b8-730">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="965b8-730">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="965b8-731">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="965b8-731">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="965b8-732">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="965b8-732">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="965b8-733">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="965b8-733">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="965b8-734">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="965b8-734">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="965b8-735">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="965b8-735">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="965b8-736">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="965b8-736">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="965b8-737">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="965b8-737">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="965b8-738">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="965b8-738">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="965b8-739">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="965b8-739">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="965b8-740">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="965b8-740">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="965b8-741">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="965b8-741">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="965b8-742">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="965b8-742">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="965b8-743">Geral</span><span class="sxs-lookup"><span data-stu-id="965b8-743">General</span></span>
* <span data-ttu-id="965b8-744">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="965b8-744">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="965b8-745">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="965b8-745">Az.Profile</span></span>
* <span data-ttu-id="965b8-746">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="965b8-746">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="965b8-747">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="965b8-747">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="965b8-748">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="965b8-748">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="965b8-749">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="965b8-749">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="965b8-750">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="965b8-750">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="965b8-751">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="965b8-751">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="965b8-752">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="965b8-752">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="965b8-753">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="965b8-753">Az.CognitiveServices</span></span>
* <span data-ttu-id="965b8-754">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="965b8-754">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="965b8-755">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="965b8-755">Az.Compute</span></span>
* <span data-ttu-id="965b8-756">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="965b8-756">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="965b8-757">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="965b8-757">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="965b8-758">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="965b8-758">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="965b8-759">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="965b8-759">Az.DataLakeStore</span></span>
* <span data-ttu-id="965b8-760">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="965b8-760">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="965b8-761">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="965b8-761">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="965b8-762">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="965b8-762">Az.Insights</span></span>
* <span data-ttu-id="965b8-763">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="965b8-763">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="965b8-764">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="965b8-764">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="965b8-765">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="965b8-765">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="965b8-766">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="965b8-766">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="965b8-767">Az.Network</span><span class="sxs-lookup"><span data-stu-id="965b8-767">Az.Network</span></span>
* <span data-ttu-id="965b8-768">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="965b8-768">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="965b8-769">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="965b8-769">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="965b8-770">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="965b8-770">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="965b8-771">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="965b8-771">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="965b8-772">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="965b8-772">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="965b8-773">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="965b8-773">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="965b8-774">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="965b8-774">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="965b8-775">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="965b8-775">Az.PolicyInsights</span></span>
* <span data-ttu-id="965b8-776">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="965b8-776">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="965b8-777">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="965b8-777">Az.Resources</span></span>
* <span data-ttu-id="965b8-778">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="965b8-778">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="965b8-779">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="965b8-779">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="965b8-780">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="965b8-780">Az.ServiceBus</span></span>
* <span data-ttu-id="965b8-781">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="965b8-781">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="965b8-782">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="965b8-782">Az.ServiceFabric</span></span>
* <span data-ttu-id="965b8-783">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="965b8-783">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="965b8-784">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="965b8-784">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="965b8-785">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="965b8-785">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="965b8-786">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="965b8-786">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="965b8-787">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="965b8-787">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="965b8-788">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="965b8-788">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="965b8-789">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="965b8-789">Az.Profile</span></span>
* <span data-ttu-id="965b8-790">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="965b8-790">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="965b8-791">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="965b8-791">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="965b8-792">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="965b8-792">Az.Compute</span></span>
* <span data-ttu-id="965b8-793">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="965b8-793">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="965b8-794">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="965b8-794">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="965b8-795">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="965b8-795">Az.DataLakeStore</span></span>
* <span data-ttu-id="965b8-796">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="965b8-796">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="965b8-797">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="965b8-797">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="965b8-798">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="965b8-798">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="965b8-799">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="965b8-799">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="965b8-800">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="965b8-800">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="965b8-801">Az.Network</span><span class="sxs-lookup"><span data-stu-id="965b8-801">Az.Network</span></span>
* <span data-ttu-id="965b8-802">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="965b8-802">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="965b8-803">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="965b8-803">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="965b8-804">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="965b8-804">Az.Resources</span></span>
* <span data-ttu-id="965b8-805">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="965b8-805">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="965b8-806">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="965b8-806">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="965b8-807">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="965b8-807">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="965b8-808">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="965b8-808">Azure.Storage</span></span>
* <span data-ttu-id="965b8-809">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="965b8-809">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="965b8-810">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="965b8-810">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="965b8-811">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="965b8-811">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="965b8-812">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="965b8-812">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="965b8-813">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="965b8-813">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="965b8-814">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="965b8-814">Az.CognitiveServices</span></span>
* <span data-ttu-id="965b8-815">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="965b8-815">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="965b8-816">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="965b8-816">Az.Compute</span></span>
* <span data-ttu-id="965b8-817">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="965b8-817">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="965b8-818">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="965b8-818">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="965b8-819">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="965b8-819">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="965b8-820">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="965b8-820">Az.DataFactoryV2</span></span>
* <span data-ttu-id="965b8-821">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="965b8-821">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="965b8-822">Az.Network</span><span class="sxs-lookup"><span data-stu-id="965b8-822">Az.Network</span></span>
* <span data-ttu-id="965b8-823">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="965b8-823">Added NetworkProfile functionality.</span></span> <span data-ttu-id="965b8-824">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="965b8-824">new cmdlets added</span></span>
    - <span data-ttu-id="965b8-825">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="965b8-825">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="965b8-826">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="965b8-826">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="965b8-827">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="965b8-827">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="965b8-828">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="965b8-828">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="965b8-829">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="965b8-829">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="965b8-830">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="965b8-830">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="965b8-831">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="965b8-831">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="965b8-832">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="965b8-832">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="965b8-833">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="965b8-833">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="965b8-834">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="965b8-834">Az.RedisCache</span></span>
* <span data-ttu-id="965b8-835">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="965b8-835">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="965b8-836">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="965b8-836">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="965b8-837">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="965b8-837">Az.Resources</span></span>
* <span data-ttu-id="965b8-838">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="965b8-838">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="965b8-839">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="965b8-839">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="965b8-840">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="965b8-840">Az.Sql</span></span>
* <span data-ttu-id="965b8-841">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="965b8-841">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="965b8-842">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="965b8-842">Az.Websites</span></span>
* <span data-ttu-id="965b8-843">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="965b8-843">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="965b8-844">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="965b8-844">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="965b8-845">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="965b8-845">0.2.0 - September 2018</span></span>
 <span data-ttu-id="965b8-846">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="965b8-846">Initial Release</span></span>