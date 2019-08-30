---
ms.openlocfilehash: f89d13d6bbedaea29b62287942d8c7a509abe32b
ms.sourcegitcommit: abca342d8687ca638679c049792d0cef6045837d
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/27/2019
ms.locfileid: "70052639"
---
## <a name="260---august-2019"></a><span data-ttu-id="41792-101">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="41792-101">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="41792-102">Geral</span><span class="sxs-lookup"><span data-stu-id="41792-102">General</span></span>
* <span data-ttu-id="41792-103">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="41792-103">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="41792-104">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="41792-104">Az.Accounts</span></span>
* <span data-ttu-id="41792-105">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="41792-105">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="41792-106">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="41792-106">Az.Aks</span></span>
* <span data-ttu-id="41792-107">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="41792-107">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="41792-108">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="41792-108">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="41792-109">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="41792-109">Az.ApiManagement</span></span>
* <span data-ttu-id="41792-110">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="41792-110">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="41792-111">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="41792-111">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="41792-112">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="41792-112">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="41792-113">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="41792-113">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="41792-114">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="41792-114">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="41792-115">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="41792-115">Az.Batch</span></span>
* <span data-ttu-id="41792-116">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="41792-116">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="41792-117">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="41792-117">Az.Cdn</span></span>
* <span data-ttu-id="41792-118">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="41792-118">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="41792-119">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="41792-119">Az.Compute</span></span>
* <span data-ttu-id="41792-120">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="41792-120">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="41792-121">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="41792-121">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="41792-122">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="41792-122">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="41792-123">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="41792-123">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="41792-124">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="41792-124">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="41792-125">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="41792-125">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="41792-126">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="41792-126">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="41792-127">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="41792-127">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="41792-128">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="41792-128">Az.DataFactory</span></span>
* <span data-ttu-id="41792-129">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="41792-129">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="41792-130">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="41792-130">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="41792-131">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="41792-131">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="41792-132">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="41792-132">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="41792-133">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="41792-133">Az.DataLakeStore</span></span>
* <span data-ttu-id="41792-134">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="41792-134">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="41792-135">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="41792-135">Az.EventHub</span></span>
* <span data-ttu-id="41792-136">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="41792-136">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="41792-137">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="41792-137">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="41792-138">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="41792-138">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="41792-139">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="41792-139">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="41792-140">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="41792-140">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="41792-141">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="41792-141">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="41792-142">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="41792-142">Az.Monitor</span></span>
* <span data-ttu-id="41792-143">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="41792-143">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="41792-144">Az.Network</span><span class="sxs-lookup"><span data-stu-id="41792-144">Az.Network</span></span>
* <span data-ttu-id="41792-145">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="41792-145">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="41792-146">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="41792-146">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="41792-147">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="41792-147">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="41792-148">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="41792-148">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="41792-149">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="41792-149">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="41792-150">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="41792-150">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="41792-151">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="41792-151">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="41792-152">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="41792-152">Az.OperationalInsights</span></span>
* <span data-ttu-id="41792-153">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="41792-153">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="41792-154">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="41792-154">Added example</span></span>
    - <span data-ttu-id="41792-155">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="41792-155">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="41792-156">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="41792-156">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="41792-157">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="41792-157">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="41792-158">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="41792-158">Az.RecoveryServices</span></span>
* <span data-ttu-id="41792-159">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="41792-159">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="41792-160">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="41792-160">Az.Resources</span></span>
* <span data-ttu-id="41792-161">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="41792-161">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="41792-162">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="41792-162">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="41792-163">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="41792-163">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="41792-164">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="41792-164">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="41792-165">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="41792-165">Az.ServiceBus</span></span>
* <span data-ttu-id="41792-166">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="41792-166">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="41792-167">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="41792-167">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="41792-168">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="41792-168">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="41792-169">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="41792-169">Az.ServiceFabric</span></span>
* <span data-ttu-id="41792-170">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="41792-170">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="41792-171">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="41792-171">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="41792-172">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="41792-172">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="41792-173">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="41792-173">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="41792-174">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="41792-174">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="41792-175">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="41792-175">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="41792-176">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="41792-176">Az.Sql</span></span>
* <span data-ttu-id="41792-177">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="41792-177">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="41792-178">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="41792-178">Az.Storage</span></span>
* <span data-ttu-id="41792-179">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="41792-179">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="41792-180">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="41792-180">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="41792-181">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="41792-181">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="41792-182">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="41792-182">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="41792-183">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="41792-183">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="41792-184">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="41792-184">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="41792-185">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="41792-185">Az.Websites</span></span>
* <span data-ttu-id="41792-186">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="41792-186">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="41792-187">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="41792-187">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="41792-188">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="41792-188">Az.Accounts</span></span>
* <span data-ttu-id="41792-189">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="41792-189">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="41792-190">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="41792-190">Az.ApplicationInsights</span></span>
* <span data-ttu-id="41792-191">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="41792-191">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="41792-192">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="41792-192">Az.Automation</span></span>
* <span data-ttu-id="41792-193">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="41792-193">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="41792-194">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="41792-194">Az.CognitiveServices</span></span>
* <span data-ttu-id="41792-195">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="41792-195">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="41792-196">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="41792-196">Az.Compute</span></span>
* <span data-ttu-id="41792-197">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="41792-197">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="41792-198">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="41792-198">Az.ContainerRegistry</span></span>
* <span data-ttu-id="41792-199">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="41792-199">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="41792-200">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="41792-200">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="41792-201">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="41792-201">Az.DataFactory</span></span>
* <span data-ttu-id="41792-202">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="41792-202">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="41792-203">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="41792-203">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="41792-204">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="41792-204">Az.EventHub</span></span>
* <span data-ttu-id="41792-205">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="41792-205">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="41792-206">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="41792-206">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="41792-207">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="41792-207">Az.KeyVault</span></span>
* <span data-ttu-id="41792-208">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="41792-208">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="41792-209">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="41792-209">Az.LogicApp</span></span>
* <span data-ttu-id="41792-210">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="41792-210">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="41792-211">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="41792-211">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="41792-212">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="41792-212">Az.ManagedServices</span></span>
* <span data-ttu-id="41792-213">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="41792-213">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="41792-214">Az.Network</span><span class="sxs-lookup"><span data-stu-id="41792-214">Az.Network</span></span>
* <span data-ttu-id="41792-215">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="41792-215">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="41792-216">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="41792-216">New cmdlets</span></span>
        - <span data-ttu-id="41792-217">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="41792-217">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="41792-218">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="41792-218">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="41792-219">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="41792-219">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="41792-220">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="41792-220">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="41792-221">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="41792-221">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="41792-222">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="41792-222">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="41792-223">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="41792-223">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="41792-224">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="41792-224">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="41792-225">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="41792-225">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="41792-226">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="41792-226">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="41792-227">Adicionado parâmetro opcional -PrivateEndpointNetworkPoliciesFlag para indicar a ativação ou desativação da aplicação de políticas de rede no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="41792-227">Added optional parameter -PrivateEndpointNetworkPoliciesFlag to indicate that enable or disable apply network policies on pivate endpoint in this subnet.</span></span>
        - <span data-ttu-id="41792-228">Adicionado parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag para indicar a ativação ou desativação da aplicação de políticas de rede no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="41792-228">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag to indicate that enable or disable apply network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="41792-229">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="41792-229">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="41792-230">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="41792-230">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="41792-231">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="41792-231">Updated cmdlets</span></span>
        - <span data-ttu-id="41792-232">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="41792-232">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="41792-233">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="41792-233">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="41792-234">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="41792-234">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="41792-235">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="41792-235">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="41792-236">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="41792-236">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="41792-237">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="41792-237">Updated cmdlet:</span></span>
        - <span data-ttu-id="41792-238">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="41792-238">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="41792-239">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="41792-239">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="41792-240">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="41792-240">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="41792-241">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="41792-241">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="41792-242">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="41792-242">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="41792-243">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="41792-243">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="41792-244">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="41792-244">Az.OperationalInsights</span></span>
