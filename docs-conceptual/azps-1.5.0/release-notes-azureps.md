---
ms.openlocfilehash: 9915ff37e59a73c1d226a216213fd9016b55d3d4
ms.sourcegitcommit: 447276d46ffeeb37f0c07a570536665e36c5ddb8
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/14/2019
ms.locfileid: "57882477"
---
## <a name="150---march-2019"></a><span data-ttu-id="543a0-101">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="543a0-101">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="543a0-102">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="543a0-102">Az.Accounts</span></span>
* <span data-ttu-id="543a0-103">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="543a0-103">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="543a0-104">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="543a0-104">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="543a0-105">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="543a0-105">Az.Automation</span></span>
* <span data-ttu-id="543a0-106">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="543a0-106">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="543a0-107">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="543a0-107">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="543a0-108">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="543a0-108">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="543a0-109">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="543a0-109">Az.Cdn</span></span>
* <span data-ttu-id="543a0-110">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="543a0-110">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="543a0-111">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="543a0-111">Az.Compute</span></span>
* <span data-ttu-id="543a0-112">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="543a0-112">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="543a0-113">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="543a0-113">Az.DataFactory</span></span>
* <span data-ttu-id="543a0-114">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="543a0-114">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="543a0-115">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="543a0-115">Az.LogicApp</span></span>
* <span data-ttu-id="543a0-116">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="543a0-116">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="543a0-117">Az.Network</span><span class="sxs-lookup"><span data-stu-id="543a0-117">Az.Network</span></span>
* <span data-ttu-id="543a0-118">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="543a0-118">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="543a0-119">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="543a0-119">Az.RecoveryServices</span></span>
* <span data-ttu-id="543a0-120">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="543a0-120">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="543a0-121">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="543a0-121">SDK Update</span></span>
* <span data-ttu-id="543a0-122">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="543a0-122">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="543a0-123">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="543a0-123">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="543a0-124">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="543a0-124">Az.Resources</span></span>
* <span data-ttu-id="543a0-125">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="543a0-125">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="543a0-126">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="543a0-126">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="543a0-127">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="543a0-127">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="543a0-128">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="543a0-128">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="543a0-129">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="543a0-129">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="543a0-130">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="543a0-130">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="543a0-131">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="543a0-131">Az.Sql</span></span>
* <span data-ttu-id="543a0-132">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="543a0-132">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="543a0-133">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="543a0-133">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="543a0-134">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="543a0-134">Az.Storage</span></span>
* <span data-ttu-id="543a0-135">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="543a0-135">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="543a0-136">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="543a0-136">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="543a0-137">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="543a0-137">Az.AnalysisServices</span></span>
* <span data-ttu-id="543a0-138">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="543a0-138">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="543a0-139">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="543a0-139">Az.Automation</span></span>
* <span data-ttu-id="543a0-140">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="543a0-140">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="543a0-141">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="543a0-141">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="543a0-142">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="543a0-142">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="543a0-143">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="543a0-143">Az.CognitiveServices</span></span>
* <span data-ttu-id="543a0-144">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="543a0-144">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="543a0-145">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="543a0-145">Az.Compute</span></span>
* <span data-ttu-id="543a0-146">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="543a0-146">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="543a0-147">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="543a0-147">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="543a0-148">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="543a0-148">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="543a0-149">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="543a0-149">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="543a0-150">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="543a0-150">Az.DataLakeStore</span></span>
* <span data-ttu-id="543a0-151">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="543a0-151">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="543a0-152">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="543a0-152">Az.EventHub</span></span>
* <span data-ttu-id="543a0-153">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="543a0-153">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="543a0-154">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="543a0-154">Az.KeyVault</span></span>
* <span data-ttu-id="543a0-155">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="543a0-155">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="543a0-156">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="543a0-156">Az.LogicApp</span></span>
* <span data-ttu-id="543a0-157">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="543a0-157">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="543a0-158">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="543a0-158">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="543a0-159">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="543a0-159">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="543a0-160">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="543a0-160">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="543a0-161">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="543a0-161">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="543a0-162">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="543a0-162">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="543a0-163">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="543a0-163">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="543a0-164">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="543a0-164">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="543a0-165">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="543a0-165">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="543a0-166">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="543a0-166">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="543a0-167">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="543a0-167">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="543a0-168">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="543a0-168">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="543a0-169">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="543a0-169">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="543a0-170">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="543a0-170">Az.Monitor</span></span>
* <span data-ttu-id="543a0-171">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="543a0-171">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="543a0-172">Az.Network</span><span class="sxs-lookup"><span data-stu-id="543a0-172">Az.Network</span></span>
* <span data-ttu-id="543a0-173">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="543a0-173">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="543a0-174">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="543a0-174">Az.OperationalInsights</span></span>
* <span data-ttu-id="543a0-175">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="543a0-175">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="543a0-176">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="543a0-176">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="543a0-177">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="543a0-177">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="543a0-178">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="543a0-178">Az.Resources</span></span>
* <span data-ttu-id="543a0-179">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="543a0-179">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="543a0-180">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="543a0-180">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="543a0-181">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="543a0-181">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="543a0-182">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="543a0-182">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="543a0-183">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="543a0-183">Az.Sql</span></span>
* <span data-ttu-id="543a0-184">Suporte adicionado para a camada Hiperescala da BD SQL</span><span class="sxs-lookup"><span data-stu-id="543a0-184">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="543a0-185">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="543a0-185">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="543a0-186">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="543a0-186">Az.Websites</span></span>
* <span data-ttu-id="543a0-187">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="543a0-187">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="543a0-188">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="543a0-188">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="543a0-189">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="543a0-189">Az.Accounts</span></span>
* <span data-ttu-id="543a0-190">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="543a0-190">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="543a0-191">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="543a0-191">Az.AnalysisServices</span></span>
<span data-ttu-id="543a0-192">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="543a0-192">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="543a0-193">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="543a0-193">Az.Compute</span></span>
* <span data-ttu-id="543a0-194">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="543a0-194">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="543a0-195">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="543a0-195">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="543a0-196">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="543a0-196">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="543a0-197">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="543a0-197">Az.RecoveryServices</span></span>
<span data-ttu-id="543a0-198">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="543a0-198">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="543a0-199">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="543a0-199">Az.Resources</span></span>
* <span data-ttu-id="543a0-200">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="543a0-200">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="543a0-201">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="543a0-201">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="543a0-202">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="543a0-202">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="543a0-203">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="543a0-203">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="543a0-204">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="543a0-204">Az.Sql</span></span>
* <span data-ttu-id="543a0-205">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="543a0-205">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="543a0-206">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="543a0-206">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="543a0-207">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="543a0-207">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="543a0-208">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="543a0-208">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="543a0-209">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="543a0-209">Az.Accounts</span></span>
* <span data-ttu-id="543a0-210">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="543a0-210">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="543a0-211">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="543a0-211">Az.AnalysisServices</span></span>
* <span data-ttu-id="543a0-212">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="543a0-212">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="543a0-213">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="543a0-213">Az.RecoveryServices</span></span>
* <span data-ttu-id="543a0-214">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="543a0-214">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="543a0-215">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="543a0-215">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="543a0-216">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="543a0-216">Az.Accounts</span></span>
* <span data-ttu-id="543a0-217">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="543a0-217">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="543a0-218">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="543a0-218">Update incorrect online help URLs</span></span>
* <span data-ttu-id="543a0-219">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="543a0-219">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="543a0-220">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="543a0-220">Az.Aks</span></span>
* <span data-ttu-id="543a0-221">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="543a0-221">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="543a0-222">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="543a0-222">Az.Automation</span></span>
* <span data-ttu-id="543a0-223">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="543a0-223">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="543a0-224">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="543a0-224">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="543a0-225">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="543a0-225">Az.Cdn</span></span>
* <span data-ttu-id="543a0-226">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="543a0-226">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="543a0-227">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="543a0-227">Az.Compute</span></span>
* <span data-ttu-id="543a0-228">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="543a0-228">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="543a0-229">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="543a0-229">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="543a0-230">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="543a0-230">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="543a0-231">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="543a0-231">Az.ContainerRegistry</span></span>
* <span data-ttu-id="543a0-232">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="543a0-232">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="543a0-233">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="543a0-233">Az.DataFactory</span></span>
* <span data-ttu-id="543a0-234">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="543a0-234">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="543a0-235">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="543a0-235">Az.DataLakeStore</span></span>
* <span data-ttu-id="543a0-236">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="543a0-236">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="543a0-237">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="543a0-237">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="543a0-238">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="543a0-238">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="543a0-239">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="543a0-239">Az.IotHub</span></span>
* <span data-ttu-id="543a0-240">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="543a0-240">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="543a0-241">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="543a0-241">Az.KeyVault</span></span>
* <span data-ttu-id="543a0-242">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="543a0-242">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="543a0-243">Az.Network</span><span class="sxs-lookup"><span data-stu-id="543a0-243">Az.Network</span></span>
* <span data-ttu-id="543a0-244">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="543a0-244">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="543a0-245">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="543a0-245">Az.Resources</span></span>
* <span data-ttu-id="543a0-246">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="543a0-246">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="543a0-247">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="543a0-247">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="543a0-248">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="543a0-248">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="543a0-249">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="543a0-249">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="543a0-250">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="543a0-250">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="543a0-251">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="543a0-251">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="543a0-252">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="543a0-252">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="543a0-253">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="543a0-253">Az.ServiceFabric</span></span>
* <span data-ttu-id="543a0-254">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="543a0-254">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="543a0-255">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="543a0-255">Fix some error messages.</span></span>
* <span data-ttu-id="543a0-256">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="543a0-256">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="543a0-257">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="543a0-257">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="543a0-258">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="543a0-258">Az.SignalR</span></span>
* <span data-ttu-id="543a0-259">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="543a0-259">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="543a0-260">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="543a0-260">Az.Sql</span></span>
* <span data-ttu-id="543a0-261">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="543a0-261">Update incorrect online help URLs</span></span>
* <span data-ttu-id="543a0-262">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="543a0-262">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="543a0-263">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="543a0-263">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="543a0-264">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="543a0-264">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="543a0-265">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="543a0-265">Az.Storage</span></span>
* <span data-ttu-id="543a0-266">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="543a0-266">Update incorrect online help URLs</span></span>
* <span data-ttu-id="543a0-267">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="543a0-267">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="543a0-268">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="543a0-268">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="543a0-269">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="543a0-269">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="543a0-270">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="543a0-270">Az.TrafficManager</span></span>
* <span data-ttu-id="543a0-271">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="543a0-271">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="543a0-272">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="543a0-272">Az.Websites</span></span>
* <span data-ttu-id="543a0-273">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="543a0-273">Update incorrect online help URLs</span></span>
* <span data-ttu-id="543a0-274">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="543a0-274">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="543a0-275">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="543a0-275">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="543a0-276">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="543a0-276">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="543a0-277">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="543a0-277">Az.Accounts</span></span>
* <span data-ttu-id="543a0-278">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="543a0-278">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="543a0-279">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="543a0-279">Az.Compute</span></span>
* <span data-ttu-id="543a0-280">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="543a0-280">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="543a0-281">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="543a0-281">Updated the description of ID in help files</span></span>
* <span data-ttu-id="543a0-282">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="543a0-282">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="543a0-283">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="543a0-283">Az.DataLakeStore</span></span>
* <span data-ttu-id="543a0-284">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="543a0-284">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="543a0-285">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="543a0-285">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="543a0-286">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="543a0-286">Az.EventGrid</span></span>
* <span data-ttu-id="543a0-287">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="543a0-287">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="543a0-288">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="543a0-288">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="543a0-289">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="543a0-289">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="543a0-290">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="543a0-290">Event Time-To-Live,</span></span>
        - <span data-ttu-id="543a0-291">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="543a0-291">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="543a0-292">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="543a0-292">Dead letter endpoint.</span></span>
    - <span data-ttu-id="543a0-293">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="543a0-293">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="543a0-294">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="543a0-294">Event Time-To-Live,</span></span>
        - <span data-ttu-id="543a0-295">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="543a0-295">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="543a0-296">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="543a0-296">Dead letter endpoint.</span></span>
