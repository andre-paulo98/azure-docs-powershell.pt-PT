---
ms.openlocfilehash: 179d22fa065944695e4769f2698e3cabc7666b04
ms.sourcegitcommit: c6fd0e490fa0e33b8b768b679682a47d8faae1cf
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/16/2019
ms.locfileid: "54342152"
---
## <a name="110---january-2019"></a><span data-ttu-id="44773-101">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="44773-101">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="44773-102">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="44773-102">Az.Accounts</span></span>
* <span data-ttu-id="44773-103">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="44773-103">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="44773-104">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="44773-104">Az.Compute</span></span>
* <span data-ttu-id="44773-105">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="44773-105">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="44773-106">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="44773-106">Updated the description of ID in help files</span></span>
* <span data-ttu-id="44773-107">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="44773-107">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="44773-108">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="44773-108">Az.DataLakeStore</span></span>
* <span data-ttu-id="44773-109">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="44773-109">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="44773-110">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="44773-110">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="44773-111">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="44773-111">Az.EventGrid</span></span>
* <span data-ttu-id="44773-112">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="44773-112">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="44773-113">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="44773-113">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="44773-114">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="44773-114">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="44773-115">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="44773-115">Event Time-To-Live,</span></span>
        - <span data-ttu-id="44773-116">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="44773-116">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="44773-117">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="44773-117">Dead letter endpoint.</span></span>
    - <span data-ttu-id="44773-118">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="44773-118">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="44773-119">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="44773-119">Event Time-To-Live,</span></span>
        - <span data-ttu-id="44773-120">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="44773-120">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="44773-121">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="44773-121">Dead letter endpoint.</span></span>
* <span data-ttu-id="44773-122">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="44773-122">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="44773-123">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="44773-123">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="44773-124">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="44773-124">Az.IotHub</span></span>
* <span data-ttu-id="44773-125">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="44773-125">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="44773-126">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="44773-126">Az.LogicApp</span></span>
* <span data-ttu-id="44773-127">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="44773-127">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="44773-128">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44773-128">Az.Resources</span></span>
* <span data-ttu-id="44773-129">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="44773-129">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="44773-130">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="44773-130">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="44773-131">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="44773-131">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="44773-132">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="44773-132">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="44773-133">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="44773-133">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="44773-134">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="44773-134">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="44773-135">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="44773-135">Az.SignalR</span></span>
* <span data-ttu-id="44773-136">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="44773-136">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="44773-137">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="44773-137">Az.Sql</span></span>
* <span data-ttu-id="44773-138">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="44773-138">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="44773-139">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="44773-139">Az.Storage</span></span>
* <span data-ttu-id="44773-140">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="44773-140">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="44773-141">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="44773-141">New-AzStorageContext</span></span>
* <span data-ttu-id="44773-142">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="44773-142">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="44773-143">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="44773-143">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="44773-144">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="44773-144">Az.Websites</span></span>
* <span data-ttu-id="44773-145">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="44773-145">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="44773-146">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="44773-146">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="44773-147">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="44773-147">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="44773-148">Geral</span><span class="sxs-lookup"><span data-stu-id="44773-148">General</span></span>

