## <a name="140---february-2019"></a><span data-ttu-id="050e5-101">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="050e5-101">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="050e5-102">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="050e5-102">Az.AnalysisServices</span></span>
* <span data-ttu-id="050e5-103">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="050e5-103">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="050e5-104">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="050e5-104">Az.Automation</span></span>
* <span data-ttu-id="050e5-105">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="050e5-105">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="050e5-106">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="050e5-106">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="050e5-107">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="050e5-107">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="050e5-108">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="050e5-108">Az.CognitiveServices</span></span>
* <span data-ttu-id="050e5-109">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="050e5-109">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="050e5-110">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="050e5-110">Az.Compute</span></span>
* <span data-ttu-id="050e5-111">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="050e5-111">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="050e5-112">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="050e5-112">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="050e5-113">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="050e5-113">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="050e5-114">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="050e5-114">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="050e5-115">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="050e5-115">Az.DataLakeStore</span></span>
* <span data-ttu-id="050e5-116">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="050e5-116">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="050e5-117">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="050e5-117">Az.EventHub</span></span>
* <span data-ttu-id="050e5-118">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="050e5-118">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="050e5-119">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="050e5-119">Az.KeyVault</span></span>
* <span data-ttu-id="050e5-120">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="050e5-120">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="050e5-121">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="050e5-121">Az.LogicApp</span></span>
* <span data-ttu-id="050e5-122">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="050e5-122">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="050e5-123">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="050e5-123">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="050e5-124">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="050e5-124">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="050e5-125">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="050e5-125">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="050e5-126">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="050e5-126">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="050e5-127">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="050e5-127">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="050e5-128">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="050e5-128">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="050e5-129">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="050e5-129">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="050e5-130">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="050e5-130">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="050e5-131">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="050e5-131">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="050e5-132">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="050e5-132">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="050e5-133">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="050e5-133">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="050e5-134">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="050e5-134">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="050e5-135">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="050e5-135">Az.Monitor</span></span>
* <span data-ttu-id="050e5-136">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="050e5-136">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="050e5-137">Az.Network</span><span class="sxs-lookup"><span data-stu-id="050e5-137">Az.Network</span></span>
* <span data-ttu-id="050e5-138">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="050e5-138">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="050e5-139">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="050e5-139">Az.OperationalInsights</span></span>
* <span data-ttu-id="050e5-140">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="050e5-140">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="050e5-141">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="050e5-141">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="050e5-142">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="050e5-142">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="050e5-143">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="050e5-143">Az.Resources</span></span>
* <span data-ttu-id="050e5-144">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="050e5-144">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="050e5-145">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="050e5-145">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="050e5-146">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="050e5-146">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="050e5-147">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="050e5-147">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="050e5-148">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="050e5-148">Az.Sql</span></span>
* <span data-ttu-id="050e5-149">Suporte adicionado para a camada Hiperescala da BD SQL</span><span class="sxs-lookup"><span data-stu-id="050e5-149">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="050e5-150">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="050e5-150">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="050e5-151">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="050e5-151">Az.Websites</span></span>
* <span data-ttu-id="050e5-152">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="050e5-152">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="050e5-153">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="050e5-153">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="050e5-154">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="050e5-154">Az.Accounts</span></span>
* <span data-ttu-id="050e5-155">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="050e5-155">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="050e5-156">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="050e5-156">Az.AnalysisServices</span></span>
<span data-ttu-id="050e5-157">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="050e5-157">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="050e5-158">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="050e5-158">Az.Compute</span></span>
* <span data-ttu-id="050e5-159">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="050e5-159">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="050e5-160">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="050e5-160">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="050e5-161">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="050e5-161">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="050e5-162">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="050e5-162">Az.RecoveryServices</span></span>
<span data-ttu-id="050e5-163">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="050e5-163">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="050e5-164">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="050e5-164">Az.Resources</span></span>
* <span data-ttu-id="050e5-165">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="050e5-165">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="050e5-166">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="050e5-166">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="050e5-167">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="050e5-167">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="050e5-168">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="050e5-168">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="050e5-169">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="050e5-169">Az.Sql</span></span>
* <span data-ttu-id="050e5-170">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="050e5-170">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="050e5-171">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="050e5-171">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="050e5-172">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="050e5-172">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="050e5-173">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="050e5-173">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="050e5-174">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="050e5-174">Az.Accounts</span></span>
* <span data-ttu-id="050e5-175">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="050e5-175">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="050e5-176">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="050e5-176">Az.AnalysisServices</span></span>
* <span data-ttu-id="050e5-177">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="050e5-177">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="050e5-178">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="050e5-178">Az.RecoveryServices</span></span>
* <span data-ttu-id="050e5-179">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="050e5-179">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="050e5-180">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="050e5-180">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="050e5-181">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="050e5-181">Az.Accounts</span></span>
* <span data-ttu-id="050e5-182">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="050e5-182">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="050e5-183">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="050e5-183">Update incorrect online help URLs</span></span>
* <span data-ttu-id="050e5-184">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="050e5-184">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="050e5-185">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="050e5-185">Az.Aks</span></span>
* <span data-ttu-id="050e5-186">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="050e5-186">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="050e5-187">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="050e5-187">Az.Automation</span></span>
* <span data-ttu-id="050e5-188">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="050e5-188">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="050e5-189">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="050e5-189">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="050e5-190">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="050e5-190">Az.Cdn</span></span>
* <span data-ttu-id="050e5-191">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="050e5-191">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="050e5-192">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="050e5-192">Az.Compute</span></span>
* <span data-ttu-id="050e5-193">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="050e5-193">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="050e5-194">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="050e5-194">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="050e5-195">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="050e5-195">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="050e5-196">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="050e5-196">Az.ContainerRegistry</span></span>
* <span data-ttu-id="050e5-197">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="050e5-197">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="050e5-198">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="050e5-198">Az.DataFactory</span></span>
* <span data-ttu-id="050e5-199">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="050e5-199">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="050e5-200">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="050e5-200">Az.DataLakeStore</span></span>
* <span data-ttu-id="050e5-201">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="050e5-201">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="050e5-202">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="050e5-202">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="050e5-203">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="050e5-203">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="050e5-204">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="050e5-204">Az.IotHub</span></span>
* <span data-ttu-id="050e5-205">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="050e5-205">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="050e5-206">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="050e5-206">Az.KeyVault</span></span>
* <span data-ttu-id="050e5-207">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="050e5-207">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="050e5-208">Az.Network</span><span class="sxs-lookup"><span data-stu-id="050e5-208">Az.Network</span></span>
* <span data-ttu-id="050e5-209">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="050e5-209">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="050e5-210">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="050e5-210">Az.Resources</span></span>
* <span data-ttu-id="050e5-211">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="050e5-211">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="050e5-212">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="050e5-212">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="050e5-213">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="050e5-213">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="050e5-214">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="050e5-214">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="050e5-215">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="050e5-215">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="050e5-216">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="050e5-216">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="050e5-217">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="050e5-217">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="050e5-218">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="050e5-218">Az.ServiceFabric</span></span>
* <span data-ttu-id="050e5-219">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="050e5-219">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="050e5-220">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="050e5-220">Fix some error messages.</span></span>
* <span data-ttu-id="050e5-221">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="050e5-221">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="050e5-222">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="050e5-222">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="050e5-223">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="050e5-223">Az.SignalR</span></span>
* <span data-ttu-id="050e5-224">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="050e5-224">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="050e5-225">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="050e5-225">Az.Sql</span></span>
* <span data-ttu-id="050e5-226">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="050e5-226">Update incorrect online help URLs</span></span>
* <span data-ttu-id="050e5-227">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="050e5-227">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="050e5-228">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="050e5-228">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="050e5-229">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="050e5-229">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="050e5-230">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="050e5-230">Az.Storage</span></span>
* <span data-ttu-id="050e5-231">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="050e5-231">Update incorrect online help URLs</span></span>
* <span data-ttu-id="050e5-232">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="050e5-232">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="050e5-233">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="050e5-233">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="050e5-234">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="050e5-234">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="050e5-235">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="050e5-235">Az.TrafficManager</span></span>
* <span data-ttu-id="050e5-236">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="050e5-236">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="050e5-237">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="050e5-237">Az.Websites</span></span>
* <span data-ttu-id="050e5-238">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="050e5-238">Update incorrect online help URLs</span></span>
* <span data-ttu-id="050e5-239">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="050e5-239">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="050e5-240">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="050e5-240">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="050e5-241">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="050e5-241">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="050e5-242">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="050e5-242">Az.Accounts</span></span>
* <span data-ttu-id="050e5-243">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="050e5-243">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="050e5-244">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="050e5-244">Az.Compute</span></span>
* <span data-ttu-id="050e5-245">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="050e5-245">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="050e5-246">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="050e5-246">Updated the description of ID in help files</span></span>
* <span data-ttu-id="050e5-247">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="050e5-247">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="050e5-248">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="050e5-248">Az.DataLakeStore</span></span>
* <span data-ttu-id="050e5-249">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="050e5-249">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="050e5-250">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="050e5-250">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="050e5-251">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="050e5-251">Az.EventGrid</span></span>
* <span data-ttu-id="050e5-252">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="050e5-252">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="050e5-253">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="050e5-253">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="050e5-254">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="050e5-254">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="050e5-255">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="050e5-255">Event Time-To-Live,</span></span>
        - <span data-ttu-id="050e5-256">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="050e5-256">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="050e5-257">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="050e5-257">Dead letter endpoint.</span></span>
    - <span data-ttu-id="050e5-258">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="050e5-258">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="050e5-259">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="050e5-259">Event Time-To-Live,</span></span>
        - <span data-ttu-id="050e5-260">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="050e5-260">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="050e5-261">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="050e5-261">Dead letter endpoint.</span></span>