* <span data-ttu-id="543a0-297">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="543a0-297">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="543a0-298">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="543a0-298">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="543a0-299">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="543a0-299">Az.IotHub</span></span>
* <span data-ttu-id="543a0-300">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="543a0-300">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="543a0-301">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="543a0-301">Az.LogicApp</span></span>
* <span data-ttu-id="543a0-302">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="543a0-302">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="543a0-303">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="543a0-303">Az.Resources</span></span>
* <span data-ttu-id="543a0-304">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="543a0-304">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="543a0-305">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="543a0-305">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="543a0-306">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="543a0-306">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="543a0-307">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="543a0-307">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="543a0-308">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="543a0-308">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="543a0-309">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="543a0-309">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="543a0-310">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="543a0-310">Az.SignalR</span></span>
* <span data-ttu-id="543a0-311">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="543a0-311">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="543a0-312">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="543a0-312">Az.Sql</span></span>
* <span data-ttu-id="543a0-313">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="543a0-313">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="543a0-314">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="543a0-314">Az.Storage</span></span>
* <span data-ttu-id="543a0-315">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="543a0-315">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="543a0-316">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="543a0-316">New-AzStorageContext</span></span>
* <span data-ttu-id="543a0-317">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="543a0-317">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="543a0-318">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="543a0-318">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="543a0-319">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="543a0-319">Az.Websites</span></span>
* <span data-ttu-id="543a0-320">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="543a0-320">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="543a0-321">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="543a0-321">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="543a0-322">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="543a0-322">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="543a0-323">Geral</span><span class="sxs-lookup"><span data-stu-id="543a0-323">General</span></span>