- <span data-ttu-id="44773-149">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="44773-149">General Availability of Az Module</span></span>
- <span data-ttu-id="44773-150">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="44773-150">Online help for each module</span></span>
- <span data-ttu-id="44773-151">Para obter mais detalhes e um mapa, consulte a [página de Anúncio do módulo Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="44773-151">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="44773-152">Consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="44773-152">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="44773-153">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="44773-153">Az.Accounts</span></span>
- <span data-ttu-id="44773-154">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="44773-154">Changed from Az.Profile</span></span>
- <span data-ttu-id="44773-155">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="44773-155">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="44773-156">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="44773-156">Az.ApiManagement</span></span>
- <span data-ttu-id="44773-157">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="44773-157">Fixes for #7002</span></span>
- <span data-ttu-id="44773-158">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44773-158">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="44773-159">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="44773-159">Az.Batch</span></span>
- <span data-ttu-id="44773-160">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="44773-160">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="44773-161">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="44773-161">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="44773-162">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44773-162">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="44773-163">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="44773-163">Az.Billing</span></span>
- <span data-ttu-id="44773-164">Combina os cmdlets Billing, Consumption e UsageAggregates; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44773-164">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="44773-165">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="44773-165">Az.CognitivServices</span></span>
- <span data-ttu-id="44773-166">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="44773-166">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="44773-167">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="44773-167">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="44773-168">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="44773-168">Az.ContainerInstance</span></span>
- <span data-ttu-id="44773-169">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="44773-169">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="44773-170">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="44773-170">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="44773-171">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44773-171">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="44773-172">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="44773-172">Az.DataLakeStore</span></span>
- <span data-ttu-id="44773-173">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44773-173">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="44773-174">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="44773-174">Az.Monitor</span></span>
- <span data-ttu-id="44773-175">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44773-175">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="44773-176">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="44773-176">Az.KeyVault</span></span>
- <span data-ttu-id="44773-177">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="44773-177">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="44773-178">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="44773-178">Az.MachineLearning</span></span>
- <span data-ttu-id="44773-179">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="44773-179">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="44773-180">Az.Media</span><span class="sxs-lookup"><span data-stu-id="44773-180">Az.Media</span></span>
- <span data-ttu-id="44773-181">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="44773-181">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="44773-182">Az.Network</span><span class="sxs-lookup"><span data-stu-id="44773-182">Az.Network</span></span>
<span data-ttu-id="44773-183">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="44773-183">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="44773-184">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="44773-184">New cmdlets added:</span></span>
        - <span data-ttu-id="44773-185">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="44773-185">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="44773-186">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="44773-186">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="44773-187">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="44773-187">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="44773-188">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="44773-188">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="44773-189">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="44773-189">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="44773-190">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="44773-190">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="44773-191">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="44773-191">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="44773-192">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="44773-192">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="44773-193">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="44773-193">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="44773-194">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="44773-194">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="44773-195">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="44773-195">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="44773-196">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="44773-196">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="44773-197">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="44773-197">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="44773-198">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="44773-198">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="44773-199">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="44773-199">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="44773-200">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="44773-200">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="44773-201">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="44773-201">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="44773-202">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="44773-202">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="44773-203">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="44773-203">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="44773-204">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="44773-204">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="44773-205">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44773-205">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="44773-206">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="44773-206">Az.OperationalInsights</span></span>
- <span data-ttu-id="44773-207">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44773-207">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="44773-208">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="44773-208">Az.Profile</span></span>
- <span data-ttu-id="44773-209">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="44773-209">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="44773-210">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="44773-210">Az.RecoveryServices</span></span>
- <span data-ttu-id="44773-211">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44773-211">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="44773-212">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44773-212">Az.Resources</span></span>
- <span data-ttu-id="44773-213">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44773-213">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="44773-214">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="44773-214">Az.ServiceFabric</span></span>
- <span data-ttu-id="44773-215">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="44773-215">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="44773-216">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44773-216">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="44773-217">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="44773-217">Az.SIgnalR</span></span>
- <span data-ttu-id="44773-218">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="44773-218">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="44773-219">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="44773-219">Az.Sql</span></span>
- <span data-ttu-id="44773-220">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="44773-220">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="44773-221">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="44773-221">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="44773-222">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44773-222">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="44773-223">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="44773-223">Az.Storage</span></span>
- <span data-ttu-id="44773-224">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44773-224">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="44773-225">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="44773-225">Az.Websites</span></span>
- <span data-ttu-id="44773-226">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44773-226">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="44773-227">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="44773-227">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="44773-228">Geral</span><span class="sxs-lookup"><span data-stu-id="44773-228">General</span></span>

* <span data-ttu-id="44773-229">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="44773-229">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="44773-230">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="44773-230">Az.Compute</span></span>

* <span data-ttu-id="44773-231">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="44773-231">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="44773-232">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="44773-232">Az.DataLakeStore</span></span>

* <span data-ttu-id="44773-233">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="44773-233">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="44773-234">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="44773-234">Az.FrontDoor</span></span>

* <span data-ttu-id="44773-235">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="44773-235">Fixed some broken links</span></span>
    - <span data-ttu-id="44773-236">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="44773-236">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="44773-237">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="44773-237">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="44773-238">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="44773-238">Az.RecoveryServices</span></span>

* <span data-ttu-id="44773-239">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="44773-239">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="44773-240">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="44773-240">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="44773-241">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44773-241">Az.Resources</span></span>

* <span data-ttu-id="44773-242">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="44773-242">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="44773-243">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="44773-243">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="44773-244">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="44773-244">Az.Sql</span></span>

* <span data-ttu-id="44773-245">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="44773-245">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="44773-246">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="44773-246">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="44773-247">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="44773-247">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="44773-248">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="44773-248">Az.Storage</span></span>

* <span data-ttu-id="44773-249">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="44773-249">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="44773-250">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="44773-250">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="44773-251">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="44773-251">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="44773-252">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="44773-252">Support Static Website configuration</span></span>
    - <span data-ttu-id="44773-253">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="44773-253">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="44773-254">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="44773-254">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="44773-255">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="44773-255">Az.Websites</span></span>

* <span data-ttu-id="44773-256">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="44773-256">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="44773-257">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="44773-257">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="44773-258">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="44773-258">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="44773-259">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="44773-259">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="44773-260">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="44773-260">Az.ApiManagement</span></span>
* <span data-ttu-id="44773-261">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="44773-261">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="44773-262">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="44773-262">Az.Automation</span></span>
* <span data-ttu-id="44773-263">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="44773-263">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="44773-264">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="44773-264">Added Update Management cmdlets</span></span>
* <span data-ttu-id="44773-265">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="44773-265">Added Source Control cmdlets</span></span>
* <span data-ttu-id="44773-266">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="44773-266">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="44773-267">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="44773-267">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="44773-268">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="44773-268">Az.Compute</span></span>
* <span data-ttu-id="44773-269">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="44773-269">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="44773-270">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="44773-270">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="44773-271">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="44773-271">Az.ContainerInstance</span></span>
* <span data-ttu-id="44773-272">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="44773-272">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="44773-273">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="44773-273">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="44773-274">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="44773-274">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="44773-275">Az.Network</span><span class="sxs-lookup"><span data-stu-id="44773-275">Az.Network</span></span>
* <span data-ttu-id="44773-276">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="44773-276">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="44773-277">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="44773-277">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="44773-278">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="44773-278">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="44773-279">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="44773-279">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="44773-280">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="44773-280">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="44773-281">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="44773-281">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="44773-282">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="44773-282">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="44773-283">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="44773-283">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="44773-284">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="44773-284">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="44773-285">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="44773-285">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="44773-286">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="44773-286">Az.Relay</span></span>
* <span data-ttu-id="44773-287">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="44773-287">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="44773-288">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44773-288">Az.Resources</span></span>
* <span data-ttu-id="44773-289">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="44773-289">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="44773-290">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="44773-290">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="44773-291">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="44773-291">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="44773-292">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="44773-292">Az.ServiceFabric</span></span>
* <span data-ttu-id="44773-293">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="44773-293">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="44773-294">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="44773-294">Az.Sql</span></span>
* <span data-ttu-id="44773-295">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="44773-295">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="44773-296">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="44773-296">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="44773-297">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="44773-297">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="44773-298">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="44773-298">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="44773-299">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="44773-299">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="44773-300">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="44773-300">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="44773-301">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="44773-301">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="44773-302">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="44773-302">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="44773-303">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="44773-303">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="44773-304">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="44773-304">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="44773-305">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="44773-305">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="44773-306">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="44773-306">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="44773-307">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="44773-307">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="44773-308">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="44773-308">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="44773-309">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="44773-309">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="44773-310">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="44773-310">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="44773-311">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="44773-311">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="44773-312">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="44773-312">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="44773-313">Geral</span><span class="sxs-lookup"><span data-stu-id="44773-313">General</span></span>
* <span data-ttu-id="44773-314">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="44773-314">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="44773-315">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="44773-315">Az.Profile</span></span>
* <span data-ttu-id="44773-316">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="44773-316">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="44773-317">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="44773-317">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="44773-318">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="44773-318">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="44773-319">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="44773-319">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="44773-320">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="44773-320">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="44773-321">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="44773-321">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="44773-322">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="44773-322">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="44773-323">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="44773-323">Az.CognitiveServices</span></span>
* <span data-ttu-id="44773-324">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="44773-324">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="44773-325">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="44773-325">Az.Compute</span></span>
* <span data-ttu-id="44773-326">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="44773-326">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="44773-327">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="44773-327">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="44773-328">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="44773-328">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="44773-329">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="44773-329">Az.DataLakeStore</span></span>
* <span data-ttu-id="44773-330">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="44773-330">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="44773-331">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="44773-331">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="44773-332">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="44773-332">Az.Insights</span></span>
* <span data-ttu-id="44773-333">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="44773-333">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="44773-334">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="44773-334">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="44773-335">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="44773-335">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="44773-336">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="44773-336">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="44773-337">Az.Network</span><span class="sxs-lookup"><span data-stu-id="44773-337">Az.Network</span></span>
* <span data-ttu-id="44773-338">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="44773-338">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="44773-339">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="44773-339">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="44773-340">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="44773-340">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="44773-341">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="44773-341">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="44773-342">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="44773-342">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="44773-343">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="44773-343">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="44773-344">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="44773-344">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="44773-345">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="44773-345">Az.PolicyInsights</span></span>
* <span data-ttu-id="44773-346">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="44773-346">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="44773-347">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44773-347">Az.Resources</span></span>
* <span data-ttu-id="44773-348">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="44773-348">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="44773-349">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="44773-349">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="44773-350">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="44773-350">Az.ServiceBus</span></span>
* <span data-ttu-id="44773-351">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="44773-351">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="44773-352">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="44773-352">Az.ServiceFabric</span></span>
* <span data-ttu-id="44773-353">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="44773-353">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="44773-354">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="44773-354">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="44773-355">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="44773-355">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="44773-356">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="44773-356">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="44773-357">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="44773-357">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="44773-358">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="44773-358">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="44773-359">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="44773-359">Az.Profile</span></span>
* <span data-ttu-id="44773-360">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="44773-360">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="44773-361">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="44773-361">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="44773-362">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="44773-362">Az.Compute</span></span>
* <span data-ttu-id="44773-363">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="44773-363">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="44773-364">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="44773-364">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="44773-365">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="44773-365">Az.DataLakeStore</span></span>
* <span data-ttu-id="44773-366">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="44773-366">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="44773-367">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="44773-367">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="44773-368">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="44773-368">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="44773-369">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="44773-369">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="44773-370">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="44773-370">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="44773-371">Az.Network</span><span class="sxs-lookup"><span data-stu-id="44773-371">Az.Network</span></span>
* <span data-ttu-id="44773-372">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="44773-372">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="44773-373">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="44773-373">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="44773-374">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44773-374">Az.Resources</span></span>
* <span data-ttu-id="44773-375">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="44773-375">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="44773-376">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="44773-376">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="44773-377">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="44773-377">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="44773-378">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="44773-378">Azure.Storage</span></span>
* <span data-ttu-id="44773-379">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="44773-379">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="44773-380">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="44773-380">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="44773-381">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="44773-381">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="44773-382">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="44773-382">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="44773-383">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="44773-383">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="44773-384">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="44773-384">Az.CognitiveServices</span></span>
* <span data-ttu-id="44773-385">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="44773-385">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="44773-386">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="44773-386">Az.Compute</span></span>
* <span data-ttu-id="44773-387">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="44773-387">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="44773-388">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="44773-388">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="44773-389">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="44773-389">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="44773-390">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="44773-390">Az.DataFactoryV2</span></span>
* <span data-ttu-id="44773-391">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="44773-391">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="44773-392">Az.Network</span><span class="sxs-lookup"><span data-stu-id="44773-392">Az.Network</span></span>
* <span data-ttu-id="44773-393">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="44773-393">Added NetworkProfile functionality.</span></span> <span data-ttu-id="44773-394">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="44773-394">new cmdlets added</span></span>
    - <span data-ttu-id="44773-395">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="44773-395">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="44773-396">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="44773-396">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="44773-397">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="44773-397">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="44773-398">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="44773-398">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="44773-399">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="44773-399">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="44773-400">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="44773-400">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="44773-401">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="44773-401">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="44773-402">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="44773-402">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="44773-403">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="44773-403">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="44773-404">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="44773-404">Az.RedisCache</span></span>
* <span data-ttu-id="44773-405">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="44773-405">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="44773-406">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="44773-406">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="44773-407">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44773-407">Az.Resources</span></span>
* <span data-ttu-id="44773-408">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="44773-408">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="44773-409">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="44773-409">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="44773-410">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="44773-410">Az.Sql</span></span>
* <span data-ttu-id="44773-411">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="44773-411">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="44773-412">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="44773-412">Az.Websites</span></span>
* <span data-ttu-id="44773-413">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="44773-413">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="44773-414">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="44773-414">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="44773-415">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="44773-415">0.2.0 - September 2018</span></span>
 <span data-ttu-id="44773-416">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="44773-416">Initial Release</span></span>