* <span data-ttu-id="050e5-262">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="050e5-262">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="050e5-263">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="050e5-263">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="050e5-264">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="050e5-264">Az.IotHub</span></span>
* <span data-ttu-id="050e5-265">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="050e5-265">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="050e5-266">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="050e5-266">Az.LogicApp</span></span>
* <span data-ttu-id="050e5-267">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="050e5-267">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="050e5-268">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="050e5-268">Az.Resources</span></span>
* <span data-ttu-id="050e5-269">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="050e5-269">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="050e5-270">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="050e5-270">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="050e5-271">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="050e5-271">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="050e5-272">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="050e5-272">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="050e5-273">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="050e5-273">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="050e5-274">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="050e5-274">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="050e5-275">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="050e5-275">Az.SignalR</span></span>
* <span data-ttu-id="050e5-276">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="050e5-276">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="050e5-277">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="050e5-277">Az.Sql</span></span>
* <span data-ttu-id="050e5-278">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="050e5-278">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="050e5-279">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="050e5-279">Az.Storage</span></span>
* <span data-ttu-id="050e5-280">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="050e5-280">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="050e5-281">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="050e5-281">New-AzStorageContext</span></span>
* <span data-ttu-id="050e5-282">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="050e5-282">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="050e5-283">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="050e5-283">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="050e5-284">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="050e5-284">Az.Websites</span></span>
* <span data-ttu-id="050e5-285">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="050e5-285">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="050e5-286">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="050e5-286">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="050e5-287">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="050e5-287">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="050e5-288">Geral</span><span class="sxs-lookup"><span data-stu-id="050e5-288">General</span></span>

