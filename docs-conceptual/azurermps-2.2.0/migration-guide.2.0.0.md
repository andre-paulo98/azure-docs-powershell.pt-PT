# <a name="table-of-contents"></a><span data-ttu-id="e9eda-101">Índice</span><span class="sxs-lookup"><span data-stu-id="e9eda-101">Table of Contents</span></span>
1. [<span data-ttu-id="e9eda-102">Remoção de parâmetros Force</span><span class="sxs-lookup"><span data-stu-id="e9eda-102">Removal of Force parameters</span></span>](#removal-of-force-parameters)
2. [<span data-ttu-id="e9eda-103">Alteração de parâmetros Tag</span><span class="sxs-lookup"><span data-stu-id="e9eda-103">Change of Tag parameters</span></span>](#change-of-tag-parameters)
3. [<span data-ttu-id="e9eda-104">Alterações recentes aos cmdlets de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e9eda-104">Breaking changes to Storage cmdlets</span></span>](#breaking-changes-to-storage-cmdlets)
4. [<span data-ttu-id="e9eda-105">Alterações recentes aos cmdlets de AD</span><span class="sxs-lookup"><span data-stu-id="e9eda-105">Breaking changes to AD cmdlets</span></span>](#breaking-changes-to-ad-cmdlets)

## <a name="removal-of-force-parameters"></a><span data-ttu-id="e9eda-106">Remoção de parâmetros Force</span><span class="sxs-lookup"><span data-stu-id="e9eda-106">Removal of Force parameters</span></span>

<span data-ttu-id="e9eda-107">Nesta versão, removemos todos os parâmetros `Force` obsoletos dos cmdlets e os avisos correspondentes segundo os quais o parâmetro iria ser removido numa versão futura.</span><span class="sxs-lookup"><span data-stu-id="e9eda-107">This release, we removed all Obsolete `Force` parameters from cmdlets and the corresponding warnings that the parameter would be removed in a future release.</span></span>

<span data-ttu-id="e9eda-108">Os seguintes cmdlets são afetados por esta alteração:</span><span class="sxs-lookup"><span data-stu-id="e9eda-108">The following cmdlets are affected by this change:</span></span>

<span data-ttu-id="e9eda-109">**ApiManagement**</span><span class="sxs-lookup"><span data-stu-id="e9eda-109">**ApiManagement**</span></span>
- <span data-ttu-id="e9eda-110">Remove-AzureRmApiManagement</span><span class="sxs-lookup"><span data-stu-id="e9eda-110">Remove-AzureRmApiManagement</span></span>
- <span data-ttu-id="e9eda-111">Remove-AzureRmApiManagementApi</span><span class="sxs-lookup"><span data-stu-id="e9eda-111">Remove-AzureRmApiManagementApi</span></span>
- <span data-ttu-id="e9eda-112">Remove-AzureRmApiManagementGroup</span><span class="sxs-lookup"><span data-stu-id="e9eda-112">Remove-AzureRmApiManagementGroup</span></span>
- <span data-ttu-id="e9eda-113">Remove-AzureRmApiManagementLogger</span><span class="sxs-lookup"><span data-stu-id="e9eda-113">Remove-AzureRmApiManagementLogger</span></span>
- <span data-ttu-id="e9eda-114">Remove-AzureRmApiManagementOpenIdConnectProvider</span><span class="sxs-lookup"><span data-stu-id="e9eda-114">Remove-AzureRmApiManagementOpenIdConnectProvider</span></span>
- <span data-ttu-id="e9eda-115">Remove-AzureRmApiManagementOperation</span><span class="sxs-lookup"><span data-stu-id="e9eda-115">Remove-AzureRmApiManagementOperation</span></span>
- <span data-ttu-id="e9eda-116">Remove-AzureRmApiManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="e9eda-116">Remove-AzureRmApiManagementPolicy</span></span>
- <span data-ttu-id="e9eda-117">Remove-AzureRmApiManagementProduct</span><span class="sxs-lookup"><span data-stu-id="e9eda-117">Remove-AzureRmApiManagementProduct</span></span>
- <span data-ttu-id="e9eda-118">Remove-AzureRmApiManagementProperty</span><span class="sxs-lookup"><span data-stu-id="e9eda-118">Remove-AzureRmApiManagementProperty</span></span>
- <span data-ttu-id="e9eda-119">Remove-AzureRmApiManagementSubscription</span><span class="sxs-lookup"><span data-stu-id="e9eda-119">Remove-AzureRmApiManagementSubscription</span></span>
- <span data-ttu-id="e9eda-120">Remove-AzureRmApiManagementUser</span><span class="sxs-lookup"><span data-stu-id="e9eda-120">Remove-AzureRmApiManagementUser</span></span>

<span data-ttu-id="e9eda-121">**Automatização**</span><span class="sxs-lookup"><span data-stu-id="e9eda-121">**Automation**</span></span>
- <span data-ttu-id="e9eda-122">Remove-AzureRmAutomationCertificate</span><span class="sxs-lookup"><span data-stu-id="e9eda-122">Remove-AzureRmAutomationCertificate</span></span>
- <span data-ttu-id="e9eda-123">Remove-AzureRmAutomationCredential</span><span class="sxs-lookup"><span data-stu-id="e9eda-123">Remove-AzureRmAutomationCredential</span></span>
- <span data-ttu-id="e9eda-124">Remove-AzureRmAutomationVariable</span><span class="sxs-lookup"><span data-stu-id="e9eda-124">Remove-AzureRmAutomationVariable</span></span>
- <span data-ttu-id="e9eda-125">Remove-AzureRmAutomationWebhook</span><span class="sxs-lookup"><span data-stu-id="e9eda-125">Remove-AzureRmAutomationWebhook</span></span>

<span data-ttu-id="e9eda-126">**Batch**</span><span class="sxs-lookup"><span data-stu-id="e9eda-126">**Batch**</span></span>
- <span data-ttu-id="e9eda-127">Remove-AzureBatchCertificate</span><span class="sxs-lookup"><span data-stu-id="e9eda-127">Remove-AzureBatchCertificate</span></span>
- <span data-ttu-id="e9eda-128">Remove-AzureBatchComputeNode</span><span class="sxs-lookup"><span data-stu-id="e9eda-128">Remove-AzureBatchComputeNode</span></span>
- <span data-ttu-id="e9eda-129">Remove-AzureBatchComputeNodeUser</span><span class="sxs-lookup"><span data-stu-id="e9eda-129">Remove-AzureBatchComputeNodeUser</span></span>

<span data-ttu-id="e9eda-130">**DataFactories**</span><span class="sxs-lookup"><span data-stu-id="e9eda-130">**DataFactories**</span></span>
- <span data-ttu-id="e9eda-131">Resume-AzureRmDataFactoryPipeline</span><span class="sxs-lookup"><span data-stu-id="e9eda-131">Resume-AzureRmDataFactoryPipeline</span></span>
- <span data-ttu-id="e9eda-132">Set-AzureRmDataFactoryPipelineActivePeriod</span><span class="sxs-lookup"><span data-stu-id="e9eda-132">Set-AzureRmDataFactoryPipelineActivePeriod</span></span>
- <span data-ttu-id="e9eda-133">Suspend-AzureRmDataFactoryPipeline</span><span class="sxs-lookup"><span data-stu-id="e9eda-133">Suspend-AzureRmDataFactoryPipeline</span></span>

<span data-ttu-id="e9eda-134">**DataLakeStore**</span><span class="sxs-lookup"><span data-stu-id="e9eda-134">**DataLakeStore**</span></span>
- <span data-ttu-id="e9eda-135">Remove-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="e9eda-135">Remove-AzureRmDataLakeStoreItemAclEntry</span></span>
- <span data-ttu-id="e9eda-136">Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="e9eda-136">Set-AzureRmDataLakeStoreItemAcl</span></span>
- <span data-ttu-id="e9eda-137">Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="e9eda-137">Set-AzureRmDataLakeStoreItemAclEntry</span></span>
- <span data-ttu-id="e9eda-138">Set-AzureRmDataLakeStoreItemOwner</span><span class="sxs-lookup"><span data-stu-id="e9eda-138">Set-AzureRmDataLakeStoreItemOwner</span></span>

<span data-ttu-id="e9eda-139">**OperationalInsights**</span><span class="sxs-lookup"><span data-stu-id="e9eda-139">**OperationalInsights**</span></span>
- <span data-ttu-id="e9eda-140">Remove-AzureRmOperationalInsightsSavedSearch</span><span class="sxs-lookup"><span data-stu-id="e9eda-140">Remove-AzureRmOperationalInsightsSavedSearch</span></span>

<span data-ttu-id="e9eda-141">**Perfil**</span><span class="sxs-lookup"><span data-stu-id="e9eda-141">**Profile**</span></span>
- <span data-ttu-id="e9eda-142">Remove-AzureRmEnvironment</span><span class="sxs-lookup"><span data-stu-id="e9eda-142">Remove-AzureRmEnvironment</span></span>

<span data-ttu-id="e9eda-143">**RedisCache**</span><span class="sxs-lookup"><span data-stu-id="e9eda-143">**RedisCache**</span></span>
- <span data-ttu-id="e9eda-144">Remove-AzureRmRedisCacheDiagnostics</span><span class="sxs-lookup"><span data-stu-id="e9eda-144">Remove-AzureRmRedisCacheDiagnostics</span></span>

<span data-ttu-id="e9eda-145">**Recursos**</span><span class="sxs-lookup"><span data-stu-id="e9eda-145">**Resources**</span></span>
- <span data-ttu-id="e9eda-146">Register-AzureRmProviderFeature</span><span class="sxs-lookup"><span data-stu-id="e9eda-146">Register-AzureRmProviderFeature</span></span>
- <span data-ttu-id="e9eda-147">Register-AzureRmResourceProvider</span><span class="sxs-lookup"><span data-stu-id="e9eda-147">Register-AzureRmResourceProvider</span></span>
- <span data-ttu-id="e9eda-148">Remove-AzureRmADServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="e9eda-148">Remove-AzureRmADServicePrincipal</span></span>
- <span data-ttu-id="e9eda-149">Remove-AzureRmPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e9eda-149">Remove-AzureRmPolicyAssignment</span></span>
- <span data-ttu-id="e9eda-150">Remove-AzureRmResourceGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="e9eda-150">Remove-AzureRmResourceGroupDeployment</span></span>
- <span data-ttu-id="e9eda-151">Remove-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e9eda-151">Remove-AzureRmRoleAssignment</span></span>
- <span data-ttu-id="e9eda-152">Stop-AzureRmResourceGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="e9eda-152">Stop-AzureRmResourceGroupDeployment</span></span>
- <span data-ttu-id="e9eda-153">Unregister-AzureRmResourceProvider</span><span class="sxs-lookup"><span data-stu-id="e9eda-153">Unregister-AzureRmResourceProvider</span></span>

<span data-ttu-id="e9eda-154">**Armazenamento**</span><span class="sxs-lookup"><span data-stu-id="e9eda-154">**Storage**</span></span>
- <span data-ttu-id="e9eda-155">Remove-AzureStorageContainerStoredAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="e9eda-155">Remove-AzureStorageContainerStoredAccessPolicy</span></span>
- <span data-ttu-id="e9eda-156">Remove-AzureStorageQueueStoredAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="e9eda-156">Remove-AzureStorageQueueStoredAccessPolicy</span></span>
- <span data-ttu-id="e9eda-157">Remove-AzureStorageShareStoredAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="e9eda-157">Remove-AzureStorageShareStoredAccessPolicy</span></span>
- <span data-ttu-id="e9eda-158">Remove-AzureStorageTableStoredAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="e9eda-158">Remove-AzureStorageTableStoredAccessPolicy</span></span>

<span data-ttu-id="e9eda-159">**StreamAnalytics**</span><span class="sxs-lookup"><span data-stu-id="e9eda-159">**StreamAnalytics**</span></span>
- <span data-ttu-id="e9eda-160">Remove-AzureRmStreamAnalyticsFunction</span><span class="sxs-lookup"><span data-stu-id="e9eda-160">Remove-AzureRmStreamAnalyticsFunction</span></span>
- <span data-ttu-id="e9eda-161">Remove-AzureRmStreamAnalyticsInput</span><span class="sxs-lookup"><span data-stu-id="e9eda-161">Remove-AzureRmStreamAnalyticsInput</span></span>
- <span data-ttu-id="e9eda-162">Remove-AzureRmStreamAnalyticsJob</span><span class="sxs-lookup"><span data-stu-id="e9eda-162">Remove-AzureRmStreamAnalyticsJob</span></span>
- <span data-ttu-id="e9eda-163">Remove-AzureRmStreamAnalyticsOutput</span><span class="sxs-lookup"><span data-stu-id="e9eda-163">Remove-AzureRmStreamAnalyticsOutput</span></span>

<span data-ttu-id="e9eda-164">**Tag**</span><span class="sxs-lookup"><span data-stu-id="e9eda-164">**Tag**</span></span>
- <span data-ttu-id="e9eda-165">Remove-AzureRmTag</span><span class="sxs-lookup"><span data-stu-id="e9eda-165">Remove-AzureRmTag</span></span>

<br>

<span data-ttu-id="e9eda-166">Se tiver um script que utiliza qualquer um dos cmdlets acima, a alteração recente pode ser corrigida bastando, para tal, remover o parâmetro `Force`.</span><span class="sxs-lookup"><span data-stu-id="e9eda-166">If you have a script that uses any of the above cmdlets, the breaking change can be fixed by simply removing the `Force` parameter.</span></span>

```powershell
# Old
New-AzureRmResourceGroup -Name $resourceGroupName -Location $location -Force

# New
New-AzureRmResourceGroup -Name $resourceGroupName -Location $location
```

<br>

## <a name="change-of-tag-parameters"></a><span data-ttu-id="e9eda-167">Alteração de parâmetros Tag</span><span class="sxs-lookup"><span data-stu-id="e9eda-167">Change of Tag parameters</span></span>

<span data-ttu-id="e9eda-168">Nesta versão, o nome do parâmetro `Tags` foi alterado para `Tag` e o tipo foi alterado de `Hashtable[]` para `Hashtable`, alterando o formato dos emparelhamentos de chave-valor.</span><span class="sxs-lookup"><span data-stu-id="e9eda-168">This release, the `Tags` parameter name was changed to `Tag`, and the type was changed from `Hashtable[]` to `Hashtable`, changing the format of the key-value pairings.</span></span>

<span data-ttu-id="e9eda-169">Anteriormente, cada entrada em `Hashtable[]` representava um único emparelhamento de chave-valor:</span><span class="sxs-lookup"><span data-stu-id="e9eda-169">Previously, each entry in the `Hashtable[]` represented a single key-value pairing:</span></span>

```powershell
$tags = @{ Name = "test1"; Value = "testval1" }, @{ Name = "test2", Value = "testval2" }
$tags[0].Name  # Key for the first entry, "test1"
$tags[0].Value # Value for the first entry, "testval1"
$tags[1].Name  # Key for the second entry, "test2"
$tags[1].Value # Value for the second entry, "testval2"
```

<span data-ttu-id="e9eda-170">Agora, `Name` e `Value` já não são necessários, dando lugar à criação de emparelhamentos de chave-valor mediante a atribuição de `Key = "Value"` em `Hashtable`:</span><span class="sxs-lookup"><span data-stu-id="e9eda-170">Now, `Name` and `Value` are no longer necessary, allowing for key-value pairings to be created by assigning `Key = "Value"` in the `Hashtable`:</span></span>

```powershell
$tag = @{ test1 = "testval1"; test2 = "testval2" }
$tag["test1"] # Gets the value associated with the key "test1"
$tag["test2"] # Gets the value associated with the key "test2"
```

<span data-ttu-id="e9eda-171">Os seguintes cmdlets são afetados por esta alteração:</span><span class="sxs-lookup"><span data-stu-id="e9eda-171">The following cmdlets are affected by this change:</span></span>

<span data-ttu-id="e9eda-172">**Batch**</span><span class="sxs-lookup"><span data-stu-id="e9eda-172">**Batch**</span></span>
- <span data-ttu-id="e9eda-173">Get-AzureRmBatchAccount</span><span class="sxs-lookup"><span data-stu-id="e9eda-173">Get-AzureRmBatchAccount</span></span>
- <span data-ttu-id="e9eda-174">New-AzureRmBatchAccount</span><span class="sxs-lookup"><span data-stu-id="e9eda-174">New-AzureRmBatchAccount</span></span>
- <span data-ttu-id="e9eda-175">Set-AzureRmBatchAccount</span><span class="sxs-lookup"><span data-stu-id="e9eda-175">Set-AzureRmBatchAccount</span></span>

<span data-ttu-id="e9eda-176">**Computação**</span><span class="sxs-lookup"><span data-stu-id="e9eda-176">**Compute**</span></span>
- <span data-ttu-id="e9eda-177">New-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="e9eda-177">New-AzureRmVM</span></span>
- <span data-ttu-id="e9eda-178">Update-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="e9eda-178">Update-AzureRmVM</span></span>

<span data-ttu-id="e9eda-179">**DataLakeAnalytics**</span><span class="sxs-lookup"><span data-stu-id="e9eda-179">**DataLakeAnalytics**</span></span>
- <span data-ttu-id="e9eda-180">New-AzureRmDataLakeAnalyticsAccount</span><span class="sxs-lookup"><span data-stu-id="e9eda-180">New-AzureRmDataLakeAnalyticsAccount</span></span>
- <span data-ttu-id="e9eda-181">Set-AzureRmDataLakeAnalyticsAccount</span><span class="sxs-lookup"><span data-stu-id="e9eda-181">Set-AzureRmDataLakeAnalyticsAccount</span></span>

<span data-ttu-id="e9eda-182">**DataLakeStore**</span><span class="sxs-lookup"><span data-stu-id="e9eda-182">**DataLakeStore**</span></span>
- <span data-ttu-id="e9eda-183">New-AzureRmDataLakeStoreAccount</span><span class="sxs-lookup"><span data-stu-id="e9eda-183">New-AzureRmDataLakeStoreAccount</span></span>
- <span data-ttu-id="e9eda-184">Set-AzureRmDataLakeStoreAccount</span><span class="sxs-lookup"><span data-stu-id="e9eda-184">Set-AzureRmDataLakeStoreAccount</span></span>

<span data-ttu-id="e9eda-185">**Dns**</span><span class="sxs-lookup"><span data-stu-id="e9eda-185">**Dns**</span></span>
- <span data-ttu-id="e9eda-186">New-AzureRmDnsZone</span><span class="sxs-lookup"><span data-stu-id="e9eda-186">New-AzureRmDnsZone</span></span>
- <span data-ttu-id="e9eda-187">Set-AzureRmDnsZone</span><span class="sxs-lookup"><span data-stu-id="e9eda-187">Set-AzureRmDnsZone</span></span>

<span data-ttu-id="e9eda-188">**KeyVault**</span><span class="sxs-lookup"><span data-stu-id="e9eda-188">**KeyVault**</span></span>
- <span data-ttu-id="e9eda-189">Get-AzureRmKeyVault</span><span class="sxs-lookup"><span data-stu-id="e9eda-189">Get-AzureRmKeyVault</span></span>
- <span data-ttu-id="e9eda-190">New-AzureRmKeyVault</span><span class="sxs-lookup"><span data-stu-id="e9eda-190">New-AzureRmKeyVault</span></span>

<span data-ttu-id="e9eda-191">**Rede**</span><span class="sxs-lookup"><span data-stu-id="e9eda-191">**Network**</span></span>
- <span data-ttu-id="e9eda-192">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="e9eda-192">New-AzureRmApplicationGateway</span></span>
- <span data-ttu-id="e9eda-193">New-AzureRmExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="e9eda-193">New-AzureRmExpressRouteCircuit</span></span>
- <span data-ttu-id="e9eda-194">New-AzureRmLoadBalancer</span><span class="sxs-lookup"><span data-stu-id="e9eda-194">New-AzureRmLoadBalancer</span></span>
- <span data-ttu-id="e9eda-195">New-AzureRmLocalNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="e9eda-195">New-AzureRmLocalNetworkGateway</span></span>
- <span data-ttu-id="e9eda-196">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="e9eda-196">New-AzureRmNetworkInterface</span></span>
- <span data-ttu-id="e9eda-197">New-AzureRmNetworkSecurityGroup</span><span class="sxs-lookup"><span data-stu-id="e9eda-197">New-AzureRmNetworkSecurityGroup</span></span>
- <span data-ttu-id="e9eda-198">New-AzureRmPublicIpAddress</span><span class="sxs-lookup"><span data-stu-id="e9eda-198">New-AzureRmPublicIpAddress</span></span>
- <span data-ttu-id="e9eda-199">New-AzureRmRouteTable</span><span class="sxs-lookup"><span data-stu-id="e9eda-199">New-AzureRmRouteTable</span></span>
- <span data-ttu-id="e9eda-200">New-AzureRmVirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="e9eda-200">New-AzureRmVirtualNetwork</span></span>
- <span data-ttu-id="e9eda-201">New-AzureRmVirtualNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="e9eda-201">New-AzureRmVirtualNetworkGateway</span></span>
- <span data-ttu-id="e9eda-202">New-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="e9eda-202">New-AzureRmVirtualNetworkGatewayConnection</span></span>
- <span data-ttu-id="e9eda-203">New-AzureRmVirtualNetworkPeering</span><span class="sxs-lookup"><span data-stu-id="e9eda-203">New-AzureRmVirtualNetworkPeering</span></span>

<span data-ttu-id="e9eda-204">**Recursos**</span><span class="sxs-lookup"><span data-stu-id="e9eda-204">**Resources**</span></span>
- <span data-ttu-id="e9eda-205">Find-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="e9eda-205">Find-AzureRmResource</span></span>
- <span data-ttu-id="e9eda-206">Find-AzureRmResourceGroup</span><span class="sxs-lookup"><span data-stu-id="e9eda-206">Find-AzureRmResourceGroup</span></span>
- <span data-ttu-id="e9eda-207">New-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="e9eda-207">New-AzureRmResource</span></span>
- <span data-ttu-id="e9eda-208">New-AzureRmResourceGroup</span><span class="sxs-lookup"><span data-stu-id="e9eda-208">New-AzureRmResourceGroup</span></span>
- <span data-ttu-id="e9eda-209">Set-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="e9eda-209">Set-AzureRmResource</span></span>
- <span data-ttu-id="e9eda-210">Set-AzureRmResourceGroup</span><span class="sxs-lookup"><span data-stu-id="e9eda-210">Set-AzureRmResourceGroup</span></span>

<span data-ttu-id="e9eda-211">**SQL**</span><span class="sxs-lookup"><span data-stu-id="e9eda-211">**SQL**</span></span>
- <span data-ttu-id="e9eda-212">New-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="e9eda-212">New-AzureRmSqlDatabase</span></span>
- <span data-ttu-id="e9eda-213">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="e9eda-213">New-AzureRmSqlDatabaseCopy</span></span>
- <span data-ttu-id="e9eda-214">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="e9eda-214">New-AzureRmSqlDatabaseSecondary</span></span>
- <span data-ttu-id="e9eda-215">New-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="e9eda-215">New-AzureRmSqlElasticPool</span></span>
- <span data-ttu-id="e9eda-216">New-AzureRmSqlServer</span><span class="sxs-lookup"><span data-stu-id="e9eda-216">New-AzureRmSqlServer</span></span>
- <span data-ttu-id="e9eda-217">Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="e9eda-217">Set-AzureRmSqlDatabase</span></span>
- <span data-ttu-id="e9eda-218">Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="e9eda-218">Set-AzureRmSqlElasticPool</span></span>
- <span data-ttu-id="e9eda-219">Set-AzureRmSqlServer</span><span class="sxs-lookup"><span data-stu-id="e9eda-219">Set-AzureRmSqlServer</span></span>

<span data-ttu-id="e9eda-220">**Armazenamento**</span><span class="sxs-lookup"><span data-stu-id="e9eda-220">**Storage**</span></span>
- <span data-ttu-id="e9eda-221">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="e9eda-221">New-AzureRmStorageAccount</span></span>
- <span data-ttu-id="e9eda-222">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="e9eda-222">Set-AzureRmStorageAccount</span></span>

<span data-ttu-id="e9eda-223">**TrafficManager**</span><span class="sxs-lookup"><span data-stu-id="e9eda-223">**TrafficManager**</span></span>
- <span data-ttu-id="e9eda-224">New-AzureRmTrafficManagerProfile</span><span class="sxs-lookup"><span data-stu-id="e9eda-224">New-AzureRmTrafficManagerProfile</span></span>

<br>

<span data-ttu-id="e9eda-225">Se tiver um script que utiliza qualquer um dos cmdlets acima, a alteração recente pode ser corrigida bastando, para tal, alterar o parâmetro `Tags` para `Tag` e o parâmetro `Tag` para o novo formato.</span><span class="sxs-lookup"><span data-stu-id="e9eda-225">If you have a script that uses any of the above cmdlets, the breaking change can be fixed by changing the `Tags` parameter to `Tag`, as well as changing the `Tag` to the new format.</span></span>

```powershell
# Old
New-AzureRmResourceGroup -Name $resourceGroupName -Location -location -Tags @{ Name = "testtag"; Value = "testval" }

# New
New-AzureRmResourceGroup -Name $resourceGroupName -Location -location -Tag @{ testtag = "testval" }
```

<br>

## <a name="breaking-changes-to-storage-cmdlets"></a><span data-ttu-id="e9eda-226">Alterações recentes aos cmdlets de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e9eda-226">Breaking changes to Storage cmdlets</span></span>

<span data-ttu-id="e9eda-227">Os seguintes cmdlets foram afetados nesta versão:</span><span class="sxs-lookup"><span data-stu-id="e9eda-227">The following cmdlets were affected this release:</span></span>

<span data-ttu-id="e9eda-228">**Get-AzureRmStorageAccountKey**</span><span class="sxs-lookup"><span data-stu-id="e9eda-228">**Get-AzureRmStorageAccountKey**</span></span>
- <span data-ttu-id="e9eda-229">Agora, o cmdlet devolve uma lista de chaves, em vez de um objeto com propriedades para cada chave</span><span class="sxs-lookup"><span data-stu-id="e9eda-229">The cmdlet now returns a list of keys, rather than an object with properties for each key</span></span>

```powershell
# Old
$key = (Get-AzureRmStorageAccountKey -ResourceGroupName $resourceGroupName -Name $accountName).Key1

# New
$key = (Get-AzureRmStorageAccountKey -ResourceGroupName $resourceGroupName -Name $accountName)[0].Value
```

<span data-ttu-id="e9eda-230">**New-AzureRmStorageAccountKey**</span><span class="sxs-lookup"><span data-stu-id="e9eda-230">**New-AzureRmStorageAccountKey**</span></span>
- <span data-ttu-id="e9eda-231">O nome do campo `StorageAccountRegenerateKeyResponse` na saída deste cmdlet foi mudado para `StorageAccountListKeysResults`, passando agora a ser uma lista de chaves em vez de um objeto com propriedades para cada chave</span><span class="sxs-lookup"><span data-stu-id="e9eda-231">`StorageAccountRegenerateKeyResponse` field in output of this cmdlet is renamed to `StorageAccountListKeysResults`, which is now a list of keys rather than an object with properties for each key</span></span>

```powershell
# Old
$key = (New-AzureRmStorageAccountKey -ResourceGroupName $resourceGroupName -Name $accountName).StorageAccountKeys.Key1

# New
$key = (New-AzureRmStorageAccountKey -ResourceGroupName $resourceGroupName -Name $accountName).Keys[0].Value
```

<span data-ttu-id="e9eda-232">**New/Get/Set-AzureRmStorageAccount**</span><span class="sxs-lookup"><span data-stu-id="e9eda-232">**New/Get/Set-AzureRmStorageAccount**</span></span>
- <span data-ttu-id="e9eda-233">O nome do campo `AccountType` na saída deste cmdlet foi mudado para `Sku.Name`</span><span class="sxs-lookup"><span data-stu-id="e9eda-233">`AccountType` field in output of this cmdlet is renamed to `Sku.Name`</span></span>
- <span data-ttu-id="e9eda-234">O tipo de saída para blob/tabela/fila/ficheiro de PrimaryEndpoints/Pontos finais secundários foi alterado de `Uri` para `String`</span><span class="sxs-lookup"><span data-stu-id="e9eda-234">Output type for PrimaryEndpoints/Secondary endpoints blob/table/queue/file changed from `Uri` to `String`</span></span>

```powershell
# Old
$accountType = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).AccountType

# New
$accountType = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).Sku.Name
```

```powershell
# Old 
$blobEndpoint = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).PrimaryEndpoints.Blob.ToString()
$blobEndpoint = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).PrimaryEndpoints.Blob.AbsolutePath

# New
$blobEndpoint = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).PrimaryEndpoints.Blob.ToString()
$blobEndpoint = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).PrimaryEndpoints.Blob
```

<br>

## <a name="breaking-changes-to-ad-cmdlets"></a><span data-ttu-id="e9eda-235">Alterações recentes aos cmdlets de AD</span><span class="sxs-lookup"><span data-stu-id="e9eda-235">Breaking changes to AD cmdlets</span></span>

<span data-ttu-id="e9eda-236">Os seguintes cmdlets foram afetados nesta versão:</span><span class="sxs-lookup"><span data-stu-id="e9eda-236">The following cmdlets were affected this release:</span></span>

<span data-ttu-id="e9eda-237">**Get-AzureRMADServicePrincipal**</span><span class="sxs-lookup"><span data-stu-id="e9eda-237">**Get-AzureRMADServicePrincipal**</span></span>
- <span data-ttu-id="e9eda-238">O nome do campo `ServicePrincipalName` na saída deste cmdlet foi mudado para `ServicePrincipalNames` e é agora uma coleção.</span><span class="sxs-lookup"><span data-stu-id="e9eda-238">`ServicePrincipalName` field in output of this cmdlet is renamed to `ServicePrincipalNames` and is now a collection.</span></span> <span data-ttu-id="e9eda-239">Apresenta agora `ApplicationId` também como um dos SPNs, juntamente com o identifierUri.</span><span class="sxs-lookup"><span data-stu-id="e9eda-239">It now displays `ApplicationId` also as one of the SPN, along with the identifierUri.</span></span>

```powershell
# Old
$servicePrincipals = Get-AzureRmADServicePrincipal -SearchString $displayName
$spn = $servicePrincipals[0].ServicePrincipalName

# New
$servicePrincipals = Get-AzureRmADServicePrincipal -SearchString $displayName
$spn = $servicePrincipals[0].ServicePrincipalNames[0]
```

<span data-ttu-id="e9eda-240">**Get-AzureRmADApplication**</span><span class="sxs-lookup"><span data-stu-id="e9eda-240">**Get-AzureRmADApplication**</span></span>
- <span data-ttu-id="e9eda-241">O nome do parâmetro `ApplicationObjectId` foi mudado para `ObjectId`.</span><span class="sxs-lookup"><span data-stu-id="e9eda-241">Parameter `ApplicationObjectId` is renamed to `ObjectId`.</span></span>
- <span data-ttu-id="e9eda-242">Na saída deste cmdlet, o nome de `ApplicationObjectId` foi mudado para `ObjectId`.</span><span class="sxs-lookup"><span data-stu-id="e9eda-242">In output of this cmdlet, `ApplicationObjectId` is renamed to `ObjectId`.</span></span>

```powershell
# Old
$app = Get-AzureRmADApplication -ApplicationObjectId $applicationObjectId
$objectId = $app.ApplicationObjectId

# New
$app = Get-AzureRmADApplication -ObjectId $objectId
$objectId = $app.ObjectId
```

<span data-ttu-id="e9eda-243">**Remove-AzureRmADApplication**</span><span class="sxs-lookup"><span data-stu-id="e9eda-243">**Remove-AzureRmADApplication**</span></span>
- <span data-ttu-id="e9eda-244">O nome do parâmetro `ApplicationObjectId` foi mudado para `ObjectId`.</span><span class="sxs-lookup"><span data-stu-id="e9eda-244">Parameter `ApplicationObjectId` is renamed to `ObjectId`.</span></span>

```powershell
# Old
$app = Remove-AzureRmADApplication -ApplicationObjectId $applicationObjectId -Force

# New
$app = Remove-AzureRmADApplication -ObjectId $objectId -Force
```

<span data-ttu-id="e9eda-245">**New-AzureRmADApplication**</span><span class="sxs-lookup"><span data-stu-id="e9eda-245">**New-AzureRmADApplication**</span></span>
- <span data-ttu-id="e9eda-246">Na saída deste cmdlet, o nome de `ApplicationObjectId` foi mudado para `ObjectId`.</span><span class="sxs-lookup"><span data-stu-id="e9eda-246">In output of this cmdlet, `ApplicationObjectId` is renamed to `ObjectId`.</span></span>
- <span data-ttu-id="e9eda-247">Os parâmetros `KeyValue`, `KeyUsage` e `KeyType` foram removidos.</span><span class="sxs-lookup"><span data-stu-id="e9eda-247">`KeyValue`, `KeyUsage`, `KeyType` parameters are removed.</span></span>

```powershell
# Old
$app = New-AzureRmADApplication -DisplayName $displayName -HomePage $homePage -IdentifierUris $identifierUris -KeyValue $kv -KeyType $kt -KeyUsage $ku
$id = $app.ApplicationObjectId

# New
$app = New-AzureRmADApplication -DisplayName $displayName -HomePage $homePage -IdentifierUris $identifierUris
$id = $app.ObjectId
New-AzureRmADAppCredential -ObjectId $id -Password $kv
```

<span data-ttu-id="e9eda-248">**Get-AzureRmADGroup**</span><span class="sxs-lookup"><span data-stu-id="e9eda-248">**Get-AzureRmADGroup**</span></span>
- <span data-ttu-id="e9eda-249">O campo `Mail` foi removido da saída.</span><span class="sxs-lookup"><span data-stu-id="e9eda-249">`Mail` field is removed from the output.</span></span>

<span data-ttu-id="e9eda-250">**Get-AzureRmADUser**</span><span class="sxs-lookup"><span data-stu-id="e9eda-250">**Get-AzureRmADUser**</span></span>
- <span data-ttu-id="e9eda-251">O campo `Mail` foi removido da saída.</span><span class="sxs-lookup"><span data-stu-id="e9eda-251">`Mail` field is removed from the output.</span></span>

<span data-ttu-id="e9eda-252">**New-AzureRmADServicePrincipal**</span><span class="sxs-lookup"><span data-stu-id="e9eda-252">**New-AzureRmADServicePrincipal**</span></span>
- <span data-ttu-id="e9eda-253">O parâmetro `DisableAccount` foi removido.</span><span class="sxs-lookup"><span data-stu-id="e9eda-253">Removed `DisableAccount` parameter.</span></span>

```powershell
# Old
$servicePrincipal = New-AzureRmADServicePrincipal -DisplayName $displayName -Password $password -DisableAccount true

# New
$servicePrincipal = New-AzureRmADServicePrincipal -DisplayName $displayName -Password $password
Remove-AzureRmADServicePrincipal -ObjectId $servicePrincipal.ObjectId
```