- <span data-ttu-id="543a0-324">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="543a0-324">General Availability of Az Module</span></span>
- <span data-ttu-id="543a0-325">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="543a0-325">Online help for each module</span></span>
- <span data-ttu-id="543a0-326">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="543a0-326">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="543a0-327">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="543a0-327">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="543a0-328">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="543a0-328">Az.Accounts</span></span>
- <span data-ttu-id="543a0-329">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="543a0-329">Changed from Az.Profile</span></span>
- <span data-ttu-id="543a0-330">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="543a0-330">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="543a0-331">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="543a0-331">Az.ApiManagement</span></span>
- <span data-ttu-id="543a0-332">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="543a0-332">Fixes for #7002</span></span>
- <span data-ttu-id="543a0-333">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="543a0-333">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="543a0-334">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="543a0-334">Az.Batch</span></span>
- <span data-ttu-id="543a0-335">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="543a0-335">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="543a0-336">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="543a0-336">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="543a0-337">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="543a0-337">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="543a0-338">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="543a0-338">Az.Billing</span></span>
- <span data-ttu-id="543a0-339">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="543a0-339">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="543a0-340">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="543a0-340">Az.CognitivServices</span></span>
- <span data-ttu-id="543a0-341">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="543a0-341">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="543a0-342">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="543a0-342">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="543a0-343">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="543a0-343">Az.ContainerInstance</span></span>
- <span data-ttu-id="543a0-344">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="543a0-344">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="543a0-345">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="543a0-345">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="543a0-346">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="543a0-346">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="543a0-347">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="543a0-347">Az.DataLakeStore</span></span>
- <span data-ttu-id="543a0-348">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="543a0-348">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="543a0-349">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="543a0-349">Az.Monitor</span></span>
- <span data-ttu-id="543a0-350">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="543a0-350">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="543a0-351">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="543a0-351">Az.KeyVault</span></span>
- <span data-ttu-id="543a0-352">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="543a0-352">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="543a0-353">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="543a0-353">Az.MachineLearning</span></span>
- <span data-ttu-id="543a0-354">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="543a0-354">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="543a0-355">Az.Media</span><span class="sxs-lookup"><span data-stu-id="543a0-355">Az.Media</span></span>
- <span data-ttu-id="543a0-356">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="543a0-356">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="543a0-357">Az.Network</span><span class="sxs-lookup"><span data-stu-id="543a0-357">Az.Network</span></span>
<span data-ttu-id="543a0-358">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="543a0-358">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="543a0-359">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="543a0-359">New cmdlets added:</span></span>
        - <span data-ttu-id="543a0-360">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="543a0-360">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="543a0-361">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="543a0-361">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="543a0-362">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="543a0-362">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="543a0-363">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="543a0-363">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="543a0-364">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="543a0-364">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="543a0-365">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="543a0-365">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="543a0-366">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="543a0-366">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="543a0-367">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="543a0-367">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="543a0-368">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="543a0-368">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="543a0-369">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="543a0-369">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="543a0-370">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="543a0-370">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="543a0-371">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="543a0-371">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="543a0-372">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="543a0-372">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="543a0-373">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="543a0-373">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="543a0-374">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="543a0-374">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="543a0-375">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="543a0-375">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="543a0-376">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="543a0-376">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="543a0-377">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="543a0-377">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="543a0-378">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="543a0-378">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="543a0-379">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="543a0-379">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="543a0-380">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="543a0-380">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="543a0-381">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="543a0-381">Az.OperationalInsights</span></span>