- <span data-ttu-id="050e5-289">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="050e5-289">General Availability of Az Module</span></span>
- <span data-ttu-id="050e5-290">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="050e5-290">Online help for each module</span></span>
- <span data-ttu-id="050e5-291">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="050e5-291">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="050e5-292">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="050e5-292">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="050e5-293">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="050e5-293">Az.Accounts</span></span>
- <span data-ttu-id="050e5-294">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="050e5-294">Changed from Az.Profile</span></span>
- <span data-ttu-id="050e5-295">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="050e5-295">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="050e5-296">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="050e5-296">Az.ApiManagement</span></span>
- <span data-ttu-id="050e5-297">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="050e5-297">Fixes for #7002</span></span>
- <span data-ttu-id="050e5-298">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="050e5-298">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="050e5-299">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="050e5-299">Az.Batch</span></span>
- <span data-ttu-id="050e5-300">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="050e5-300">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="050e5-301">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="050e5-301">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="050e5-302">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="050e5-302">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="050e5-303">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="050e5-303">Az.Billing</span></span>
- <span data-ttu-id="050e5-304">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="050e5-304">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="050e5-305">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="050e5-305">Az.CognitivServices</span></span>
- <span data-ttu-id="050e5-306">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="050e5-306">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="050e5-307">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="050e5-307">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="050e5-308">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="050e5-308">Az.ContainerInstance</span></span>
- <span data-ttu-id="050e5-309">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="050e5-309">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="050e5-310">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="050e5-310">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="050e5-311">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="050e5-311">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="050e5-312">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="050e5-312">Az.DataLakeStore</span></span>
- <span data-ttu-id="050e5-313">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="050e5-313">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="050e5-314">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="050e5-314">Az.Monitor</span></span>
- <span data-ttu-id="050e5-315">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="050e5-315">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="050e5-316">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="050e5-316">Az.KeyVault</span></span>
- <span data-ttu-id="050e5-317">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="050e5-317">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="050e5-318">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="050e5-318">Az.MachineLearning</span></span>
- <span data-ttu-id="050e5-319">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="050e5-319">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="050e5-320">Az.Media</span><span class="sxs-lookup"><span data-stu-id="050e5-320">Az.Media</span></span>
- <span data-ttu-id="050e5-321">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="050e5-321">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="050e5-322">Az.Network</span><span class="sxs-lookup"><span data-stu-id="050e5-322">Az.Network</span></span>
<span data-ttu-id="050e5-323">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="050e5-323">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="050e5-324">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="050e5-324">New cmdlets added:</span></span>
        - <span data-ttu-id="050e5-325">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="050e5-325">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="050e5-326">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="050e5-326">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="050e5-327">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="050e5-327">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="050e5-328">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="050e5-328">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="050e5-329">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="050e5-329">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="050e5-330">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="050e5-330">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="050e5-331">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="050e5-331">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="050e5-332">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="050e5-332">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="050e5-333">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="050e5-333">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="050e5-334">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="050e5-334">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="050e5-335">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="050e5-335">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="050e5-336">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="050e5-336">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="050e5-337">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="050e5-337">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="050e5-338">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="050e5-338">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="050e5-339">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="050e5-339">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="050e5-340">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="050e5-340">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="050e5-341">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="050e5-341">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="050e5-342">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="050e5-342">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="050e5-343">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="050e5-343">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="050e5-344">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="050e5-344">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="050e5-345">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="050e5-345">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="050e5-346">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="050e5-346">Az.OperationalInsights</span></span>