* <span data-ttu-id="41792-245">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="41792-245">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="41792-246">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="41792-246">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="41792-247">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="41792-247">Az.RecoveryServices</span></span>
* <span data-ttu-id="41792-248">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="41792-248">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="41792-249">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="41792-249">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="41792-250">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="41792-250">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="41792-251">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="41792-251">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="41792-252">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="41792-252">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="41792-253">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="41792-253">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="41792-254">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="41792-254">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="41792-255">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="41792-255">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="41792-256">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="41792-256">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="41792-257">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="41792-257">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="41792-258">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="41792-258">Az.Resources</span></span>
- <span data-ttu-id="41792-259">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="41792-259">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="41792-260">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="41792-260">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="41792-261">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="41792-261">Az.ServiceBus</span></span>
* <span data-ttu-id="41792-262">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="41792-262">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="41792-263">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="41792-263">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="41792-264">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="41792-264">Az.Sql</span></span>
* <span data-ttu-id="41792-265">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="41792-265">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="41792-266">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="41792-266">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="41792-267">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="41792-267">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="41792-268">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="41792-268">Az.Storage</span></span>
* <span data-ttu-id="41792-269">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="41792-269">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="41792-270">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="41792-270">Az.StorageSync</span></span>
* <span data-ttu-id="41792-271">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="41792-271">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="41792-272">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="41792-272">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="41792-273">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="41792-273">Az.Websites</span></span>
* <span data-ttu-id="41792-274">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="41792-274">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="41792-275">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="41792-275">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="41792-276">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="41792-276">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="41792-277">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="41792-277">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="41792-278">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="41792-278">Az.Accounts</span></span>
* <span data-ttu-id="41792-279">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="41792-279">Add support for profile cmdlets</span></span>
* <span data-ttu-id="41792-280">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="41792-280">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="41792-281">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="41792-281">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="41792-282">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="41792-282">Az.Advisor</span></span>
* <span data-ttu-id="41792-283">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="41792-283">GA release of Az.Advisor</span></span>
* <span data-ttu-id="41792-284">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="41792-284">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="41792-285">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="41792-285">Az.ApiManagement</span></span>
* <span data-ttu-id="41792-286">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="41792-286">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="41792-287">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="41792-287">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="41792-288">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="41792-288">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="41792-289">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="41792-289">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="41792-290">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="41792-290">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="41792-291">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="41792-291">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="41792-292">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="41792-292">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="41792-293">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="41792-293">Az.Automation</span></span>
* <span data-ttu-id="41792-294">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="41792-294">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="41792-295">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="41792-295">Az.Compute</span></span>
* <span data-ttu-id="41792-296">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="41792-296">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="41792-297">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="41792-297">Az.DataFactory</span></span>
* <span data-ttu-id="41792-298">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="41792-298">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="41792-299">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="41792-299">Az.EventGrid</span></span>
* <span data-ttu-id="41792-300">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="41792-300">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="41792-301">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="41792-301">Az.IotHub</span></span>
* <span data-ttu-id="41792-302">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="41792-302">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="41792-303">Az.Network</span><span class="sxs-lookup"><span data-stu-id="41792-303">Az.Network</span></span>
* <span data-ttu-id="41792-304">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="41792-304">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="41792-305">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="41792-305">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="41792-306">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="41792-306">Az.PolicyInsights</span></span>
* <span data-ttu-id="41792-307">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="41792-307">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="41792-308">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="41792-308">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="41792-309">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="41792-309">Az.OperationalInsights</span></span>
* <span data-ttu-id="41792-310">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="41792-310">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="41792-311">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="41792-311">Az.RecoveryServices</span></span>
* <span data-ttu-id="41792-312">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="41792-312">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="41792-313">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="41792-313">Az.Resources</span></span>
    - <span data-ttu-id="41792-314">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="41792-314">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="41792-315">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="41792-315">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="41792-316">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="41792-316">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="41792-317">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="41792-317">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="41792-318">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="41792-318">Az.ServiceBus</span></span>
* <span data-ttu-id="41792-319">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="41792-319">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="41792-320">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="41792-320">Az.Sql</span></span>
* <span data-ttu-id="41792-321">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="41792-321">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="41792-322">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="41792-322">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="41792-323">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="41792-323">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="41792-324">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="41792-324">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="41792-325">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="41792-325">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="41792-326">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="41792-326">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="41792-327">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="41792-327">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="41792-328">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="41792-328">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="41792-329">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="41792-329">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="41792-330">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="41792-330">Az.Storage</span></span>
* <span data-ttu-id="41792-331">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="41792-331">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="41792-332">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="41792-332">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="41792-333">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="41792-333">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="41792-334">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="41792-334">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="41792-335">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="41792-335">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="41792-336">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="41792-336">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="41792-337">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="41792-337">Set-AzStorageAccount</span></span>
* <span data-ttu-id="41792-338">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="41792-338">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="41792-339">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="41792-339">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="41792-340">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="41792-340">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="41792-341">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="41792-341">Az.StorageSync</span></span>
* <span data-ttu-id="41792-342">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="41792-342">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="41792-343">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="41792-343">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="41792-344">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="41792-344">Az.Accounts</span></span>
* <span data-ttu-id="41792-345">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="41792-345">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="41792-346">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="41792-346">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="41792-347">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="41792-347">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="41792-348">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="41792-348">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="41792-349">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="41792-349">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="41792-350">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="41792-350">Az.Compute</span></span>
* <span data-ttu-id="41792-351">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="41792-351">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="41792-352">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="41792-352">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="41792-353">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="41792-353">Az.Dns</span></span>
* <span data-ttu-id="41792-354">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="41792-354">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="41792-355">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="41792-355">Az.EventGrid</span></span>
* <span data-ttu-id="41792-356">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="41792-356">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="41792-357">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="41792-357">New cmdlets:</span></span>
    - <span data-ttu-id="41792-358">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="41792-358">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="41792-359">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="41792-359">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="41792-360">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="41792-360">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="41792-361">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="41792-361">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="41792-362">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="41792-362">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="41792-363">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="41792-363">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="41792-364">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="41792-364">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="41792-365">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="41792-365">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="41792-366">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="41792-366">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="41792-367">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="41792-367">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="41792-368">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="41792-368">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="41792-369">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="41792-369">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="41792-370">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="41792-370">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="41792-371">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="41792-371">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="41792-372">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="41792-372">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="41792-373">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="41792-373">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="41792-374">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="41792-374">Updated cmdlets:</span></span>
    - <span data-ttu-id="41792-375">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="41792-375">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="41792-376">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="41792-376">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="41792-377">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="41792-377">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="41792-378">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="41792-378">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="41792-379">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="41792-379">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="41792-380">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="41792-380">Event subscription expiration date,</span></span>
            - <span data-ttu-id="41792-381">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="41792-381">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="41792-382">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="41792-382">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="41792-383">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="41792-383">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="41792-384">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="41792-384">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="41792-385">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="41792-385">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="41792-386">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="41792-386">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="41792-387">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="41792-387">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="41792-388">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="41792-388">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="41792-389">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="41792-389">Az.FrontDoor</span></span>
* <span data-ttu-id="41792-390">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="41792-390">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="41792-391">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="41792-391">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="41792-392">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="41792-392">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="41792-393">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="41792-393">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="41792-394">Az.Network</span><span class="sxs-lookup"><span data-stu-id="41792-394">Az.Network</span></span>
* <span data-ttu-id="41792-395">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="41792-395">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="41792-396">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="41792-396">New cmdlets</span></span>
        - <span data-ttu-id="41792-397">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="41792-397">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="41792-398">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="41792-398">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="41792-399">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="41792-399">New cmdlets</span></span> 
        - <span data-ttu-id="41792-400">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="41792-400">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="41792-401">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="41792-401">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="41792-402">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="41792-402">New cmdlets</span></span> 
        - <span data-ttu-id="41792-403">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="41792-403">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="41792-404">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="41792-404">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="41792-405">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="41792-405">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="41792-406">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="41792-406">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="41792-407">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="41792-407">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="41792-408">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="41792-408">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="41792-409">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="41792-409">New cmdlets</span></span>
        - <span data-ttu-id="41792-410">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="41792-410">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="41792-411">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="41792-411">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="41792-412">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="41792-412">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="41792-413">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="41792-413">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="41792-414">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="41792-414">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="41792-415">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="41792-415">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="41792-416">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="41792-416">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="41792-417">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="41792-417">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="41792-418">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="41792-418">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="41792-419">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="41792-419">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="41792-420">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="41792-420">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="41792-421">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="41792-421">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="41792-422">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="41792-422">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="41792-423">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="41792-423">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="41792-424">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="41792-424">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="41792-425">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="41792-425">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="41792-426">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="41792-426">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="41792-427">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="41792-427">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="41792-428">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="41792-428">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="41792-429">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="41792-429">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="41792-430">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="41792-430">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="41792-431">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="41792-431">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="41792-432">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="41792-432">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="41792-433">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="41792-433">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="41792-434">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="41792-434">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="41792-435">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="41792-435">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="41792-436">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="41792-436">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="41792-437">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="41792-437">Az.OperationalInsights</span></span>
