## <a name="100---december-2018"></a><span data-ttu-id="f8102-101">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="f8102-101">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="f8102-102">Geral</span><span class="sxs-lookup"><span data-stu-id="f8102-102">General</span></span>

- <span data-ttu-id="f8102-103">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="f8102-103">General Availability of Az Module</span></span>
- <span data-ttu-id="f8102-104">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="f8102-104">Online help for each module</span></span>
- <span data-ttu-id="f8102-105">Para obter mais detalhes e um mapa, consulte a [página de Anúncio do módulo Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="f8102-105">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="f8102-106">Consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="f8102-106">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="f8102-107">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="f8102-107">Az.Accounts</span></span>
- <span data-ttu-id="f8102-108">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="f8102-108">Changed from Az.Profile</span></span>
- <span data-ttu-id="f8102-109">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="f8102-109">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="f8102-110">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="f8102-110">Az.ApiManagement</span></span>
- <span data-ttu-id="f8102-111">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="f8102-111">Fixes for #7002</span></span>
- <span data-ttu-id="f8102-112">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="f8102-112">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="f8102-113">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="f8102-113">Az.Batch</span></span>
- <span data-ttu-id="f8102-114">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="f8102-114">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="f8102-115">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="f8102-115">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="f8102-116">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="f8102-116">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="f8102-117">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="f8102-117">Az.Billing</span></span>
- <span data-ttu-id="f8102-118">Combina os cmdlets Billing, Consumption e UsageAggregates; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="f8102-118">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="f8102-119">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="f8102-119">Az.CognitivServices</span></span>
- <span data-ttu-id="f8102-120">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="f8102-120">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="f8102-121">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="f8102-121">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="f8102-122">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="f8102-122">Az.ContainerInstance</span></span>
- <span data-ttu-id="f8102-123">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="f8102-123">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="f8102-124">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="f8102-124">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="f8102-125">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="f8102-125">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="f8102-126">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="f8102-126">Az.DataLakeStore</span></span>
- <span data-ttu-id="f8102-127">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="f8102-127">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="f8102-128">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="f8102-128">Az.Monitor</span></span>
- <span data-ttu-id="f8102-129">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="f8102-129">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="f8102-130">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="f8102-130">Az.KeyVault</span></span>
- <span data-ttu-id="f8102-131">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="f8102-131">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="f8102-132">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="f8102-132">Az.MachineLearning</span></span>
- <span data-ttu-id="f8102-133">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="f8102-133">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="f8102-134">Az.Media</span><span class="sxs-lookup"><span data-stu-id="f8102-134">Az.Media</span></span>
- <span data-ttu-id="f8102-135">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="f8102-135">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="f8102-136">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f8102-136">Az.Network</span></span>
<span data-ttu-id="f8102-137">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="f8102-137">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="f8102-138">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="f8102-138">New cmdlets added:</span></span>
        - <span data-ttu-id="f8102-139">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="f8102-139">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="f8102-140">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="f8102-140">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="f8102-141">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="f8102-141">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="f8102-142">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="f8102-142">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="f8102-143">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="f8102-143">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="f8102-144">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="f8102-144">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="f8102-145">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="f8102-145">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="f8102-146">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8102-146">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="f8102-147">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="f8102-147">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="f8102-148">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="f8102-148">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="f8102-149">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="f8102-149">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="f8102-150">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="f8102-150">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="f8102-151">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="f8102-151">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="f8102-152">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="f8102-152">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="f8102-153">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="f8102-153">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="f8102-154">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="f8102-154">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="f8102-155">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="f8102-155">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="f8102-156">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="f8102-156">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="f8102-157">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="f8102-157">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="f8102-158">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="f8102-158">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="f8102-159">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="f8102-159">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="f8102-160">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="f8102-160">Az.OperationalInsights</span></span>
- <span data-ttu-id="f8102-161">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="f8102-161">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="f8102-162">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="f8102-162">Az.Profile</span></span>
- <span data-ttu-id="f8102-163">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="f8102-163">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="f8102-164">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="f8102-164">Az.RecoveryServices</span></span>
- <span data-ttu-id="f8102-165">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="f8102-165">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="f8102-166">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f8102-166">Az.Resources</span></span>
- <span data-ttu-id="f8102-167">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="f8102-167">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="f8102-168">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f8102-168">Az.ServiceFabric</span></span>
- <span data-ttu-id="f8102-169">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="f8102-169">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="f8102-170">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="f8102-170">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="f8102-171">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="f8102-171">Az.SIgnalR</span></span>
- <span data-ttu-id="f8102-172">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="f8102-172">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="f8102-173">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f8102-173">Az.Sql</span></span>
- <span data-ttu-id="f8102-174">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="f8102-174">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="f8102-175">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="f8102-175">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="f8102-176">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="f8102-176">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="f8102-177">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="f8102-177">Az.Storage</span></span>
- <span data-ttu-id="f8102-178">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="f8102-178">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="f8102-179">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="f8102-179">Az.Websites</span></span>
- <span data-ttu-id="f8102-180">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="f8102-180">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="f8102-181">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="f8102-181">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="f8102-182">Geral</span><span class="sxs-lookup"><span data-stu-id="f8102-182">General</span></span>

* <span data-ttu-id="f8102-183">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="f8102-183">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="f8102-184">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f8102-184">Az.Compute</span></span>

* <span data-ttu-id="f8102-185">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="f8102-185">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="f8102-186">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="f8102-186">Az.DataLakeStore</span></span>

* <span data-ttu-id="f8102-187">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="f8102-187">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="f8102-188">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="f8102-188">Az.FrontDoor</span></span>

* <span data-ttu-id="f8102-189">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="f8102-189">Fixed some broken links</span></span>
    - <span data-ttu-id="f8102-190">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="f8102-190">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="f8102-191">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="f8102-191">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="f8102-192">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="f8102-192">Az.RecoveryServices</span></span>

* <span data-ttu-id="f8102-193">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="f8102-193">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="f8102-194">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="f8102-194">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="f8102-195">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f8102-195">Az.Resources</span></span>

* <span data-ttu-id="f8102-196">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="f8102-196">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="f8102-197">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="f8102-197">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="f8102-198">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f8102-198">Az.Sql</span></span>

* <span data-ttu-id="f8102-199">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="f8102-199">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="f8102-200">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="f8102-200">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="f8102-201">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="f8102-201">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="f8102-202">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="f8102-202">Az.Storage</span></span>

* <span data-ttu-id="f8102-203">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="f8102-203">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="f8102-204">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="f8102-204">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="f8102-205">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="f8102-205">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="f8102-206">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="f8102-206">Support Static Website configuration</span></span>
    - <span data-ttu-id="f8102-207">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="f8102-207">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="f8102-208">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="f8102-208">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="f8102-209">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="f8102-209">Az.Websites</span></span>

* <span data-ttu-id="f8102-210">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="f8102-210">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="f8102-211">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="f8102-211">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="f8102-212">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="f8102-212">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="f8102-213">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="f8102-213">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="f8102-214">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="f8102-214">Az.ApiManagement</span></span>
* <span data-ttu-id="f8102-215">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="f8102-215">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="f8102-216">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="f8102-216">Az.Automation</span></span>
* <span data-ttu-id="f8102-217">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="f8102-217">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="f8102-218">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="f8102-218">Added Update Management cmdlets</span></span>
* <span data-ttu-id="f8102-219">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="f8102-219">Added Source Control cmdlets</span></span>
* <span data-ttu-id="f8102-220">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="f8102-220">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="f8102-221">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="f8102-221">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="f8102-222">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f8102-222">Az.Compute</span></span>
* <span data-ttu-id="f8102-223">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="f8102-223">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="f8102-224">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="f8102-224">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="f8102-225">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="f8102-225">Az.ContainerInstance</span></span>
* <span data-ttu-id="f8102-226">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="f8102-226">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="f8102-227">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="f8102-227">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="f8102-228">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="f8102-228">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="f8102-229">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f8102-229">Az.Network</span></span>
* <span data-ttu-id="f8102-230">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="f8102-230">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="f8102-231">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="f8102-231">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="f8102-232">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="f8102-232">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="f8102-233">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="f8102-233">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="f8102-234">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="f8102-234">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="f8102-235">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="f8102-235">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="f8102-236">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="f8102-236">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="f8102-237">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="f8102-237">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="f8102-238">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="f8102-238">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="f8102-239">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="f8102-239">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="f8102-240">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="f8102-240">Az.Relay</span></span>
* <span data-ttu-id="f8102-241">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="f8102-241">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="f8102-242">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f8102-242">Az.Resources</span></span>
* <span data-ttu-id="f8102-243">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="f8102-243">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="f8102-244">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="f8102-244">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="f8102-245">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="f8102-245">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="f8102-246">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f8102-246">Az.ServiceFabric</span></span>
* <span data-ttu-id="f8102-247">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="f8102-247">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="f8102-248">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f8102-248">Az.Sql</span></span>
* <span data-ttu-id="f8102-249">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="f8102-249">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="f8102-250">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="f8102-250">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="f8102-251">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="f8102-251">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="f8102-252">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="f8102-252">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="f8102-253">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="f8102-253">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="f8102-254">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="f8102-254">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="f8102-255">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="f8102-255">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="f8102-256">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="f8102-256">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="f8102-257">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="f8102-257">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="f8102-258">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="f8102-258">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="f8102-259">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="f8102-259">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="f8102-260">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="f8102-260">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="f8102-261">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="f8102-261">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="f8102-262">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="f8102-262">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="f8102-263">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="f8102-263">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="f8102-264">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="f8102-264">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="f8102-265">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="f8102-265">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="f8102-266">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="f8102-266">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="f8102-267">Geral</span><span class="sxs-lookup"><span data-stu-id="f8102-267">General</span></span>
* <span data-ttu-id="f8102-268">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="f8102-268">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="f8102-269">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="f8102-269">Az.Profile</span></span>
* <span data-ttu-id="f8102-270">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="f8102-270">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="f8102-271">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="f8102-271">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="f8102-272">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="f8102-272">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="f8102-273">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="f8102-273">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="f8102-274">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="f8102-274">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="f8102-275">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="f8102-275">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="f8102-276">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="f8102-276">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="f8102-277">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="f8102-277">Az.CognitiveServices</span></span>
* <span data-ttu-id="f8102-278">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="f8102-278">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f8102-279">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f8102-279">Az.Compute</span></span>
* <span data-ttu-id="f8102-280">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="f8102-280">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="f8102-281">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="f8102-281">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="f8102-282">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="f8102-282">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="f8102-283">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="f8102-283">Az.DataLakeStore</span></span>
* <span data-ttu-id="f8102-284">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="f8102-284">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="f8102-285">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="f8102-285">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="f8102-286">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="f8102-286">Az.Insights</span></span>
* <span data-ttu-id="f8102-287">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="f8102-287">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="f8102-288">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="f8102-288">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="f8102-289">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="f8102-289">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="f8102-290">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="f8102-290">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="f8102-291">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f8102-291">Az.Network</span></span>
* <span data-ttu-id="f8102-292">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="f8102-292">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="f8102-293">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="f8102-293">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="f8102-294">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="f8102-294">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="f8102-295">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="f8102-295">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="f8102-296">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="f8102-296">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="f8102-297">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="f8102-297">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="f8102-298">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="f8102-298">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="f8102-299">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="f8102-299">Az.PolicyInsights</span></span>
* <span data-ttu-id="f8102-300">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="f8102-300">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="f8102-301">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f8102-301">Az.Resources</span></span>
* <span data-ttu-id="f8102-302">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="f8102-302">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="f8102-303">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="f8102-303">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="f8102-304">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f8102-304">Az.ServiceBus</span></span>
* <span data-ttu-id="f8102-305">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="f8102-305">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="f8102-306">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f8102-306">Az.ServiceFabric</span></span>
* <span data-ttu-id="f8102-307">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="f8102-307">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="f8102-308">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="f8102-308">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="f8102-309">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="f8102-309">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="f8102-310">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="f8102-310">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="f8102-311">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="f8102-311">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="f8102-312">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="f8102-312">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="f8102-313">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="f8102-313">Az.Profile</span></span>
* <span data-ttu-id="f8102-314">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="f8102-314">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="f8102-315">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="f8102-315">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f8102-316">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f8102-316">Az.Compute</span></span>
* <span data-ttu-id="f8102-317">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="f8102-317">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="f8102-318">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="f8102-318">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="f8102-319">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="f8102-319">Az.DataLakeStore</span></span>
* <span data-ttu-id="f8102-320">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="f8102-320">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="f8102-321">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="f8102-321">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="f8102-322">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="f8102-322">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="f8102-323">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="f8102-323">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="f8102-324">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="f8102-324">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="f8102-325">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f8102-325">Az.Network</span></span>
* <span data-ttu-id="f8102-326">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="f8102-326">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="f8102-327">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="f8102-327">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="f8102-328">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f8102-328">Az.Resources</span></span>
* <span data-ttu-id="f8102-329">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="f8102-329">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="f8102-330">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="f8102-330">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="f8102-331">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="f8102-331">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="f8102-332">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="f8102-332">Azure.Storage</span></span>
* <span data-ttu-id="f8102-333">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="f8102-333">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="f8102-334">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="f8102-334">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="f8102-335">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="f8102-335">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="f8102-336">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="f8102-336">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="f8102-337">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="f8102-337">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="f8102-338">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="f8102-338">Az.CognitiveServices</span></span>
* <span data-ttu-id="f8102-339">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="f8102-339">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f8102-340">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f8102-340">Az.Compute</span></span>
* <span data-ttu-id="f8102-341">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="f8102-341">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="f8102-342">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="f8102-342">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="f8102-343">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="f8102-343">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="f8102-344">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="f8102-344">Az.DataFactoryV2</span></span>
* <span data-ttu-id="f8102-345">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="f8102-345">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="f8102-346">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f8102-346">Az.Network</span></span>
* <span data-ttu-id="f8102-347">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="f8102-347">Added NetworkProfile functionality.</span></span> <span data-ttu-id="f8102-348">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="f8102-348">new cmdlets added</span></span>
    - <span data-ttu-id="f8102-349">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f8102-349">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="f8102-350">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f8102-350">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="f8102-351">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f8102-351">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="f8102-352">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f8102-352">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="f8102-353">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="f8102-353">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="f8102-354">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="f8102-354">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="f8102-355">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="f8102-355">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="f8102-356">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="f8102-356">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="f8102-357">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="f8102-357">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="f8102-358">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="f8102-358">Az.RedisCache</span></span>
* <span data-ttu-id="f8102-359">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="f8102-359">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="f8102-360">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="f8102-360">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="f8102-361">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f8102-361">Az.Resources</span></span>
* <span data-ttu-id="f8102-362">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="f8102-362">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="f8102-363">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="f8102-363">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="f8102-364">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f8102-364">Az.Sql</span></span>
* <span data-ttu-id="f8102-365">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="f8102-365">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="f8102-366">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="f8102-366">Az.Websites</span></span>
* <span data-ttu-id="f8102-367">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="f8102-367">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="f8102-368">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="f8102-368">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="f8102-369">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="f8102-369">0.2.0 - September 2018</span></span>
 <span data-ttu-id="f8102-370">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="f8102-370">Initial Release</span></span>