- <span data-ttu-id="543a0-382">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="543a0-382">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="543a0-383">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="543a0-383">Az.Profile</span></span>
- <span data-ttu-id="543a0-384">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="543a0-384">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="543a0-385">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="543a0-385">Az.RecoveryServices</span></span>
- <span data-ttu-id="543a0-386">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="543a0-386">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="543a0-387">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="543a0-387">Az.Resources</span></span>
- <span data-ttu-id="543a0-388">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="543a0-388">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="543a0-389">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="543a0-389">Az.ServiceFabric</span></span>
- <span data-ttu-id="543a0-390">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="543a0-390">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="543a0-391">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="543a0-391">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="543a0-392">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="543a0-392">Az.SIgnalR</span></span>
- <span data-ttu-id="543a0-393">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="543a0-393">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="543a0-394">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="543a0-394">Az.Sql</span></span>
- <span data-ttu-id="543a0-395">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="543a0-395">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="543a0-396">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="543a0-396">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="543a0-397">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="543a0-397">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="543a0-398">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="543a0-398">Az.Storage</span></span>
- <span data-ttu-id="543a0-399">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="543a0-399">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="543a0-400">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="543a0-400">Az.Websites</span></span>
- <span data-ttu-id="543a0-401">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="543a0-401">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="543a0-402">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="543a0-402">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="543a0-403">Geral</span><span class="sxs-lookup"><span data-stu-id="543a0-403">General</span></span>