* <span data-ttu-id="41792-438">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="41792-438">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="41792-439">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="41792-439">Az.Resources</span></span>
* <span data-ttu-id="41792-440">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="41792-440">Support for additional Template Export options</span></span>
    - <span data-ttu-id="41792-441">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="41792-441">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="41792-442">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="41792-442">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="41792-443">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="41792-443">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="41792-444">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="41792-444">Az.ServiceFabric</span></span>
* <span data-ttu-id="41792-445">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="41792-445">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="41792-446">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="41792-446">Az.Sql</span></span>
* <span data-ttu-id="41792-447">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="41792-447">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="41792-448">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="41792-448">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="41792-449">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="41792-449">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="41792-450">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="41792-450">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="41792-451">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="41792-451">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="41792-452">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="41792-452">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="41792-453">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="41792-453">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="41792-454">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="41792-454">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="41792-455">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="41792-455">Az.Storage</span></span>
* <span data-ttu-id="41792-456">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="41792-456">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="41792-457">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="41792-457">New-AzStorageAccount</span></span>
* <span data-ttu-id="41792-458">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="41792-458">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="41792-459">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="41792-459">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="41792-460">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="41792-460">Az.Websites</span></span>
* <span data-ttu-id="41792-461">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="41792-461">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="41792-462">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="41792-462">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="41792-463">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="41792-463">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="41792-464">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="41792-464">Az.Cdn</span></span>
* <span data-ttu-id="41792-465">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="41792-465">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="41792-466">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="41792-466">Az.Compute</span></span>
* <span data-ttu-id="41792-467">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="41792-467">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="41792-468">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="41792-468">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="41792-469">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="41792-469">Az.EventHub</span></span>
* <span data-ttu-id="41792-470">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="41792-470">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="41792-471">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="41792-471">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="41792-472">Az.Network</span><span class="sxs-lookup"><span data-stu-id="41792-472">Az.Network</span></span>
* <span data-ttu-id="41792-473">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="41792-473">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="41792-474">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="41792-474">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="41792-475">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="41792-475">Az.PolicyInsights</span></span>
* <span data-ttu-id="41792-476">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="41792-476">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="41792-477">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="41792-477">Az.RecoveryServices</span></span>
* <span data-ttu-id="41792-478">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="41792-478">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="41792-479">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="41792-479">Az.ServiceBus</span></span>
* <span data-ttu-id="41792-480">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="41792-480">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="41792-481">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="41792-481">Az.ServiceFabric</span></span>
* <span data-ttu-id="41792-482">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="41792-482">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="41792-483">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="41792-483">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="41792-484">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="41792-484">Az.Sql</span></span>
* <span data-ttu-id="41792-485">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="41792-485">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="41792-486">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="41792-486">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="41792-487">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="41792-487">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="41792-488">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="41792-488">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="41792-489">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="41792-489">Az.Websites</span></span>
* <span data-ttu-id="41792-490">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="41792-490">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="41792-491">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="41792-491">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="41792-492">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="41792-492">Az.ApiManagement</span></span>
* <span data-ttu-id="41792-493">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="41792-493">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="41792-494">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="41792-494">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="41792-495">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="41792-495">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="41792-496">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="41792-496">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="41792-497">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="41792-497">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="41792-498">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="41792-498">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="41792-499">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="41792-499">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="41792-500">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="41792-500">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="41792-501">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="41792-501">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="41792-502">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="41792-502">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="41792-503">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="41792-503">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="41792-504">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="41792-504">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="41792-505">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="41792-505">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="41792-506">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="41792-506">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="41792-507">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="41792-507">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="41792-508">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="41792-508">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="41792-509">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="41792-509">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="41792-510">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="41792-510">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="41792-511">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="41792-511">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="41792-512">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="41792-512">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="41792-513">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="41792-513">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="41792-514">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="41792-514">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="41792-515">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="41792-515">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="41792-516">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="41792-516">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="41792-517">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="41792-517">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="41792-518">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="41792-518">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="41792-519">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="41792-519">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="41792-520">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="41792-520">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="41792-521">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="41792-521">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="41792-522">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="41792-522">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="41792-523">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="41792-523">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="41792-524">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="41792-524">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="41792-525">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="41792-525">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="41792-526">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="41792-526">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="41792-527">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="41792-527">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="41792-528">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="41792-528">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="41792-529">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="41792-529">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="41792-530">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="41792-530">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="41792-531">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="41792-531">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="41792-532">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="41792-532">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="41792-533">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="41792-533">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="41792-534">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="41792-534">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="41792-535">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="41792-535">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="41792-536">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="41792-536">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="41792-537">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="41792-537">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="41792-538">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="41792-538">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="41792-539">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="41792-539">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="41792-540">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="41792-540">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="41792-541">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="41792-541">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="41792-542">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="41792-542">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="41792-543">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="41792-543">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="41792-544">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="41792-544">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="41792-545">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="41792-545">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="41792-546">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="41792-546">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="41792-547">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="41792-547">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="41792-548">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="41792-548">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="41792-549">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="41792-549">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="41792-550">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="41792-550">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="41792-551">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="41792-551">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="41792-552">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="41792-552">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="41792-553">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="41792-553">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="41792-554">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="41792-554">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="41792-555">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="41792-555">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="41792-556">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="41792-556">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="41792-557">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="41792-557">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="41792-558">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="41792-558">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="41792-559">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="41792-559">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="41792-560">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="41792-560">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="41792-561">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="41792-561">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="41792-562">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="41792-562">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="41792-563">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="41792-563">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="41792-564">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="41792-564">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="41792-565">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="41792-565">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="41792-566">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="41792-566">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="41792-567">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="41792-567">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="41792-568">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="41792-568">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="41792-569">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="41792-569">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="41792-570">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="41792-570">Az.Automation</span></span>
* <span data-ttu-id="41792-571">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="41792-571">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="41792-572">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="41792-572">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="41792-573">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="41792-573">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="41792-574">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="41792-574">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="41792-575">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="41792-575">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="41792-576">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="41792-576">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="41792-577">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="41792-577">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="41792-578">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="41792-578">Az.Compute</span></span>
* <span data-ttu-id="41792-579">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="41792-579">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="41792-580">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="41792-580">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="41792-581">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="41792-581">Az.DataLakeStore</span></span>
* <span data-ttu-id="41792-582">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="41792-582">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="41792-583">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="41792-583">Az.Monitor</span></span>
* <span data-ttu-id="41792-584">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="41792-584">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="41792-585">Az.Network</span><span class="sxs-lookup"><span data-stu-id="41792-585">Az.Network</span></span>
* <span data-ttu-id="41792-586">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="41792-586">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="41792-587">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="41792-587">Updated cmdlet:</span></span>
        - <span data-ttu-id="41792-588">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="41792-588">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="41792-589">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="41792-589">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="41792-590">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="41792-590">Az.Resources</span></span>
* <span data-ttu-id="41792-591">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="41792-591">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="41792-592">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="41792-592">Az.Sql</span></span>
* <span data-ttu-id="41792-593">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="41792-593">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="41792-594">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="41792-594">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="41792-595">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="41792-595">Az.Accounts</span></span>
* <span data-ttu-id="41792-596">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="41792-596">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="41792-597">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="41792-597">Az.CognitiveServices</span></span>
* <span data-ttu-id="41792-598">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="41792-598">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="41792-599">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="41792-599">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="41792-600">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="41792-600">Az.Compute</span></span>
* <span data-ttu-id="41792-601">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="41792-601">Proximity placement group feature.</span></span>
    - <span data-ttu-id="41792-602">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="41792-602">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="41792-603">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="41792-603">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="41792-604">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="41792-604">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="41792-605">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="41792-605">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="41792-606">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="41792-606">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="41792-607">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="41792-607">Breaking changes</span></span>
    - <span data-ttu-id="41792-608">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="41792-608">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="41792-609">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="41792-609">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="41792-610">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="41792-610">Az.DeploymentManager</span></span>