- <span data-ttu-id="050e5-347">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="050e5-347">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="050e5-348">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="050e5-348">Az.Profile</span></span>
- <span data-ttu-id="050e5-349">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="050e5-349">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="050e5-350">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="050e5-350">Az.RecoveryServices</span></span>
- <span data-ttu-id="050e5-351">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="050e5-351">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="050e5-352">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="050e5-352">Az.Resources</span></span>
- <span data-ttu-id="050e5-353">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="050e5-353">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="050e5-354">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="050e5-354">Az.ServiceFabric</span></span>
- <span data-ttu-id="050e5-355">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="050e5-355">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="050e5-356">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="050e5-356">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="050e5-357">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="050e5-357">Az.SIgnalR</span></span>
- <span data-ttu-id="050e5-358">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="050e5-358">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="050e5-359">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="050e5-359">Az.Sql</span></span>
- <span data-ttu-id="050e5-360">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="050e5-360">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="050e5-361">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="050e5-361">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="050e5-362">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="050e5-362">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="050e5-363">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="050e5-363">Az.Storage</span></span>
- <span data-ttu-id="050e5-364">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="050e5-364">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="050e5-365">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="050e5-365">Az.Websites</span></span>
- <span data-ttu-id="050e5-366">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="050e5-366">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="050e5-367">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="050e5-367">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="050e5-368">Geral</span><span class="sxs-lookup"><span data-stu-id="050e5-368">General</span></span>