* <span data-ttu-id="543a0-404">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="543a0-404">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="543a0-405">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="543a0-405">Az.Compute</span></span>

* <span data-ttu-id="543a0-406">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="543a0-406">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="543a0-407">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="543a0-407">Az.DataLakeStore</span></span>

* <span data-ttu-id="543a0-408">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="543a0-408">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="543a0-409">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="543a0-409">Az.FrontDoor</span></span>

* <span data-ttu-id="543a0-410">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="543a0-410">Fixed some broken links</span></span>
    - <span data-ttu-id="543a0-411">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="543a0-411">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="543a0-412">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="543a0-412">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="543a0-413">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="543a0-413">Az.RecoveryServices</span></span>

* <span data-ttu-id="543a0-414">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="543a0-414">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="543a0-415">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="543a0-415">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="543a0-416">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="543a0-416">Az.Resources</span></span>

* <span data-ttu-id="543a0-417">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="543a0-417">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="543a0-418">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="543a0-418">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="543a0-419">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="543a0-419">Az.Sql</span></span>

* <span data-ttu-id="543a0-420">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="543a0-420">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="543a0-421">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="543a0-421">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="543a0-422">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="543a0-422">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="543a0-423">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="543a0-423">Az.Storage</span></span>

* <span data-ttu-id="543a0-424">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="543a0-424">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="543a0-425">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="543a0-425">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="543a0-426">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="543a0-426">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="543a0-427">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="543a0-427">Support Static Website configuration</span></span>
    - <span data-ttu-id="543a0-428">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="543a0-428">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="543a0-429">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="543a0-429">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="543a0-430">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="543a0-430">Az.Websites</span></span>