* <span data-ttu-id="41792-611">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="41792-611">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="41792-612">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="41792-612">Az.Dns</span></span>
* <span data-ttu-id="41792-613">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="41792-613">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="41792-614">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="41792-614">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="41792-615">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="41792-615">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="41792-616">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="41792-616">Az.FrontDoor</span></span>
* <span data-ttu-id="41792-617">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="41792-617">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="41792-618">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="41792-618">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="41792-619">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="41792-619">Az.HDInsight</span></span>
* <span data-ttu-id="41792-620">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="41792-620">Removed two cmdlets:</span></span>
    - <span data-ttu-id="41792-621">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="41792-621">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="41792-622">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="41792-622">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="41792-623">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="41792-623">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="41792-624">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="41792-624">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="41792-625">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="41792-625">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="41792-626">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="41792-626">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="41792-627">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="41792-627">Az.Monitor</span></span>
* <span data-ttu-id="41792-628">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="41792-628">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="41792-629">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="41792-629">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="41792-630">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="41792-630">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="41792-631">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="41792-631">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="41792-632">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="41792-632">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="41792-633">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="41792-633">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="41792-634">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="41792-634">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="41792-635">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="41792-635">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="41792-636">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="41792-636">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="41792-637">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="41792-637">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="41792-638">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="41792-638">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="41792-639">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="41792-639">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="41792-640">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="41792-640">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="41792-641">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="41792-641">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="41792-642">Az.Network</span><span class="sxs-lookup"><span data-stu-id="41792-642">Az.Network</span></span>
* <span data-ttu-id="41792-643">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="41792-643">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="41792-644">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="41792-644">New cmdlets</span></span>
        - <span data-ttu-id="41792-645">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="41792-645">New-AzNatGateway</span></span>
        - <span data-ttu-id="41792-646">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="41792-646">Get-AzNatGateway</span></span>
        - <span data-ttu-id="41792-647">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="41792-647">Set-AzNatGateway</span></span>
        - <span data-ttu-id="41792-648">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="41792-648">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="41792-649">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="41792-649">Updated cmdlets</span></span>
        - <span data-ttu-id="41792-650">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="41792-650">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="41792-651">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="41792-651">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="41792-652">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="41792-652">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="41792-653">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="41792-653">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="41792-654">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="41792-654">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="41792-655">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="41792-655">Az.PolicyInsights</span></span>
* <span data-ttu-id="41792-656">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="41792-656">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="41792-657">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="41792-657">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="41792-658">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="41792-658">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="41792-659">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="41792-659">Az.RecoveryServices</span></span>
* <span data-ttu-id="41792-660">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="41792-660">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="41792-661">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="41792-661">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="41792-662">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="41792-662">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="41792-663">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="41792-663">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="41792-664">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="41792-664">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="41792-665">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="41792-665">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="41792-666">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="41792-666">Az.Relay</span></span>
* <span data-ttu-id="41792-667">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="41792-667">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="41792-668">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="41792-668">Az.ServiceBus</span></span>
* <span data-ttu-id="41792-669">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="41792-669">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="41792-670">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="41792-670">Az.Storage</span></span>
* <span data-ttu-id="41792-671">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="41792-671">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="41792-672">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="41792-672">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="41792-673">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="41792-673">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="41792-674">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="41792-674">New-AzStorageAccount</span></span>
* <span data-ttu-id="41792-675">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="41792-675">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="41792-676">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="41792-676">New-AzStorageAccount</span></span>
    - <span data-ttu-id="41792-677">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="41792-677">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="41792-678">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="41792-678">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="41792-679">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="41792-679">Az.Websites</span></span>
* <span data-ttu-id="41792-680">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="41792-680">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="41792-681">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="41792-681">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="41792-682">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="41792-682">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="41792-683">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="41792-683">Highlights since the last major release</span></span>
* <span data-ttu-id="41792-684">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="41792-684">General availability of `Az` module</span></span>
* <span data-ttu-id="41792-685">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="41792-685">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="41792-686">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="41792-686">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="41792-687">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="41792-687">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="41792-688">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="41792-688">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="41792-689">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="41792-689">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="41792-690">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="41792-690">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="41792-691">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="41792-691">Az.Accounts</span></span>
* <span data-ttu-id="41792-692">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="41792-692">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="41792-693">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="41792-693">Az.Batch</span></span>
* <span data-ttu-id="41792-694">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="41792-694">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="41792-695">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="41792-695">Az.Cdn</span></span>
* <span data-ttu-id="41792-696">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="41792-696">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="41792-697">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="41792-697">Az.CognitiveServices</span></span>
* <span data-ttu-id="41792-698">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="41792-698">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="41792-699">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="41792-699">Az.Compute</span></span>
* <span data-ttu-id="41792-700">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="41792-700">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="41792-701">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="41792-701">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="41792-702">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="41792-702">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="41792-703">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="41792-703">Az.DataFactory</span></span>
* <span data-ttu-id="41792-704">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="41792-704">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="41792-705">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="41792-705">Az.DataLakeStore</span></span>
* <span data-ttu-id="41792-706">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="41792-706">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="41792-707">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="41792-707">Az.EventGrid</span></span>
* <span data-ttu-id="41792-708">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="41792-708">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="41792-709">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="41792-709">Az.EventHub</span></span>
* <span data-ttu-id="41792-710">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="41792-710">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="41792-711">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="41792-711">Az.HDInsight</span></span>
* <span data-ttu-id="41792-712">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="41792-712">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="41792-713">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="41792-713">Az.IotHub</span></span>
* <span data-ttu-id="41792-714">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="41792-714">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="41792-715">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="41792-715">Az.KeyVault</span></span>
* <span data-ttu-id="41792-716">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="41792-716">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="41792-717">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="41792-717">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="41792-718">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="41792-718">Az.MachineLearning</span></span>
* <span data-ttu-id="41792-719">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="41792-719">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="41792-720">Az.Media</span><span class="sxs-lookup"><span data-stu-id="41792-720">Az.Media</span></span>
* <span data-ttu-id="41792-721">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="41792-721">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="41792-722">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="41792-722">Az.Monitor</span></span>
  * <span data-ttu-id="41792-723">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="41792-723">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="41792-724">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="41792-724">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="41792-725">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="41792-725">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="41792-726">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="41792-726">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="41792-727">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="41792-727">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="41792-728">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="41792-728">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="41792-729">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="41792-729">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="41792-730">Az.Network</span><span class="sxs-lookup"><span data-stu-id="41792-730">Az.Network</span></span>