* <span data-ttu-id="050e5-369">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="050e5-369">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="050e5-370">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="050e5-370">Az.Compute</span></span>

* <span data-ttu-id="050e5-371">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="050e5-371">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="050e5-372">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="050e5-372">Az.DataLakeStore</span></span>

* <span data-ttu-id="050e5-373">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="050e5-373">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="050e5-374">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="050e5-374">Az.FrontDoor</span></span>

* <span data-ttu-id="050e5-375">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="050e5-375">Fixed some broken links</span></span>
    - <span data-ttu-id="050e5-376">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="050e5-376">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="050e5-377">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="050e5-377">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="050e5-378">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="050e5-378">Az.RecoveryServices</span></span>

* <span data-ttu-id="050e5-379">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="050e5-379">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="050e5-380">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="050e5-380">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="050e5-381">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="050e5-381">Az.Resources</span></span>

* <span data-ttu-id="050e5-382">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="050e5-382">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="050e5-383">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="050e5-383">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="050e5-384">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="050e5-384">Az.Sql</span></span>

* <span data-ttu-id="050e5-385">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="050e5-385">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="050e5-386">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="050e5-386">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="050e5-387">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="050e5-387">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="050e5-388">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="050e5-388">Az.Storage</span></span>

* <span data-ttu-id="050e5-389">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="050e5-389">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="050e5-390">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="050e5-390">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="050e5-391">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="050e5-391">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="050e5-392">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="050e5-392">Support Static Website configuration</span></span>
    - <span data-ttu-id="050e5-393">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="050e5-393">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="050e5-394">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="050e5-394">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="050e5-395">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="050e5-395">Az.Websites</span></span>