* <span data-ttu-id="543a0-431">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="543a0-431">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="543a0-432">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="543a0-432">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="543a0-433">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="543a0-433">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="543a0-434">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="543a0-434">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="543a0-435">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="543a0-435">Az.ApiManagement</span></span>
* <span data-ttu-id="543a0-436">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="543a0-436">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="543a0-437">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="543a0-437">Az.Automation</span></span>
* <span data-ttu-id="543a0-438">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="543a0-438">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="543a0-439">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="543a0-439">Added Update Management cmdlets</span></span>
* <span data-ttu-id="543a0-440">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="543a0-440">Added Source Control cmdlets</span></span>
* <span data-ttu-id="543a0-441">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="543a0-441">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="543a0-442">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="543a0-442">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="543a0-443">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="543a0-443">Az.Compute</span></span>
* <span data-ttu-id="543a0-444">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="543a0-444">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="543a0-445">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="543a0-445">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="543a0-446">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="543a0-446">Az.ContainerInstance</span></span>
* <span data-ttu-id="543a0-447">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="543a0-447">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="543a0-448">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="543a0-448">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="543a0-449">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="543a0-449">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="543a0-450">Az.Network</span><span class="sxs-lookup"><span data-stu-id="543a0-450">Az.Network</span></span>
* <span data-ttu-id="543a0-451">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="543a0-451">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="543a0-452">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="543a0-452">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="543a0-453">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="543a0-453">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="543a0-454">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="543a0-454">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="543a0-455">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="543a0-455">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="543a0-456">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="543a0-456">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="543a0-457">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="543a0-457">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="543a0-458">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="543a0-458">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="543a0-459">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="543a0-459">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="543a0-460">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="543a0-460">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="543a0-461">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="543a0-461">Az.Relay</span></span>
* <span data-ttu-id="543a0-462">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="543a0-462">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="543a0-463">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="543a0-463">Az.Resources</span></span>
* <span data-ttu-id="543a0-464">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="543a0-464">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="543a0-465">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="543a0-465">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="543a0-466">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="543a0-466">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="543a0-467">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="543a0-467">Az.ServiceFabric</span></span>
* <span data-ttu-id="543a0-468">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="543a0-468">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="543a0-469">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="543a0-469">Az.Sql</span></span>
* <span data-ttu-id="543a0-470">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="543a0-470">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="543a0-471">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="543a0-471">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="543a0-472">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="543a0-472">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="543a0-473">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="543a0-473">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="543a0-474">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="543a0-474">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="543a0-475">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="543a0-475">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="543a0-476">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="543a0-476">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="543a0-477">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="543a0-477">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="543a0-478">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="543a0-478">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="543a0-479">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="543a0-479">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="543a0-480">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="543a0-480">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="543a0-481">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="543a0-481">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="543a0-482">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="543a0-482">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="543a0-483">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="543a0-483">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="543a0-484">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="543a0-484">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="543a0-485">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="543a0-485">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="543a0-486">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="543a0-486">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="543a0-487">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="543a0-487">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="543a0-488">Geral</span><span class="sxs-lookup"><span data-stu-id="543a0-488">General</span></span>
* <span data-ttu-id="543a0-489">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="543a0-489">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="543a0-490">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="543a0-490">Az.Profile</span></span>
* <span data-ttu-id="543a0-491">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="543a0-491">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="543a0-492">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="543a0-492">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="543a0-493">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="543a0-493">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="543a0-494">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="543a0-494">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="543a0-495">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="543a0-495">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="543a0-496">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="543a0-496">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="543a0-497">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="543a0-497">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="543a0-498">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="543a0-498">Az.CognitiveServices</span></span>
* <span data-ttu-id="543a0-499">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="543a0-499">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="543a0-500">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="543a0-500">Az.Compute</span></span>
* <span data-ttu-id="543a0-501">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="543a0-501">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="543a0-502">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="543a0-502">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="543a0-503">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="543a0-503">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="543a0-504">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="543a0-504">Az.DataLakeStore</span></span>
* <span data-ttu-id="543a0-505">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="543a0-505">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="543a0-506">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="543a0-506">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="543a0-507">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="543a0-507">Az.Insights</span></span>
* <span data-ttu-id="543a0-508">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="543a0-508">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="543a0-509">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="543a0-509">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="543a0-510">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="543a0-510">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="543a0-511">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="543a0-511">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="543a0-512">Az.Network</span><span class="sxs-lookup"><span data-stu-id="543a0-512">Az.Network</span></span>
* <span data-ttu-id="543a0-513">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="543a0-513">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="543a0-514">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="543a0-514">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="543a0-515">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="543a0-515">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="543a0-516">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="543a0-516">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="543a0-517">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="543a0-517">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="543a0-518">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="543a0-518">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="543a0-519">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="543a0-519">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="543a0-520">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="543a0-520">Az.PolicyInsights</span></span>
* <span data-ttu-id="543a0-521">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="543a0-521">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="543a0-522">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="543a0-522">Az.Resources</span></span>
* <span data-ttu-id="543a0-523">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="543a0-523">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="543a0-524">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="543a0-524">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="543a0-525">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="543a0-525">Az.ServiceBus</span></span>
* <span data-ttu-id="543a0-526">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="543a0-526">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="543a0-527">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="543a0-527">Az.ServiceFabric</span></span>
* <span data-ttu-id="543a0-528">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="543a0-528">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="543a0-529">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="543a0-529">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="543a0-530">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="543a0-530">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="543a0-531">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="543a0-531">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="543a0-532">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="543a0-532">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="543a0-533">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="543a0-533">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="543a0-534">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="543a0-534">Az.Profile</span></span>
* <span data-ttu-id="543a0-535">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="543a0-535">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="543a0-536">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="543a0-536">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="543a0-537">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="543a0-537">Az.Compute</span></span>
* <span data-ttu-id="543a0-538">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="543a0-538">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="543a0-539">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="543a0-539">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="543a0-540">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="543a0-540">Az.DataLakeStore</span></span>
* <span data-ttu-id="543a0-541">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="543a0-541">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="543a0-542">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="543a0-542">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="543a0-543">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="543a0-543">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="543a0-544">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="543a0-544">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="543a0-545">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="543a0-545">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="543a0-546">Az.Network</span><span class="sxs-lookup"><span data-stu-id="543a0-546">Az.Network</span></span>
* <span data-ttu-id="543a0-547">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="543a0-547">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="543a0-548">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="543a0-548">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="543a0-549">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="543a0-549">Az.Resources</span></span>
* <span data-ttu-id="543a0-550">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="543a0-550">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="543a0-551">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="543a0-551">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="543a0-552">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="543a0-552">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="543a0-553">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="543a0-553">Azure.Storage</span></span>
* <span data-ttu-id="543a0-554">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="543a0-554">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="543a0-555">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="543a0-555">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="543a0-556">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="543a0-556">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="543a0-557">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="543a0-557">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="543a0-558">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="543a0-558">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="543a0-559">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="543a0-559">Az.CognitiveServices</span></span>
* <span data-ttu-id="543a0-560">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="543a0-560">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="543a0-561">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="543a0-561">Az.Compute</span></span>
* <span data-ttu-id="543a0-562">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="543a0-562">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="543a0-563">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="543a0-563">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="543a0-564">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="543a0-564">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="543a0-565">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="543a0-565">Az.DataFactoryV2</span></span>
* <span data-ttu-id="543a0-566">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="543a0-566">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="543a0-567">Az.Network</span><span class="sxs-lookup"><span data-stu-id="543a0-567">Az.Network</span></span>
* <span data-ttu-id="543a0-568">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="543a0-568">Added NetworkProfile functionality.</span></span> <span data-ttu-id="543a0-569">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="543a0-569">new cmdlets added</span></span>
    - <span data-ttu-id="543a0-570">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="543a0-570">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="543a0-571">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="543a0-571">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="543a0-572">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="543a0-572">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="543a0-573">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="543a0-573">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="543a0-574">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="543a0-574">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="543a0-575">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="543a0-575">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="543a0-576">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="543a0-576">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="543a0-577">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="543a0-577">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="543a0-578">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="543a0-578">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="543a0-579">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="543a0-579">Az.RedisCache</span></span>
* <span data-ttu-id="543a0-580">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="543a0-580">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="543a0-581">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="543a0-581">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="543a0-582">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="543a0-582">Az.Resources</span></span>
* <span data-ttu-id="543a0-583">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="543a0-583">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="543a0-584">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="543a0-584">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="543a0-585">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="543a0-585">Az.Sql</span></span>
* <span data-ttu-id="543a0-586">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="543a0-586">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="543a0-587">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="543a0-587">Az.Websites</span></span>
* <span data-ttu-id="543a0-588">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="543a0-588">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="543a0-589">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="543a0-589">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="543a0-590">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="543a0-590">0.2.0 - September 2018</span></span>
 <span data-ttu-id="543a0-591">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="543a0-591">Initial Release</span></span>