* <span data-ttu-id="41792-731">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="41792-731">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="41792-732">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="41792-732">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="41792-733">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="41792-733">Az.NotificationHubs</span></span>
* <span data-ttu-id="41792-734">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="41792-734">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="41792-735">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="41792-735">Az.OperationalInsights</span></span>
* <span data-ttu-id="41792-736">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="41792-736">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="41792-737">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="41792-737">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="41792-738">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="41792-738">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="41792-739">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="41792-739">Az.RecoveryServices</span></span>
* <span data-ttu-id="41792-740">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="41792-740">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="41792-741">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="41792-741">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="41792-742">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="41792-742">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="41792-743">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="41792-743">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="41792-744">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="41792-744">Az.RedisCache</span></span>
* <span data-ttu-id="41792-745">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="41792-745">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="41792-746">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="41792-746">Az.Resources</span></span>
* <span data-ttu-id="41792-747">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="41792-747">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="41792-748">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="41792-748">Az.Sql</span></span>
* <span data-ttu-id="41792-749">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="41792-749">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="41792-750">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="41792-750">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="41792-751">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="41792-751">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="41792-752">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="41792-752">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="41792-753">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="41792-753">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="41792-754">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="41792-754">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="41792-755">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="41792-755">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="41792-756">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="41792-756">Az.Websites</span></span>
* <span data-ttu-id="41792-757">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="41792-757">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="41792-758">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="41792-758">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="41792-759">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="41792-759">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="41792-760">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="41792-760">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="41792-761">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="41792-761">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="41792-762">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="41792-762">Highlights since the last major release</span></span>
* <span data-ttu-id="41792-763">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="41792-763">General availability of `Az` module</span></span>
* <span data-ttu-id="41792-764">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="41792-764">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="41792-765">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="41792-765">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="41792-766">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="41792-766">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="41792-767">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="41792-767">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="41792-768">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="41792-768">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="41792-769">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="41792-769">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="41792-770">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="41792-770">Az.Accounts</span></span>
* <span data-ttu-id="41792-771">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="41792-771">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="41792-772">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="41792-772">Az.AnalysisServices</span></span>
* <span data-ttu-id="41792-773">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="41792-773">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="41792-774">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="41792-774">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="41792-775">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="41792-775">Az.Automation</span></span>
* <span data-ttu-id="41792-776">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="41792-776">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="41792-777">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="41792-777">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="41792-778">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="41792-778">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="41792-779">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="41792-779">Az.Compute</span></span>
* <span data-ttu-id="41792-780">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="41792-780">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="41792-781">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="41792-781">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="41792-782">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="41792-782">Az.ContainerInstance</span></span>
* <span data-ttu-id="41792-783">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="41792-783">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="41792-784">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="41792-784">Az.DataFactory</span></span>
* <span data-ttu-id="41792-785">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="41792-785">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="41792-786">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="41792-786">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="41792-787">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="41792-787">Az.Resources</span></span>
* <span data-ttu-id="41792-788">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="41792-788">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="41792-789">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="41792-789">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="41792-790">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="41792-790">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="41792-791">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="41792-791">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="41792-792">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="41792-792">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="41792-793">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="41792-793">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="41792-794">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="41792-794">Az.Sql</span></span>
* <span data-ttu-id="41792-795">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="41792-795">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="41792-796">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="41792-796">Az.Storage</span></span>
* <span data-ttu-id="41792-797">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="41792-797">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="41792-798">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="41792-798">New-AzStorageContext</span></span>
* <span data-ttu-id="41792-799">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="41792-799">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="41792-800">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="41792-800">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="41792-801">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="41792-801">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="41792-802">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="41792-802">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="41792-803">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="41792-803">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="41792-804">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="41792-804">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="41792-805">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="41792-805">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="41792-806">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="41792-806">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="41792-807">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="41792-807">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="41792-808">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="41792-808">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="41792-809">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="41792-809">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="41792-810">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="41792-810">Highlights since the last major release</span></span>
* <span data-ttu-id="41792-811">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="41792-811">General availability of `Az` module</span></span>
* <span data-ttu-id="41792-812">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="41792-812">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="41792-813">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="41792-813">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="41792-814">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="41792-814">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="41792-815">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="41792-815">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="41792-816">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="41792-816">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="41792-817">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="41792-817">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="41792-818">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="41792-818">Az.Automation</span></span>
* <span data-ttu-id="41792-819">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="41792-819">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="41792-820">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="41792-820">Dynamic grouping</span></span>
    * <span data-ttu-id="41792-821">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="41792-821">Pre-Post script</span></span>
    * <span data-ttu-id="41792-822">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="41792-822">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="41792-823">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="41792-823">Az.Compute</span></span>