* <span data-ttu-id="050e5-396">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="050e5-396">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="050e5-397">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="050e5-397">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="050e5-398">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="050e5-398">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="050e5-399">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="050e5-399">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="050e5-400">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="050e5-400">Az.ApiManagement</span></span>
* <span data-ttu-id="050e5-401">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="050e5-401">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="050e5-402">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="050e5-402">Az.Automation</span></span>
* <span data-ttu-id="050e5-403">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="050e5-403">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="050e5-404">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="050e5-404">Added Update Management cmdlets</span></span>
* <span data-ttu-id="050e5-405">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="050e5-405">Added Source Control cmdlets</span></span>
* <span data-ttu-id="050e5-406">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="050e5-406">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="050e5-407">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="050e5-407">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="050e5-408">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="050e5-408">Az.Compute</span></span>
* <span data-ttu-id="050e5-409">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="050e5-409">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="050e5-410">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="050e5-410">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="050e5-411">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="050e5-411">Az.ContainerInstance</span></span>
* <span data-ttu-id="050e5-412">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="050e5-412">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="050e5-413">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="050e5-413">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="050e5-414">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="050e5-414">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="050e5-415">Az.Network</span><span class="sxs-lookup"><span data-stu-id="050e5-415">Az.Network</span></span>
* <span data-ttu-id="050e5-416">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="050e5-416">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="050e5-417">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="050e5-417">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="050e5-418">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="050e5-418">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="050e5-419">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="050e5-419">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="050e5-420">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="050e5-420">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="050e5-421">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="050e5-421">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="050e5-422">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="050e5-422">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="050e5-423">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="050e5-423">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="050e5-424">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="050e5-424">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="050e5-425">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="050e5-425">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="050e5-426">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="050e5-426">Az.Relay</span></span>
* <span data-ttu-id="050e5-427">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="050e5-427">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="050e5-428">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="050e5-428">Az.Resources</span></span>
* <span data-ttu-id="050e5-429">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="050e5-429">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="050e5-430">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="050e5-430">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="050e5-431">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="050e5-431">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="050e5-432">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="050e5-432">Az.ServiceFabric</span></span>
* <span data-ttu-id="050e5-433">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="050e5-433">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="050e5-434">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="050e5-434">Az.Sql</span></span>
* <span data-ttu-id="050e5-435">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="050e5-435">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="050e5-436">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="050e5-436">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="050e5-437">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="050e5-437">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="050e5-438">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="050e5-438">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="050e5-439">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="050e5-439">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="050e5-440">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="050e5-440">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="050e5-441">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="050e5-441">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="050e5-442">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="050e5-442">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="050e5-443">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="050e5-443">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="050e5-444">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="050e5-444">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="050e5-445">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="050e5-445">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="050e5-446">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="050e5-446">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="050e5-447">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="050e5-447">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="050e5-448">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="050e5-448">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="050e5-449">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="050e5-449">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="050e5-450">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="050e5-450">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="050e5-451">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="050e5-451">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="050e5-452">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="050e5-452">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="050e5-453">Geral</span><span class="sxs-lookup"><span data-stu-id="050e5-453">General</span></span>
* <span data-ttu-id="050e5-454">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="050e5-454">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="050e5-455">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="050e5-455">Az.Profile</span></span>
* <span data-ttu-id="050e5-456">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="050e5-456">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="050e5-457">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="050e5-457">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="050e5-458">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="050e5-458">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="050e5-459">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="050e5-459">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="050e5-460">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="050e5-460">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="050e5-461">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="050e5-461">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="050e5-462">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="050e5-462">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="050e5-463">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="050e5-463">Az.CognitiveServices</span></span>
* <span data-ttu-id="050e5-464">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="050e5-464">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="050e5-465">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="050e5-465">Az.Compute</span></span>
* <span data-ttu-id="050e5-466">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="050e5-466">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="050e5-467">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="050e5-467">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="050e5-468">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="050e5-468">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="050e5-469">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="050e5-469">Az.DataLakeStore</span></span>
* <span data-ttu-id="050e5-470">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="050e5-470">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="050e5-471">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="050e5-471">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="050e5-472">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="050e5-472">Az.Insights</span></span>
* <span data-ttu-id="050e5-473">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="050e5-473">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="050e5-474">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="050e5-474">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="050e5-475">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="050e5-475">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="050e5-476">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="050e5-476">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="050e5-477">Az.Network</span><span class="sxs-lookup"><span data-stu-id="050e5-477">Az.Network</span></span>
* <span data-ttu-id="050e5-478">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="050e5-478">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="050e5-479">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="050e5-479">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="050e5-480">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="050e5-480">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="050e5-481">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="050e5-481">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="050e5-482">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="050e5-482">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="050e5-483">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="050e5-483">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="050e5-484">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="050e5-484">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="050e5-485">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="050e5-485">Az.PolicyInsights</span></span>
* <span data-ttu-id="050e5-486">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="050e5-486">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="050e5-487">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="050e5-487">Az.Resources</span></span>
* <span data-ttu-id="050e5-488">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="050e5-488">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="050e5-489">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="050e5-489">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="050e5-490">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="050e5-490">Az.ServiceBus</span></span>
* <span data-ttu-id="050e5-491">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="050e5-491">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="050e5-492">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="050e5-492">Az.ServiceFabric</span></span>
* <span data-ttu-id="050e5-493">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="050e5-493">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="050e5-494">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="050e5-494">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="050e5-495">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="050e5-495">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="050e5-496">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="050e5-496">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="050e5-497">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="050e5-497">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="050e5-498">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="050e5-498">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="050e5-499">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="050e5-499">Az.Profile</span></span>
* <span data-ttu-id="050e5-500">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="050e5-500">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="050e5-501">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="050e5-501">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="050e5-502">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="050e5-502">Az.Compute</span></span>
* <span data-ttu-id="050e5-503">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="050e5-503">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="050e5-504">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="050e5-504">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="050e5-505">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="050e5-505">Az.DataLakeStore</span></span>
* <span data-ttu-id="050e5-506">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="050e5-506">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="050e5-507">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="050e5-507">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="050e5-508">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="050e5-508">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="050e5-509">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="050e5-509">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="050e5-510">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="050e5-510">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="050e5-511">Az.Network</span><span class="sxs-lookup"><span data-stu-id="050e5-511">Az.Network</span></span>
* <span data-ttu-id="050e5-512">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="050e5-512">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="050e5-513">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="050e5-513">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="050e5-514">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="050e5-514">Az.Resources</span></span>
* <span data-ttu-id="050e5-515">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="050e5-515">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="050e5-516">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="050e5-516">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="050e5-517">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="050e5-517">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="050e5-518">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="050e5-518">Azure.Storage</span></span>
* <span data-ttu-id="050e5-519">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="050e5-519">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="050e5-520">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="050e5-520">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="050e5-521">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="050e5-521">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="050e5-522">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="050e5-522">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="050e5-523">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="050e5-523">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="050e5-524">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="050e5-524">Az.CognitiveServices</span></span>
* <span data-ttu-id="050e5-525">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="050e5-525">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="050e5-526">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="050e5-526">Az.Compute</span></span>
* <span data-ttu-id="050e5-527">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="050e5-527">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="050e5-528">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="050e5-528">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="050e5-529">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="050e5-529">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="050e5-530">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="050e5-530">Az.DataFactoryV2</span></span>
* <span data-ttu-id="050e5-531">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="050e5-531">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="050e5-532">Az.Network</span><span class="sxs-lookup"><span data-stu-id="050e5-532">Az.Network</span></span>
* <span data-ttu-id="050e5-533">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="050e5-533">Added NetworkProfile functionality.</span></span> <span data-ttu-id="050e5-534">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="050e5-534">new cmdlets added</span></span>
    - <span data-ttu-id="050e5-535">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="050e5-535">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="050e5-536">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="050e5-536">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="050e5-537">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="050e5-537">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="050e5-538">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="050e5-538">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="050e5-539">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="050e5-539">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="050e5-540">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="050e5-540">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="050e5-541">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="050e5-541">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="050e5-542">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="050e5-542">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="050e5-543">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="050e5-543">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="050e5-544">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="050e5-544">Az.RedisCache</span></span>
* <span data-ttu-id="050e5-545">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="050e5-545">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="050e5-546">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="050e5-546">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="050e5-547">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="050e5-547">Az.Resources</span></span>
* <span data-ttu-id="050e5-548">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="050e5-548">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="050e5-549">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="050e5-549">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="050e5-550">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="050e5-550">Az.Sql</span></span>
* <span data-ttu-id="050e5-551">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="050e5-551">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="050e5-552">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="050e5-552">Az.Websites</span></span>
* <span data-ttu-id="050e5-553">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="050e5-553">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="050e5-554">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="050e5-554">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="050e5-555">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="050e5-555">0.2.0 - September 2018</span></span>
 <span data-ttu-id="050e5-556">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="050e5-556">Initial Release</span></span>