* <span data-ttu-id="41792-824">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="41792-824">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="41792-825">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="41792-825">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="41792-826">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="41792-826">Az.KeyVault</span></span>
* <span data-ttu-id="41792-827">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="41792-827">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="41792-828">Az.Network</span><span class="sxs-lookup"><span data-stu-id="41792-828">Az.Network</span></span>
* <span data-ttu-id="41792-829">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="41792-829">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="41792-830">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="41792-830">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="41792-831">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="41792-831">Az.RecoveryServices</span></span>
* <span data-ttu-id="41792-832">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="41792-832">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="41792-833">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="41792-833">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="41792-834">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="41792-834">Az.Resources</span></span>
* <span data-ttu-id="41792-835">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="41792-835">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="41792-836">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="41792-836">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="41792-837">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="41792-837">Az.Sql</span></span>
* <span data-ttu-id="41792-838">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="41792-838">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="41792-839">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="41792-839">Az.Storage</span></span>
* <span data-ttu-id="41792-840">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="41792-840">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="41792-841">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="41792-841">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="41792-842">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="41792-842">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="41792-843">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="41792-843">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="41792-844">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="41792-844">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="41792-845">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="41792-845">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="41792-846">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="41792-846">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="41792-847">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="41792-847">Az.Websites</span></span>
* <span data-ttu-id="41792-848">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="41792-848">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="41792-849">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="41792-849">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="41792-850">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="41792-850">Az.Accounts</span></span>
* <span data-ttu-id="41792-851">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="41792-851">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="41792-852">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="41792-852">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="41792-853">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="41792-853">Az.Automation</span></span>
* <span data-ttu-id="41792-854">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="41792-854">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="41792-855">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="41792-855">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="41792-856">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="41792-856">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="41792-857">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="41792-857">Az.Cdn</span></span>
* <span data-ttu-id="41792-858">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="41792-858">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="41792-859">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="41792-859">Az.Compute</span></span>
* <span data-ttu-id="41792-860">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="41792-860">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="41792-861">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="41792-861">Az.DataFactory</span></span>
* <span data-ttu-id="41792-862">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="41792-862">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="41792-863">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="41792-863">Az.LogicApp</span></span>
* <span data-ttu-id="41792-864">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="41792-864">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="41792-865">Az.Network</span><span class="sxs-lookup"><span data-stu-id="41792-865">Az.Network</span></span>
* <span data-ttu-id="41792-866">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="41792-866">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="41792-867">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="41792-867">Az.RecoveryServices</span></span>
* <span data-ttu-id="41792-868">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="41792-868">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="41792-869">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="41792-869">SDK Update</span></span>
* <span data-ttu-id="41792-870">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="41792-870">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="41792-871">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="41792-871">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="41792-872">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="41792-872">Az.Resources</span></span>
* <span data-ttu-id="41792-873">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="41792-873">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="41792-874">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="41792-874">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="41792-875">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="41792-875">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="41792-876">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="41792-876">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="41792-877">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="41792-877">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="41792-878">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="41792-878">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="41792-879">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="41792-879">Az.Sql</span></span>
* <span data-ttu-id="41792-880">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="41792-880">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="41792-881">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="41792-881">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="41792-882">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="41792-882">Az.Storage</span></span>
* <span data-ttu-id="41792-883">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="41792-883">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="41792-884">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="41792-884">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="41792-885">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="41792-885">Az.AnalysisServices</span></span>
* <span data-ttu-id="41792-886">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="41792-886">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="41792-887">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="41792-887">Az.Automation</span></span>
* <span data-ttu-id="41792-888">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="41792-888">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="41792-889">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="41792-889">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="41792-890">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="41792-890">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="41792-891">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="41792-891">Az.CognitiveServices</span></span>
* <span data-ttu-id="41792-892">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="41792-892">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="41792-893">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="41792-893">Az.Compute</span></span>
* <span data-ttu-id="41792-894">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="41792-894">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="41792-895">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="41792-895">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="41792-896">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="41792-896">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="41792-897">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="41792-897">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="41792-898">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="41792-898">Az.DataLakeStore</span></span>
* <span data-ttu-id="41792-899">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="41792-899">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="41792-900">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="41792-900">Az.EventHub</span></span>
* <span data-ttu-id="41792-901">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="41792-901">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="41792-902">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="41792-902">Az.KeyVault</span></span>
* <span data-ttu-id="41792-903">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="41792-903">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="41792-904">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="41792-904">Az.LogicApp</span></span>
* <span data-ttu-id="41792-905">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="41792-905">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="41792-906">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="41792-906">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="41792-907">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="41792-907">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="41792-908">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="41792-908">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="41792-909">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="41792-909">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="41792-910">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="41792-910">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="41792-911">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="41792-911">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="41792-912">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="41792-912">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="41792-913">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="41792-913">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="41792-914">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="41792-914">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="41792-915">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="41792-915">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="41792-916">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="41792-916">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="41792-917">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="41792-917">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="41792-918">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="41792-918">Az.Monitor</span></span>
* <span data-ttu-id="41792-919">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="41792-919">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="41792-920">Az.Network</span><span class="sxs-lookup"><span data-stu-id="41792-920">Az.Network</span></span>
* <span data-ttu-id="41792-921">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="41792-921">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="41792-922">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="41792-922">Az.OperationalInsights</span></span>
* <span data-ttu-id="41792-923">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="41792-923">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="41792-924">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="41792-924">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="41792-925">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="41792-925">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="41792-926">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="41792-926">Az.Resources</span></span>
* <span data-ttu-id="41792-927">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="41792-927">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="41792-928">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="41792-928">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="41792-929">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="41792-929">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="41792-930">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="41792-930">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="41792-931">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="41792-931">Az.Sql</span></span>
* <span data-ttu-id="41792-932">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="41792-932">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="41792-933">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="41792-933">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="41792-934">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="41792-934">Az.Websites</span></span>
* <span data-ttu-id="41792-935">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="41792-935">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="41792-936">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="41792-936">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="41792-937">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="41792-937">Az.Accounts</span></span>
* <span data-ttu-id="41792-938">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="41792-938">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="41792-939">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="41792-939">Az.AnalysisServices</span></span>
<span data-ttu-id="41792-940">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="41792-940">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="41792-941">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="41792-941">Az.Compute</span></span>
* <span data-ttu-id="41792-942">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="41792-942">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="41792-943">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="41792-943">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="41792-944">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="41792-944">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="41792-945">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="41792-945">Az.RecoveryServices</span></span>
<span data-ttu-id="41792-946">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="41792-946">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="41792-947">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="41792-947">Az.Resources</span></span>
* <span data-ttu-id="41792-948">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="41792-948">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="41792-949">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="41792-949">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="41792-950">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="41792-950">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="41792-951">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="41792-951">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="41792-952">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="41792-952">Az.Sql</span></span>
* <span data-ttu-id="41792-953">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="41792-953">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="41792-954">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="41792-954">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="41792-955">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="41792-955">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="41792-956">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="41792-956">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="41792-957">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="41792-957">Az.Accounts</span></span>
* <span data-ttu-id="41792-958">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="41792-958">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="41792-959">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="41792-959">Az.AnalysisServices</span></span>
* <span data-ttu-id="41792-960">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="41792-960">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="41792-961">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="41792-961">Az.RecoveryServices</span></span>
* <span data-ttu-id="41792-962">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="41792-962">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="41792-963">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="41792-963">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="41792-964">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="41792-964">Az.Accounts</span></span>
* <span data-ttu-id="41792-965">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="41792-965">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="41792-966">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="41792-966">Update incorrect online help URLs</span></span>
* <span data-ttu-id="41792-967">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="41792-967">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="41792-968">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="41792-968">Az.Aks</span></span>
* <span data-ttu-id="41792-969">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="41792-969">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="41792-970">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="41792-970">Az.Automation</span></span>
* <span data-ttu-id="41792-971">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="41792-971">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="41792-972">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="41792-972">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="41792-973">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="41792-973">Az.Cdn</span></span>
* <span data-ttu-id="41792-974">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="41792-974">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="41792-975">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="41792-975">Az.Compute</span></span>
* <span data-ttu-id="41792-976">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="41792-976">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="41792-977">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="41792-977">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="41792-978">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="41792-978">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="41792-979">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="41792-979">Az.ContainerRegistry</span></span>
* <span data-ttu-id="41792-980">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="41792-980">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="41792-981">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="41792-981">Az.DataFactory</span></span>
* <span data-ttu-id="41792-982">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="41792-982">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="41792-983">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="41792-983">Az.DataLakeStore</span></span>
* <span data-ttu-id="41792-984">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="41792-984">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="41792-985">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="41792-985">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="41792-986">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="41792-986">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="41792-987">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="41792-987">Az.IotHub</span></span>
* <span data-ttu-id="41792-988">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="41792-988">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="41792-989">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="41792-989">Az.KeyVault</span></span>
* <span data-ttu-id="41792-990">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="41792-990">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="41792-991">Az.Network</span><span class="sxs-lookup"><span data-stu-id="41792-991">Az.Network</span></span>
* <span data-ttu-id="41792-992">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="41792-992">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="41792-993">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="41792-993">Az.Resources</span></span>
* <span data-ttu-id="41792-994">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="41792-994">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="41792-995">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="41792-995">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="41792-996">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="41792-996">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="41792-997">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="41792-997">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="41792-998">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="41792-998">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="41792-999">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="41792-999">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="41792-1000">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="41792-1000">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="41792-1001">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="41792-1001">Az.ServiceFabric</span></span>
* <span data-ttu-id="41792-1002">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="41792-1002">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="41792-1003">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="41792-1003">Fix some error messages.</span></span>
* <span data-ttu-id="41792-1004">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="41792-1004">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="41792-1005">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="41792-1005">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="41792-1006">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="41792-1006">Az.SignalR</span></span>
* <span data-ttu-id="41792-1007">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="41792-1007">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="41792-1008">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="41792-1008">Az.Sql</span></span>
* <span data-ttu-id="41792-1009">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="41792-1009">Update incorrect online help URLs</span></span>
* <span data-ttu-id="41792-1010">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="41792-1010">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="41792-1011">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="41792-1011">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="41792-1012">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="41792-1012">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="41792-1013">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="41792-1013">Az.Storage</span></span>
* <span data-ttu-id="41792-1014">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="41792-1014">Update incorrect online help URLs</span></span>
* <span data-ttu-id="41792-1015">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="41792-1015">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="41792-1016">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="41792-1016">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="41792-1017">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="41792-1017">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="41792-1018">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="41792-1018">Az.TrafficManager</span></span>
* <span data-ttu-id="41792-1019">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="41792-1019">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="41792-1020">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="41792-1020">Az.Websites</span></span>
* <span data-ttu-id="41792-1021">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="41792-1021">Update incorrect online help URLs</span></span>
* <span data-ttu-id="41792-1022">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="41792-1022">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="41792-1023">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="41792-1023">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="41792-1024">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="41792-1024">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="41792-1025">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="41792-1025">Az.Accounts</span></span>
* <span data-ttu-id="41792-1026">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="41792-1026">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="41792-1027">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="41792-1027">Az.Compute</span></span>
* <span data-ttu-id="41792-1028">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="41792-1028">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="41792-1029">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="41792-1029">Updated the description of ID in help files</span></span>
* <span data-ttu-id="41792-1030">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="41792-1030">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="41792-1031">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="41792-1031">Az.DataLakeStore</span></span>
* <span data-ttu-id="41792-1032">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="41792-1032">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="41792-1033">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="41792-1033">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="41792-1034">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="41792-1034">Az.EventGrid</span></span>
* <span data-ttu-id="41792-1035">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="41792-1035">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="41792-1036">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="41792-1036">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="41792-1037">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="41792-1037">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="41792-1038">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="41792-1038">Event Time-To-Live,</span></span>
        - <span data-ttu-id="41792-1039">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="41792-1039">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="41792-1040">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="41792-1040">Dead letter endpoint.</span></span>
    - <span data-ttu-id="41792-1041">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="41792-1041">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="41792-1042">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="41792-1042">Event Time-To-Live,</span></span>
        - <span data-ttu-id="41792-1043">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="41792-1043">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="41792-1044">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="41792-1044">Dead letter endpoint.</span></span>
* <span data-ttu-id="41792-1045">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="41792-1045">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="41792-1046">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="41792-1046">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="41792-1047">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="41792-1047">Az.IotHub</span></span>
* <span data-ttu-id="41792-1048">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="41792-1048">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="41792-1049">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="41792-1049">Az.LogicApp</span></span>
* <span data-ttu-id="41792-1050">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="41792-1050">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="41792-1051">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="41792-1051">Az.Resources</span></span>
* <span data-ttu-id="41792-1052">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="41792-1052">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="41792-1053">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="41792-1053">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="41792-1054">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="41792-1054">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="41792-1055">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="41792-1055">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="41792-1056">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="41792-1056">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="41792-1057">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="41792-1057">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="41792-1058">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="41792-1058">Az.SignalR</span></span>
* <span data-ttu-id="41792-1059">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="41792-1059">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="41792-1060">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="41792-1060">Az.Sql</span></span>
* <span data-ttu-id="41792-1061">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="41792-1061">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="41792-1062">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="41792-1062">Az.Storage</span></span>
* <span data-ttu-id="41792-1063">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="41792-1063">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="41792-1064">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="41792-1064">New-AzStorageContext</span></span>
* <span data-ttu-id="41792-1065">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="41792-1065">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="41792-1066">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="41792-1066">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="41792-1067">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="41792-1067">Az.Websites</span></span>
* <span data-ttu-id="41792-1068">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="41792-1068">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="41792-1069">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="41792-1069">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="41792-1070">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="41792-1070">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="41792-1071">Geral</span><span class="sxs-lookup"><span data-stu-id="41792-1071">General</span></span>

- <span data-ttu-id="41792-1072">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="41792-1072">General Availability of Az Module</span></span>
- <span data-ttu-id="41792-1073">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="41792-1073">Online help for each module</span></span>
- <span data-ttu-id="41792-1074">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="41792-1074">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="41792-1075">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="41792-1075">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="41792-1076">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="41792-1076">Az.Accounts</span></span>
- <span data-ttu-id="41792-1077">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="41792-1077">Changed from Az.Profile</span></span>
- <span data-ttu-id="41792-1078">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="41792-1078">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="41792-1079">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="41792-1079">Az.ApiManagement</span></span>
- <span data-ttu-id="41792-1080">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="41792-1080">Fixes for #7002</span></span>
- <span data-ttu-id="41792-1081">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="41792-1081">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="41792-1082">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="41792-1082">Az.Batch</span></span>
- <span data-ttu-id="41792-1083">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="41792-1083">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="41792-1084">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="41792-1084">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="41792-1085">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="41792-1085">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="41792-1086">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="41792-1086">Az.Billing</span></span>
- <span data-ttu-id="41792-1087">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="41792-1087">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="41792-1088">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="41792-1088">Az.CognitivServices</span></span>
- <span data-ttu-id="41792-1089">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="41792-1089">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="41792-1090">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="41792-1090">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="41792-1091">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="41792-1091">Az.ContainerInstance</span></span>
- <span data-ttu-id="41792-1092">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="41792-1092">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="41792-1093">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="41792-1093">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="41792-1094">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="41792-1094">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="41792-1095">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="41792-1095">Az.DataLakeStore</span></span>
- <span data-ttu-id="41792-1096">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="41792-1096">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="41792-1097">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="41792-1097">Az.Monitor</span></span>
- <span data-ttu-id="41792-1098">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="41792-1098">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="41792-1099">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="41792-1099">Az.KeyVault</span></span>
- <span data-ttu-id="41792-1100">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="41792-1100">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="41792-1101">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="41792-1101">Az.MachineLearning</span></span>
- <span data-ttu-id="41792-1102">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="41792-1102">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="41792-1103">Az.Media</span><span class="sxs-lookup"><span data-stu-id="41792-1103">Az.Media</span></span>
- <span data-ttu-id="41792-1104">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="41792-1104">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="41792-1105">Az.Network</span><span class="sxs-lookup"><span data-stu-id="41792-1105">Az.Network</span></span>
<span data-ttu-id="41792-1106">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="41792-1106">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="41792-1107">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="41792-1107">New cmdlets added:</span></span>
        - <span data-ttu-id="41792-1108">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="41792-1108">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="41792-1109">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="41792-1109">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="41792-1110">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="41792-1110">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="41792-1111">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="41792-1111">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="41792-1112">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="41792-1112">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="41792-1113">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="41792-1113">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="41792-1114">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="41792-1114">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="41792-1115">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="41792-1115">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="41792-1116">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="41792-1116">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="41792-1117">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="41792-1117">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="41792-1118">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="41792-1118">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="41792-1119">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="41792-1119">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="41792-1120">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="41792-1120">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="41792-1121">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="41792-1121">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="41792-1122">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="41792-1122">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="41792-1123">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="41792-1123">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="41792-1124">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="41792-1124">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="41792-1125">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="41792-1125">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="41792-1126">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="41792-1126">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="41792-1127">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="41792-1127">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="41792-1128">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="41792-1128">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="41792-1129">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="41792-1129">Az.OperationalInsights</span></span>
- <span data-ttu-id="41792-1130">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="41792-1130">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="41792-1131">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="41792-1131">Az.Profile</span></span>
- <span data-ttu-id="41792-1132">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="41792-1132">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="41792-1133">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="41792-1133">Az.RecoveryServices</span></span>
- <span data-ttu-id="41792-1134">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="41792-1134">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="41792-1135">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="41792-1135">Az.Resources</span></span>
- <span data-ttu-id="41792-1136">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="41792-1136">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="41792-1137">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="41792-1137">Az.ServiceFabric</span></span>
- <span data-ttu-id="41792-1138">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="41792-1138">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="41792-1139">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="41792-1139">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="41792-1140">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="41792-1140">Az.SIgnalR</span></span>
- <span data-ttu-id="41792-1141">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="41792-1141">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="41792-1142">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="41792-1142">Az.Sql</span></span>
- <span data-ttu-id="41792-1143">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="41792-1143">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="41792-1144">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="41792-1144">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="41792-1145">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="41792-1145">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="41792-1146">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="41792-1146">Az.Storage</span></span>
- <span data-ttu-id="41792-1147">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="41792-1147">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="41792-1148">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="41792-1148">Az.Websites</span></span>
- <span data-ttu-id="41792-1149">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="41792-1149">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="41792-1150">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="41792-1150">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="41792-1151">Geral</span><span class="sxs-lookup"><span data-stu-id="41792-1151">General</span></span>

* <span data-ttu-id="41792-1152">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="41792-1152">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="41792-1153">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="41792-1153">Az.Compute</span></span>

* <span data-ttu-id="41792-1154">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="41792-1154">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="41792-1155">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="41792-1155">Az.DataLakeStore</span></span>

* <span data-ttu-id="41792-1156">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="41792-1156">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="41792-1157">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="41792-1157">Az.FrontDoor</span></span>

* <span data-ttu-id="41792-1158">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="41792-1158">Fixed some broken links</span></span>
    - <span data-ttu-id="41792-1159">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="41792-1159">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="41792-1160">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="41792-1160">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="41792-1161">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="41792-1161">Az.RecoveryServices</span></span>

* <span data-ttu-id="41792-1162">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="41792-1162">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="41792-1163">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="41792-1163">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="41792-1164">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="41792-1164">Az.Resources</span></span>

* <span data-ttu-id="41792-1165">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="41792-1165">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="41792-1166">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="41792-1166">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="41792-1167">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="41792-1167">Az.Sql</span></span>

* <span data-ttu-id="41792-1168">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="41792-1168">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="41792-1169">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="41792-1169">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="41792-1170">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="41792-1170">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="41792-1171">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="41792-1171">Az.Storage</span></span>

* <span data-ttu-id="41792-1172">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="41792-1172">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="41792-1173">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="41792-1173">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="41792-1174">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="41792-1174">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="41792-1175">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="41792-1175">Support Static Website configuration</span></span>
    - <span data-ttu-id="41792-1176">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="41792-1176">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="41792-1177">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="41792-1177">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="41792-1178">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="41792-1178">Az.Websites</span></span>

* <span data-ttu-id="41792-1179">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="41792-1179">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="41792-1180">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="41792-1180">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="41792-1181">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="41792-1181">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="41792-1182">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="41792-1182">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="41792-1183">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="41792-1183">Az.ApiManagement</span></span>
* <span data-ttu-id="41792-1184">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="41792-1184">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="41792-1185">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="41792-1185">Az.Automation</span></span>
* <span data-ttu-id="41792-1186">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="41792-1186">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="41792-1187">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="41792-1187">Added Update Management cmdlets</span></span>
* <span data-ttu-id="41792-1188">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="41792-1188">Added Source Control cmdlets</span></span>
* <span data-ttu-id="41792-1189">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="41792-1189">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="41792-1190">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="41792-1190">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="41792-1191">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="41792-1191">Az.Compute</span></span>
* <span data-ttu-id="41792-1192">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="41792-1192">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="41792-1193">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="41792-1193">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="41792-1194">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="41792-1194">Az.ContainerInstance</span></span>
* <span data-ttu-id="41792-1195">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="41792-1195">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="41792-1196">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="41792-1196">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="41792-1197">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="41792-1197">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="41792-1198">Az.Network</span><span class="sxs-lookup"><span data-stu-id="41792-1198">Az.Network</span></span>
* <span data-ttu-id="41792-1199">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="41792-1199">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="41792-1200">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="41792-1200">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="41792-1201">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="41792-1201">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="41792-1202">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="41792-1202">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="41792-1203">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="41792-1203">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="41792-1204">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="41792-1204">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="41792-1205">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="41792-1205">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="41792-1206">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="41792-1206">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="41792-1207">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="41792-1207">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="41792-1208">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="41792-1208">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="41792-1209">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="41792-1209">Az.Relay</span></span>
* <span data-ttu-id="41792-1210">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="41792-1210">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="41792-1211">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="41792-1211">Az.Resources</span></span>
* <span data-ttu-id="41792-1212">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="41792-1212">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="41792-1213">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="41792-1213">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="41792-1214">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="41792-1214">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="41792-1215">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="41792-1215">Az.ServiceFabric</span></span>
* <span data-ttu-id="41792-1216">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="41792-1216">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="41792-1217">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="41792-1217">Az.Sql</span></span>
* <span data-ttu-id="41792-1218">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="41792-1218">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="41792-1219">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="41792-1219">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="41792-1220">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="41792-1220">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="41792-1221">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="41792-1221">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="41792-1222">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="41792-1222">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="41792-1223">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="41792-1223">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="41792-1224">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="41792-1224">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="41792-1225">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="41792-1225">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="41792-1226">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="41792-1226">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="41792-1227">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="41792-1227">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="41792-1228">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="41792-1228">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="41792-1229">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="41792-1229">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="41792-1230">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="41792-1230">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="41792-1231">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="41792-1231">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="41792-1232">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="41792-1232">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="41792-1233">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="41792-1233">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="41792-1234">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="41792-1234">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="41792-1235">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="41792-1235">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="41792-1236">Geral</span><span class="sxs-lookup"><span data-stu-id="41792-1236">General</span></span>
* <span data-ttu-id="41792-1237">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="41792-1237">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="41792-1238">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="41792-1238">Az.Profile</span></span>
* <span data-ttu-id="41792-1239">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="41792-1239">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="41792-1240">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="41792-1240">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="41792-1241">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="41792-1241">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="41792-1242">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="41792-1242">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="41792-1243">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="41792-1243">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="41792-1244">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="41792-1244">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="41792-1245">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="41792-1245">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="41792-1246">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="41792-1246">Az.CognitiveServices</span></span>
* <span data-ttu-id="41792-1247">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="41792-1247">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="41792-1248">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="41792-1248">Az.Compute</span></span>
* <span data-ttu-id="41792-1249">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="41792-1249">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="41792-1250">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="41792-1250">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="41792-1251">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="41792-1251">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="41792-1252">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="41792-1252">Az.DataLakeStore</span></span>
* <span data-ttu-id="41792-1253">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="41792-1253">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="41792-1254">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="41792-1254">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="41792-1255">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="41792-1255">Az.Insights</span></span>
* <span data-ttu-id="41792-1256">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="41792-1256">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="41792-1257">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="41792-1257">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="41792-1258">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="41792-1258">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="41792-1259">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="41792-1259">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="41792-1260">Az.Network</span><span class="sxs-lookup"><span data-stu-id="41792-1260">Az.Network</span></span>
* <span data-ttu-id="41792-1261">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="41792-1261">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="41792-1262">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="41792-1262">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="41792-1263">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="41792-1263">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="41792-1264">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="41792-1264">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="41792-1265">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="41792-1265">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="41792-1266">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="41792-1266">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="41792-1267">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="41792-1267">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="41792-1268">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="41792-1268">Az.PolicyInsights</span></span>
* <span data-ttu-id="41792-1269">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="41792-1269">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="41792-1270">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="41792-1270">Az.Resources</span></span>
* <span data-ttu-id="41792-1271">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="41792-1271">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="41792-1272">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="41792-1272">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="41792-1273">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="41792-1273">Az.ServiceBus</span></span>
* <span data-ttu-id="41792-1274">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="41792-1274">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="41792-1275">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="41792-1275">Az.ServiceFabric</span></span>
* <span data-ttu-id="41792-1276">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="41792-1276">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="41792-1277">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="41792-1277">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="41792-1278">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="41792-1278">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="41792-1279">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="41792-1279">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="41792-1280">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="41792-1280">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="41792-1281">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="41792-1281">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="41792-1282">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="41792-1282">Az.Profile</span></span>
* <span data-ttu-id="41792-1283">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="41792-1283">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="41792-1284">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="41792-1284">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="41792-1285">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="41792-1285">Az.Compute</span></span>
* <span data-ttu-id="41792-1286">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="41792-1286">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="41792-1287">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="41792-1287">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="41792-1288">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="41792-1288">Az.DataLakeStore</span></span>
* <span data-ttu-id="41792-1289">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="41792-1289">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="41792-1290">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="41792-1290">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="41792-1291">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="41792-1291">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="41792-1292">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="41792-1292">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="41792-1293">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="41792-1293">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="41792-1294">Az.Network</span><span class="sxs-lookup"><span data-stu-id="41792-1294">Az.Network</span></span>
* <span data-ttu-id="41792-1295">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="41792-1295">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="41792-1296">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="41792-1296">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="41792-1297">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="41792-1297">Az.Resources</span></span>
* <span data-ttu-id="41792-1298">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="41792-1298">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="41792-1299">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="41792-1299">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="41792-1300">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="41792-1300">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="41792-1301">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="41792-1301">Azure.Storage</span></span>
* <span data-ttu-id="41792-1302">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="41792-1302">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="41792-1303">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="41792-1303">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="41792-1304">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="41792-1304">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="41792-1305">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="41792-1305">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="41792-1306">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="41792-1306">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="41792-1307">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="41792-1307">Az.CognitiveServices</span></span>
* <span data-ttu-id="41792-1308">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="41792-1308">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="41792-1309">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="41792-1309">Az.Compute</span></span>
* <span data-ttu-id="41792-1310">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="41792-1310">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="41792-1311">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="41792-1311">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="41792-1312">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="41792-1312">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="41792-1313">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="41792-1313">Az.DataFactoryV2</span></span>
* <span data-ttu-id="41792-1314">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="41792-1314">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="41792-1315">Az.Network</span><span class="sxs-lookup"><span data-stu-id="41792-1315">Az.Network</span></span>
* <span data-ttu-id="41792-1316">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="41792-1316">Added NetworkProfile functionality.</span></span> <span data-ttu-id="41792-1317">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="41792-1317">new cmdlets added</span></span>
    - <span data-ttu-id="41792-1318">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="41792-1318">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="41792-1319">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="41792-1319">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="41792-1320">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="41792-1320">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="41792-1321">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="41792-1321">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="41792-1322">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="41792-1322">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="41792-1323">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="41792-1323">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="41792-1324">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="41792-1324">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="41792-1325">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="41792-1325">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="41792-1326">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="41792-1326">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="41792-1327">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="41792-1327">Az.RedisCache</span></span>
* <span data-ttu-id="41792-1328">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="41792-1328">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="41792-1329">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="41792-1329">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="41792-1330">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="41792-1330">Az.Resources</span></span>
* <span data-ttu-id="41792-1331">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="41792-1331">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="41792-1332">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="41792-1332">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="41792-1333">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="41792-1333">Az.Sql</span></span>
* <span data-ttu-id="41792-1334">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="41792-1334">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="41792-1335">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="41792-1335">Az.Websites</span></span>
* <span data-ttu-id="41792-1336">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="41792-1336">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="41792-1337">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="41792-1337">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="41792-1338">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="41792-1338">0.2.0 - September 2018</span></span>
 <span data-ttu-id="41792-1339">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="41792-1339">Initial Release</span></span>