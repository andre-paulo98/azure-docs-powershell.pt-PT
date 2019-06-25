---
ms.openlocfilehash: 10d8d50131b3c55ae19c5142c42cb47f37c68c92
ms.sourcegitcommit: 5bdedc77b27b66998387486761ec67ed9326f169
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/24/2019
ms.locfileid: "67345222"
---
## <a name="180---april-2019"></a><span data-ttu-id="aafd8-101">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="aafd8-101">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="aafd8-102">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="aafd8-102">Highlights since the last major release</span></span>
* <span data-ttu-id="aafd8-103">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="aafd8-103">General availability of `Az` module</span></span>
* <span data-ttu-id="aafd8-104">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="aafd8-104">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="aafd8-105">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="aafd8-105">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="aafd8-106">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="aafd8-106">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="aafd8-107">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="aafd8-107">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="aafd8-108">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="aafd8-108">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="aafd8-109">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="aafd8-109">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="aafd8-110">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aafd8-110">Az.Accounts</span></span>
* <span data-ttu-id="aafd8-111">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="aafd8-111">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="aafd8-112">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="aafd8-112">Az.Batch</span></span>
* <span data-ttu-id="aafd8-113">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="aafd8-113">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="aafd8-114">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="aafd8-114">Az.Cdn</span></span>
* <span data-ttu-id="aafd8-115">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="aafd8-115">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="aafd8-116">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="aafd8-116">Az.CognitiveServices</span></span>
* <span data-ttu-id="aafd8-117">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="aafd8-117">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aafd8-118">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aafd8-118">Az.Compute</span></span>
* <span data-ttu-id="aafd8-119">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="aafd8-119">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="aafd8-120">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="aafd8-120">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="aafd8-121">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="aafd8-121">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="aafd8-122">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="aafd8-122">Az.DataFactory</span></span>
* <span data-ttu-id="aafd8-123">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="aafd8-123">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="aafd8-124">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="aafd8-124">Az.DataLakeStore</span></span>
* <span data-ttu-id="aafd8-125">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="aafd8-125">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="aafd8-126">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="aafd8-126">Az.EventGrid</span></span>
* <span data-ttu-id="aafd8-127">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="aafd8-127">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="aafd8-128">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="aafd8-128">Az.EventHub</span></span>
* <span data-ttu-id="aafd8-129">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="aafd8-129">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="aafd8-130">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="aafd8-130">Az.HDInsight</span></span>
* <span data-ttu-id="aafd8-131">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="aafd8-131">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="aafd8-132">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="aafd8-132">Az.IotHub</span></span>
* <span data-ttu-id="aafd8-133">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="aafd8-133">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="aafd8-134">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="aafd8-134">Az.KeyVault</span></span>
* <span data-ttu-id="aafd8-135">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="aafd8-135">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="aafd8-136">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="aafd8-136">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="aafd8-137">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="aafd8-137">Az.MachineLearning</span></span>
* <span data-ttu-id="aafd8-138">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="aafd8-138">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="aafd8-139">Az.Media</span><span class="sxs-lookup"><span data-stu-id="aafd8-139">Az.Media</span></span>
* <span data-ttu-id="aafd8-140">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="aafd8-140">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="aafd8-141">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="aafd8-141">Az.Monitor</span></span>
  * <span data-ttu-id="aafd8-142">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="aafd8-142">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="aafd8-143">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="aafd8-143">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="aafd8-144">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="aafd8-144">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="aafd8-145">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="aafd8-145">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="aafd8-146">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="aafd8-146">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="aafd8-147">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="aafd8-147">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="aafd8-148">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="aafd8-148">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aafd8-149">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aafd8-149">Az.Network</span></span>
* <span data-ttu-id="aafd8-150">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="aafd8-150">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="aafd8-151">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="aafd8-151">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="aafd8-152">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="aafd8-152">Az.NotificationHubs</span></span>
* <span data-ttu-id="aafd8-153">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="aafd8-153">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="aafd8-154">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="aafd8-154">Az.OperationalInsights</span></span>
* <span data-ttu-id="aafd8-155">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="aafd8-155">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="aafd8-156">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="aafd8-156">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="aafd8-157">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="aafd8-157">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="aafd8-158">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="aafd8-158">Az.RecoveryServices</span></span>
* <span data-ttu-id="aafd8-159">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="aafd8-159">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="aafd8-160">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="aafd8-160">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="aafd8-161">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="aafd8-161">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="aafd8-162">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="aafd8-162">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="aafd8-163">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="aafd8-163">Az.RedisCache</span></span>
* <span data-ttu-id="aafd8-164">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="aafd8-164">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="aafd8-165">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aafd8-165">Az.Resources</span></span>
* <span data-ttu-id="aafd8-166">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="aafd8-166">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="aafd8-167">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aafd8-167">Az.Sql</span></span>
* <span data-ttu-id="aafd8-168">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="aafd8-168">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="aafd8-169">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="aafd8-169">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="aafd8-170">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="aafd8-170">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="aafd8-171">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="aafd8-171">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="aafd8-172">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="aafd8-172">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="aafd8-173">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="aafd8-173">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="aafd8-174">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="aafd8-174">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="aafd8-175">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aafd8-175">Az.Websites</span></span>
* <span data-ttu-id="aafd8-176">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="aafd8-176">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="aafd8-177">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="aafd8-177">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="aafd8-178">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="aafd8-178">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="aafd8-179">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="aafd8-179">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="aafd8-180">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="aafd8-180">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="aafd8-181">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="aafd8-181">Highlights since the last major release</span></span>
* <span data-ttu-id="aafd8-182">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="aafd8-182">General availability of `Az` module</span></span>
* <span data-ttu-id="aafd8-183">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="aafd8-183">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="aafd8-184">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="aafd8-184">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="aafd8-185">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="aafd8-185">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="aafd8-186">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="aafd8-186">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="aafd8-187">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="aafd8-187">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="aafd8-188">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="aafd8-188">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="aafd8-189">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aafd8-189">Az.Accounts</span></span>
* <span data-ttu-id="aafd8-190">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="aafd8-190">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="aafd8-191">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="aafd8-191">Az.AnalysisServices</span></span>
* <span data-ttu-id="aafd8-192">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="aafd8-192">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="aafd8-193">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="aafd8-193">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="aafd8-194">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="aafd8-194">Az.Automation</span></span>
* <span data-ttu-id="aafd8-195">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="aafd8-195">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="aafd8-196">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="aafd8-196">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="aafd8-197">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="aafd8-197">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aafd8-198">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aafd8-198">Az.Compute</span></span>
* <span data-ttu-id="aafd8-199">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="aafd8-199">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="aafd8-200">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="aafd8-200">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="aafd8-201">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="aafd8-201">Az.ContainerInstance</span></span>
* <span data-ttu-id="aafd8-202">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="aafd8-202">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="aafd8-203">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="aafd8-203">Az.DataFactory</span></span>
* <span data-ttu-id="aafd8-204">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="aafd8-204">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="aafd8-205">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="aafd8-205">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="aafd8-206">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aafd8-206">Az.Resources</span></span>
* <span data-ttu-id="aafd8-207">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="aafd8-207">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="aafd8-208">Melhor processamento de erros de "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="aafd8-208">Improve error handling for for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="aafd8-209">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="aafd8-209">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="aafd8-210">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="aafd8-210">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="aafd8-211">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="aafd8-211">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="aafd8-212">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="aafd8-212">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="aafd8-213">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aafd8-213">Az.Sql</span></span>
* <span data-ttu-id="aafd8-214">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="aafd8-214">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="aafd8-215">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aafd8-215">Az.Storage</span></span>
* <span data-ttu-id="aafd8-216">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="aafd8-216">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="aafd8-217">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="aafd8-217">New-AzStorageContext</span></span>
* <span data-ttu-id="aafd8-218">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="aafd8-218">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="aafd8-219">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="aafd8-219">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="aafd8-220">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="aafd8-220">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="aafd8-221">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="aafd8-221">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="aafd8-222">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="aafd8-222">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="aafd8-223">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="aafd8-223">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="aafd8-224">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="aafd8-224">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="aafd8-225">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="aafd8-225">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="aafd8-226">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="aafd8-226">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="aafd8-227">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="aafd8-227">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="aafd8-228">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="aafd8-228">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="aafd8-229">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="aafd8-229">Highlights since the last major release</span></span>
* <span data-ttu-id="aafd8-230">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="aafd8-230">General availability of `Az` module</span></span>
* <span data-ttu-id="aafd8-231">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="aafd8-231">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="aafd8-232">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="aafd8-232">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="aafd8-233">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="aafd8-233">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="aafd8-234">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="aafd8-234">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="aafd8-235">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="aafd8-235">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="aafd8-236">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="aafd8-236">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="aafd8-237">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="aafd8-237">Az.Automation</span></span>
* <span data-ttu-id="aafd8-238">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="aafd8-238">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="aafd8-239">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="aafd8-239">Dynamic grouping</span></span>
    * <span data-ttu-id="aafd8-240">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="aafd8-240">Pre-Post script</span></span>
    * <span data-ttu-id="aafd8-241">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="aafd8-241">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aafd8-242">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aafd8-242">Az.Compute</span></span>
* <span data-ttu-id="aafd8-243">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="aafd8-243">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="aafd8-244">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="aafd8-244">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="aafd8-245">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="aafd8-245">Az.KeyVault</span></span>
* <span data-ttu-id="aafd8-246">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="aafd8-246">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aafd8-247">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aafd8-247">Az.Network</span></span>
* <span data-ttu-id="aafd8-248">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="aafd8-248">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="aafd8-249">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="aafd8-249">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="aafd8-250">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="aafd8-250">Az.RecoveryServices</span></span>
* <span data-ttu-id="aafd8-251">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="aafd8-251">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="aafd8-252">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="aafd8-252">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="aafd8-253">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aafd8-253">Az.Resources</span></span>
* <span data-ttu-id="aafd8-254">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="aafd8-254">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="aafd8-255">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="aafd8-255">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="aafd8-256">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aafd8-256">Az.Sql</span></span>
* <span data-ttu-id="aafd8-257">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="aafd8-257">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="aafd8-258">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aafd8-258">Az.Storage</span></span>
* <span data-ttu-id="aafd8-259">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aafd8-259">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="aafd8-260">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="aafd8-260">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="aafd8-261">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="aafd8-261">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="aafd8-262">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="aafd8-262">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="aafd8-263">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="aafd8-263">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="aafd8-264">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="aafd8-264">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="aafd8-265">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="aafd8-265">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="aafd8-266">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aafd8-266">Az.Websites</span></span>
* <span data-ttu-id="aafd8-267">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="aafd8-267">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="aafd8-268">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="aafd8-268">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="aafd8-269">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aafd8-269">Az.Accounts</span></span>
* <span data-ttu-id="aafd8-270">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="aafd8-270">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="aafd8-271">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="aafd8-271">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="aafd8-272">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="aafd8-272">Az.Automation</span></span>
* <span data-ttu-id="aafd8-273">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="aafd8-273">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="aafd8-274">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="aafd8-274">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="aafd8-275">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="aafd8-275">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="aafd8-276">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="aafd8-276">Az.Cdn</span></span>
* <span data-ttu-id="aafd8-277">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="aafd8-277">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aafd8-278">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aafd8-278">Az.Compute</span></span>
* <span data-ttu-id="aafd8-279">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="aafd8-279">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="aafd8-280">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="aafd8-280">Az.DataFactory</span></span>
* <span data-ttu-id="aafd8-281">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="aafd8-281">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="aafd8-282">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="aafd8-282">Az.LogicApp</span></span>
* <span data-ttu-id="aafd8-283">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="aafd8-283">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aafd8-284">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aafd8-284">Az.Network</span></span>
* <span data-ttu-id="aafd8-285">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="aafd8-285">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="aafd8-286">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="aafd8-286">Az.RecoveryServices</span></span>
* <span data-ttu-id="aafd8-287">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="aafd8-287">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="aafd8-288">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="aafd8-288">SDK Update</span></span>
* <span data-ttu-id="aafd8-289">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="aafd8-289">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="aafd8-290">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="aafd8-290">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="aafd8-291">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aafd8-291">Az.Resources</span></span>
* <span data-ttu-id="aafd8-292">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="aafd8-292">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="aafd8-293">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="aafd8-293">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="aafd8-294">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="aafd8-294">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="aafd8-295">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="aafd8-295">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="aafd8-296">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="aafd8-296">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="aafd8-297">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="aafd8-297">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="aafd8-298">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aafd8-298">Az.Sql</span></span>
* <span data-ttu-id="aafd8-299">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="aafd8-299">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="aafd8-300">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="aafd8-300">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="aafd8-301">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aafd8-301">Az.Storage</span></span>
* <span data-ttu-id="aafd8-302">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="aafd8-302">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="aafd8-303">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="aafd8-303">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="aafd8-304">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="aafd8-304">Az.AnalysisServices</span></span>
* <span data-ttu-id="aafd8-305">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="aafd8-305">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="aafd8-306">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="aafd8-306">Az.Automation</span></span>
* <span data-ttu-id="aafd8-307">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="aafd8-307">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="aafd8-308">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="aafd8-308">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="aafd8-309">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="aafd8-309">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="aafd8-310">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="aafd8-310">Az.CognitiveServices</span></span>
* <span data-ttu-id="aafd8-311">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="aafd8-311">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aafd8-312">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aafd8-312">Az.Compute</span></span>
* <span data-ttu-id="aafd8-313">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="aafd8-313">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="aafd8-314">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="aafd8-314">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="aafd8-315">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="aafd8-315">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="aafd8-316">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="aafd8-316">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="aafd8-317">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="aafd8-317">Az.DataLakeStore</span></span>
* <span data-ttu-id="aafd8-318">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="aafd8-318">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="aafd8-319">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="aafd8-319">Az.EventHub</span></span>
* <span data-ttu-id="aafd8-320">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="aafd8-320">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="aafd8-321">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="aafd8-321">Az.KeyVault</span></span>
* <span data-ttu-id="aafd8-322">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="aafd8-322">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="aafd8-323">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="aafd8-323">Az.LogicApp</span></span>
* <span data-ttu-id="aafd8-324">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="aafd8-324">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="aafd8-325">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="aafd8-325">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="aafd8-326">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="aafd8-326">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="aafd8-327">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="aafd8-327">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="aafd8-328">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="aafd8-328">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="aafd8-329">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="aafd8-329">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="aafd8-330">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="aafd8-330">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="aafd8-331">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="aafd8-331">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="aafd8-332">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="aafd8-332">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="aafd8-333">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="aafd8-333">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="aafd8-334">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="aafd8-334">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="aafd8-335">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="aafd8-335">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="aafd8-336">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="aafd8-336">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="aafd8-337">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="aafd8-337">Az.Monitor</span></span>
* <span data-ttu-id="aafd8-338">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="aafd8-338">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aafd8-339">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aafd8-339">Az.Network</span></span>
* <span data-ttu-id="aafd8-340">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="aafd8-340">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="aafd8-341">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="aafd8-341">Az.OperationalInsights</span></span>
* <span data-ttu-id="aafd8-342">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="aafd8-342">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="aafd8-343">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="aafd8-343">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="aafd8-344">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="aafd8-344">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="aafd8-345">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aafd8-345">Az.Resources</span></span>
* <span data-ttu-id="aafd8-346">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="aafd8-346">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="aafd8-347">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="aafd8-347">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="aafd8-348">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="aafd8-348">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="aafd8-349">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="aafd8-349">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="aafd8-350">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aafd8-350">Az.Sql</span></span>
* <span data-ttu-id="aafd8-351">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="aafd8-351">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="aafd8-352">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="aafd8-352">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="aafd8-353">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aafd8-353">Az.Websites</span></span>
* <span data-ttu-id="aafd8-354">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="aafd8-354">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="aafd8-355">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="aafd8-355">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="aafd8-356">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aafd8-356">Az.Accounts</span></span>
* <span data-ttu-id="aafd8-357">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="aafd8-357">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="aafd8-358">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="aafd8-358">Az.AnalysisServices</span></span>
<span data-ttu-id="aafd8-359">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="aafd8-359">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aafd8-360">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aafd8-360">Az.Compute</span></span>
* <span data-ttu-id="aafd8-361">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="aafd8-361">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="aafd8-362">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="aafd8-362">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="aafd8-363">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="aafd8-363">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="aafd8-364">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="aafd8-364">Az.RecoveryServices</span></span>
<span data-ttu-id="aafd8-365">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="aafd8-365">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="aafd8-366">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aafd8-366">Az.Resources</span></span>
* <span data-ttu-id="aafd8-367">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="aafd8-367">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="aafd8-368">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="aafd8-368">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="aafd8-369">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="aafd8-369">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="aafd8-370">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="aafd8-370">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="aafd8-371">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aafd8-371">Az.Sql</span></span>
* <span data-ttu-id="aafd8-372">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="aafd8-372">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="aafd8-373">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="aafd8-373">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="aafd8-374">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="aafd8-374">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="aafd8-375">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="aafd8-375">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="aafd8-376">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aafd8-376">Az.Accounts</span></span>
* <span data-ttu-id="aafd8-377">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="aafd8-377">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="aafd8-378">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="aafd8-378">Az.AnalysisServices</span></span>
* <span data-ttu-id="aafd8-379">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="aafd8-379">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="aafd8-380">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="aafd8-380">Az.RecoveryServices</span></span>
* <span data-ttu-id="aafd8-381">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="aafd8-381">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="aafd8-382">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="aafd8-382">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="aafd8-383">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aafd8-383">Az.Accounts</span></span>
* <span data-ttu-id="aafd8-384">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="aafd8-384">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="aafd8-385">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="aafd8-385">Update incorrect online help URLs</span></span>
* <span data-ttu-id="aafd8-386">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="aafd8-386">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="aafd8-387">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="aafd8-387">Az.Aks</span></span>
* <span data-ttu-id="aafd8-388">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="aafd8-388">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="aafd8-389">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="aafd8-389">Az.Automation</span></span>
* <span data-ttu-id="aafd8-390">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="aafd8-390">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="aafd8-391">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="aafd8-391">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="aafd8-392">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="aafd8-392">Az.Cdn</span></span>
* <span data-ttu-id="aafd8-393">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="aafd8-393">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aafd8-394">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aafd8-394">Az.Compute</span></span>
* <span data-ttu-id="aafd8-395">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="aafd8-395">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="aafd8-396">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="aafd8-396">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="aafd8-397">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="aafd8-397">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="aafd8-398">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="aafd8-398">Az.ContainerRegistry</span></span>
* <span data-ttu-id="aafd8-399">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="aafd8-399">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="aafd8-400">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="aafd8-400">Az.DataFactory</span></span>
* <span data-ttu-id="aafd8-401">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="aafd8-401">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="aafd8-402">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="aafd8-402">Az.DataLakeStore</span></span>
* <span data-ttu-id="aafd8-403">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="aafd8-403">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="aafd8-404">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="aafd8-404">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="aafd8-405">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="aafd8-405">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="aafd8-406">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="aafd8-406">Az.IotHub</span></span>
* <span data-ttu-id="aafd8-407">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="aafd8-407">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="aafd8-408">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="aafd8-408">Az.KeyVault</span></span>
* <span data-ttu-id="aafd8-409">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="aafd8-409">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aafd8-410">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aafd8-410">Az.Network</span></span>
* <span data-ttu-id="aafd8-411">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="aafd8-411">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="aafd8-412">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aafd8-412">Az.Resources</span></span>
* <span data-ttu-id="aafd8-413">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="aafd8-413">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="aafd8-414">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="aafd8-414">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="aafd8-415">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="aafd8-415">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="aafd8-416">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="aafd8-416">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="aafd8-417">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="aafd8-417">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="aafd8-418">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="aafd8-418">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="aafd8-419">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="aafd8-419">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="aafd8-420">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aafd8-420">Az.ServiceFabric</span></span>
* <span data-ttu-id="aafd8-421">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="aafd8-421">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="aafd8-422">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="aafd8-422">Fix some error messages.</span></span>
* <span data-ttu-id="aafd8-423">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="aafd8-423">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="aafd8-424">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="aafd8-424">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="aafd8-425">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="aafd8-425">Az.SignalR</span></span>
* <span data-ttu-id="aafd8-426">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="aafd8-426">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="aafd8-427">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aafd8-427">Az.Sql</span></span>
* <span data-ttu-id="aafd8-428">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="aafd8-428">Update incorrect online help URLs</span></span>
* <span data-ttu-id="aafd8-429">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="aafd8-429">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="aafd8-430">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="aafd8-430">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="aafd8-431">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="aafd8-431">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="aafd8-432">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aafd8-432">Az.Storage</span></span>
* <span data-ttu-id="aafd8-433">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="aafd8-433">Update incorrect online help URLs</span></span>
* <span data-ttu-id="aafd8-434">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="aafd8-434">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="aafd8-435">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="aafd8-435">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="aafd8-436">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="aafd8-436">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="aafd8-437">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="aafd8-437">Az.TrafficManager</span></span>
* <span data-ttu-id="aafd8-438">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="aafd8-438">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="aafd8-439">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aafd8-439">Az.Websites</span></span>
* <span data-ttu-id="aafd8-440">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="aafd8-440">Update incorrect online help URLs</span></span>
* <span data-ttu-id="aafd8-441">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="aafd8-441">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="aafd8-442">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="aafd8-442">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="aafd8-443">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="aafd8-443">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="aafd8-444">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aafd8-444">Az.Accounts</span></span>
* <span data-ttu-id="aafd8-445">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="aafd8-445">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aafd8-446">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aafd8-446">Az.Compute</span></span>
* <span data-ttu-id="aafd8-447">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="aafd8-447">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="aafd8-448">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="aafd8-448">Updated the description of ID in help files</span></span>
* <span data-ttu-id="aafd8-449">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aafd8-449">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="aafd8-450">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="aafd8-450">Az.DataLakeStore</span></span>
* <span data-ttu-id="aafd8-451">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="aafd8-451">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="aafd8-452">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="aafd8-452">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="aafd8-453">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="aafd8-453">Az.EventGrid</span></span>
* <span data-ttu-id="aafd8-454">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="aafd8-454">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="aafd8-455">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="aafd8-455">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="aafd8-456">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="aafd8-456">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="aafd8-457">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="aafd8-457">Event Time-To-Live,</span></span>
        - <span data-ttu-id="aafd8-458">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="aafd8-458">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="aafd8-459">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="aafd8-459">Dead letter endpoint.</span></span>
    - <span data-ttu-id="aafd8-460">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="aafd8-460">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="aafd8-461">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="aafd8-461">Event Time-To-Live,</span></span>
        - <span data-ttu-id="aafd8-462">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="aafd8-462">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="aafd8-463">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="aafd8-463">Dead letter endpoint.</span></span>
* <span data-ttu-id="aafd8-464">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="aafd8-464">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="aafd8-465">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="aafd8-465">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="aafd8-466">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="aafd8-466">Az.IotHub</span></span>
* <span data-ttu-id="aafd8-467">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="aafd8-467">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="aafd8-468">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="aafd8-468">Az.LogicApp</span></span>
* <span data-ttu-id="aafd8-469">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="aafd8-469">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="aafd8-470">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aafd8-470">Az.Resources</span></span>
* <span data-ttu-id="aafd8-471">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="aafd8-471">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="aafd8-472">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="aafd8-472">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="aafd8-473">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="aafd8-473">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="aafd8-474">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="aafd8-474">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="aafd8-475">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="aafd8-475">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="aafd8-476">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="aafd8-476">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="aafd8-477">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="aafd8-477">Az.SignalR</span></span>
* <span data-ttu-id="aafd8-478">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aafd8-478">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="aafd8-479">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aafd8-479">Az.Sql</span></span>
* <span data-ttu-id="aafd8-480">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="aafd8-480">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="aafd8-481">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aafd8-481">Az.Storage</span></span>
* <span data-ttu-id="aafd8-482">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="aafd8-482">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="aafd8-483">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="aafd8-483">New-AzStorageContext</span></span>
* <span data-ttu-id="aafd8-484">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="aafd8-484">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="aafd8-485">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="aafd8-485">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="aafd8-486">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aafd8-486">Az.Websites</span></span>
* <span data-ttu-id="aafd8-487">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="aafd8-487">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="aafd8-488">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aafd8-488">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="aafd8-489">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="aafd8-489">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="aafd8-490">Geral</span><span class="sxs-lookup"><span data-stu-id="aafd8-490">General</span></span>

- <span data-ttu-id="aafd8-491">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="aafd8-491">General Availability of Az Module</span></span>
- <span data-ttu-id="aafd8-492">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="aafd8-492">Online help for each module</span></span>
- <span data-ttu-id="aafd8-493">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="aafd8-493">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="aafd8-494">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="aafd8-494">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="aafd8-495">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aafd8-495">Az.Accounts</span></span>
- <span data-ttu-id="aafd8-496">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="aafd8-496">Changed from Az.Profile</span></span>
- <span data-ttu-id="aafd8-497">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="aafd8-497">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="aafd8-498">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="aafd8-498">Az.ApiManagement</span></span>
- <span data-ttu-id="aafd8-499">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="aafd8-499">Fixes for #7002</span></span>
- <span data-ttu-id="aafd8-500">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="aafd8-500">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="aafd8-501">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="aafd8-501">Az.Batch</span></span>
- <span data-ttu-id="aafd8-502">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="aafd8-502">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="aafd8-503">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="aafd8-503">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="aafd8-504">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="aafd8-504">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="aafd8-505">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="aafd8-505">Az.Billing</span></span>
- <span data-ttu-id="aafd8-506">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="aafd8-506">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="aafd8-507">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="aafd8-507">Az.CognitivServices</span></span>
- <span data-ttu-id="aafd8-508">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="aafd8-508">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="aafd8-509">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="aafd8-509">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="aafd8-510">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="aafd8-510">Az.ContainerInstance</span></span>
- <span data-ttu-id="aafd8-511">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="aafd8-511">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="aafd8-512">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="aafd8-512">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="aafd8-513">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="aafd8-513">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="aafd8-514">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="aafd8-514">Az.DataLakeStore</span></span>
- <span data-ttu-id="aafd8-515">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="aafd8-515">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="aafd8-516">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="aafd8-516">Az.Monitor</span></span>
- <span data-ttu-id="aafd8-517">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="aafd8-517">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="aafd8-518">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="aafd8-518">Az.KeyVault</span></span>
- <span data-ttu-id="aafd8-519">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="aafd8-519">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="aafd8-520">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="aafd8-520">Az.MachineLearning</span></span>
- <span data-ttu-id="aafd8-521">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="aafd8-521">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="aafd8-522">Az.Media</span><span class="sxs-lookup"><span data-stu-id="aafd8-522">Az.Media</span></span>
- <span data-ttu-id="aafd8-523">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="aafd8-523">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="aafd8-524">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aafd8-524">Az.Network</span></span>
<span data-ttu-id="aafd8-525">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="aafd8-525">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="aafd8-526">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="aafd8-526">New cmdlets added:</span></span>
        - <span data-ttu-id="aafd8-527">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="aafd8-527">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="aafd8-528">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="aafd8-528">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="aafd8-529">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="aafd8-529">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="aafd8-530">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="aafd8-530">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="aafd8-531">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="aafd8-531">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="aafd8-532">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="aafd8-532">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="aafd8-533">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="aafd8-533">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="aafd8-534">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="aafd8-534">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="aafd8-535">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="aafd8-535">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="aafd8-536">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="aafd8-536">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="aafd8-537">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="aafd8-537">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="aafd8-538">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="aafd8-538">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="aafd8-539">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="aafd8-539">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="aafd8-540">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="aafd8-540">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="aafd8-541">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="aafd8-541">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="aafd8-542">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="aafd8-542">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="aafd8-543">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="aafd8-543">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="aafd8-544">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="aafd8-544">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="aafd8-545">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="aafd8-545">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="aafd8-546">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="aafd8-546">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="aafd8-547">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="aafd8-547">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="aafd8-548">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="aafd8-548">Az.OperationalInsights</span></span>
- <span data-ttu-id="aafd8-549">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="aafd8-549">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="aafd8-550">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="aafd8-550">Az.Profile</span></span>
- <span data-ttu-id="aafd8-551">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aafd8-551">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="aafd8-552">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="aafd8-552">Az.RecoveryServices</span></span>
- <span data-ttu-id="aafd8-553">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="aafd8-553">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="aafd8-554">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aafd8-554">Az.Resources</span></span>
- <span data-ttu-id="aafd8-555">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="aafd8-555">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="aafd8-556">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aafd8-556">Az.ServiceFabric</span></span>
- <span data-ttu-id="aafd8-557">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="aafd8-557">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="aafd8-558">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="aafd8-558">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="aafd8-559">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="aafd8-559">Az.SIgnalR</span></span>
- <span data-ttu-id="aafd8-560">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="aafd8-560">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="aafd8-561">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aafd8-561">Az.Sql</span></span>
- <span data-ttu-id="aafd8-562">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="aafd8-562">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="aafd8-563">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="aafd8-563">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="aafd8-564">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="aafd8-564">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="aafd8-565">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aafd8-565">Az.Storage</span></span>
- <span data-ttu-id="aafd8-566">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="aafd8-566">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="aafd8-567">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aafd8-567">Az.Websites</span></span>
- <span data-ttu-id="aafd8-568">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="aafd8-568">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="aafd8-569">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="aafd8-569">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="aafd8-570">Geral</span><span class="sxs-lookup"><span data-stu-id="aafd8-570">General</span></span>

* <span data-ttu-id="aafd8-571">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="aafd8-571">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="aafd8-572">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aafd8-572">Az.Compute</span></span>

* <span data-ttu-id="aafd8-573">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="aafd8-573">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="aafd8-574">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="aafd8-574">Az.DataLakeStore</span></span>

* <span data-ttu-id="aafd8-575">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="aafd8-575">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="aafd8-576">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="aafd8-576">Az.FrontDoor</span></span>

* <span data-ttu-id="aafd8-577">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="aafd8-577">Fixed some broken links</span></span>
    - <span data-ttu-id="aafd8-578">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="aafd8-578">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="aafd8-579">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="aafd8-579">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="aafd8-580">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="aafd8-580">Az.RecoveryServices</span></span>

* <span data-ttu-id="aafd8-581">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="aafd8-581">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="aafd8-582">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="aafd8-582">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="aafd8-583">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aafd8-583">Az.Resources</span></span>

* <span data-ttu-id="aafd8-584">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="aafd8-584">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="aafd8-585">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="aafd8-585">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="aafd8-586">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aafd8-586">Az.Sql</span></span>

* <span data-ttu-id="aafd8-587">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="aafd8-587">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="aafd8-588">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="aafd8-588">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="aafd8-589">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="aafd8-589">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="aafd8-590">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aafd8-590">Az.Storage</span></span>

* <span data-ttu-id="aafd8-591">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="aafd8-591">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="aafd8-592">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="aafd8-592">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="aafd8-593">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="aafd8-593">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="aafd8-594">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="aafd8-594">Support Static Website configuration</span></span>
    - <span data-ttu-id="aafd8-595">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="aafd8-595">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="aafd8-596">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="aafd8-596">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="aafd8-597">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aafd8-597">Az.Websites</span></span>

* <span data-ttu-id="aafd8-598">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="aafd8-598">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="aafd8-599">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="aafd8-599">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="aafd8-600">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="aafd8-600">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="aafd8-601">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="aafd8-601">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="aafd8-602">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="aafd8-602">Az.ApiManagement</span></span>
* <span data-ttu-id="aafd8-603">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="aafd8-603">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="aafd8-604">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="aafd8-604">Az.Automation</span></span>
* <span data-ttu-id="aafd8-605">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="aafd8-605">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="aafd8-606">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="aafd8-606">Added Update Management cmdlets</span></span>
* <span data-ttu-id="aafd8-607">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="aafd8-607">Added Source Control cmdlets</span></span>
* <span data-ttu-id="aafd8-608">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="aafd8-608">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="aafd8-609">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="aafd8-609">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="aafd8-610">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aafd8-610">Az.Compute</span></span>
* <span data-ttu-id="aafd8-611">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="aafd8-611">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="aafd8-612">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="aafd8-612">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="aafd8-613">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="aafd8-613">Az.ContainerInstance</span></span>
* <span data-ttu-id="aafd8-614">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="aafd8-614">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="aafd8-615">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="aafd8-615">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="aafd8-616">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="aafd8-616">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="aafd8-617">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aafd8-617">Az.Network</span></span>
* <span data-ttu-id="aafd8-618">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="aafd8-618">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="aafd8-619">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="aafd8-619">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="aafd8-620">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="aafd8-620">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="aafd8-621">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="aafd8-621">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="aafd8-622">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="aafd8-622">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="aafd8-623">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="aafd8-623">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="aafd8-624">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="aafd8-624">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="aafd8-625">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="aafd8-625">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="aafd8-626">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="aafd8-626">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="aafd8-627">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="aafd8-627">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="aafd8-628">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="aafd8-628">Az.Relay</span></span>
* <span data-ttu-id="aafd8-629">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="aafd8-629">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="aafd8-630">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aafd8-630">Az.Resources</span></span>
* <span data-ttu-id="aafd8-631">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="aafd8-631">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="aafd8-632">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="aafd8-632">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="aafd8-633">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="aafd8-633">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="aafd8-634">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aafd8-634">Az.ServiceFabric</span></span>
* <span data-ttu-id="aafd8-635">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="aafd8-635">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="aafd8-636">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aafd8-636">Az.Sql</span></span>
* <span data-ttu-id="aafd8-637">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="aafd8-637">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="aafd8-638">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="aafd8-638">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="aafd8-639">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="aafd8-639">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="aafd8-640">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="aafd8-640">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="aafd8-641">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="aafd8-641">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="aafd8-642">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="aafd8-642">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="aafd8-643">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="aafd8-643">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="aafd8-644">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="aafd8-644">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="aafd8-645">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="aafd8-645">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="aafd8-646">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="aafd8-646">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="aafd8-647">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="aafd8-647">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="aafd8-648">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="aafd8-648">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="aafd8-649">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="aafd8-649">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="aafd8-650">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="aafd8-650">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="aafd8-651">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="aafd8-651">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="aafd8-652">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="aafd8-652">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="aafd8-653">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="aafd8-653">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="aafd8-654">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="aafd8-654">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="aafd8-655">Geral</span><span class="sxs-lookup"><span data-stu-id="aafd8-655">General</span></span>
* <span data-ttu-id="aafd8-656">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="aafd8-656">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="aafd8-657">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="aafd8-657">Az.Profile</span></span>
* <span data-ttu-id="aafd8-658">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="aafd8-658">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="aafd8-659">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="aafd8-659">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="aafd8-660">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="aafd8-660">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="aafd8-661">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="aafd8-661">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="aafd8-662">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="aafd8-662">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="aafd8-663">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="aafd8-663">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="aafd8-664">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="aafd8-664">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="aafd8-665">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="aafd8-665">Az.CognitiveServices</span></span>
* <span data-ttu-id="aafd8-666">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="aafd8-666">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aafd8-667">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aafd8-667">Az.Compute</span></span>
* <span data-ttu-id="aafd8-668">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="aafd8-668">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="aafd8-669">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="aafd8-669">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="aafd8-670">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="aafd8-670">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="aafd8-671">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="aafd8-671">Az.DataLakeStore</span></span>
* <span data-ttu-id="aafd8-672">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="aafd8-672">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="aafd8-673">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="aafd8-673">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="aafd8-674">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="aafd8-674">Az.Insights</span></span>
* <span data-ttu-id="aafd8-675">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="aafd8-675">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="aafd8-676">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="aafd8-676">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="aafd8-677">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="aafd8-677">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="aafd8-678">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="aafd8-678">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aafd8-679">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aafd8-679">Az.Network</span></span>
* <span data-ttu-id="aafd8-680">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="aafd8-680">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="aafd8-681">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="aafd8-681">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="aafd8-682">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="aafd8-682">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="aafd8-683">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="aafd8-683">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="aafd8-684">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="aafd8-684">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="aafd8-685">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="aafd8-685">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="aafd8-686">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="aafd8-686">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="aafd8-687">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="aafd8-687">Az.PolicyInsights</span></span>
* <span data-ttu-id="aafd8-688">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="aafd8-688">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="aafd8-689">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aafd8-689">Az.Resources</span></span>
* <span data-ttu-id="aafd8-690">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="aafd8-690">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="aafd8-691">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="aafd8-691">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="aafd8-692">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="aafd8-692">Az.ServiceBus</span></span>
* <span data-ttu-id="aafd8-693">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="aafd8-693">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="aafd8-694">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aafd8-694">Az.ServiceFabric</span></span>
* <span data-ttu-id="aafd8-695">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="aafd8-695">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="aafd8-696">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="aafd8-696">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="aafd8-697">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="aafd8-697">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="aafd8-698">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="aafd8-698">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="aafd8-699">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="aafd8-699">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="aafd8-700">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="aafd8-700">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="aafd8-701">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="aafd8-701">Az.Profile</span></span>
* <span data-ttu-id="aafd8-702">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="aafd8-702">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="aafd8-703">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="aafd8-703">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aafd8-704">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aafd8-704">Az.Compute</span></span>
* <span data-ttu-id="aafd8-705">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="aafd8-705">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="aafd8-706">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="aafd8-706">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="aafd8-707">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="aafd8-707">Az.DataLakeStore</span></span>
* <span data-ttu-id="aafd8-708">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="aafd8-708">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="aafd8-709">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="aafd8-709">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="aafd8-710">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="aafd8-710">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="aafd8-711">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="aafd8-711">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="aafd8-712">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="aafd8-712">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aafd8-713">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aafd8-713">Az.Network</span></span>
* <span data-ttu-id="aafd8-714">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="aafd8-714">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="aafd8-715">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="aafd8-715">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="aafd8-716">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aafd8-716">Az.Resources</span></span>
* <span data-ttu-id="aafd8-717">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="aafd8-717">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="aafd8-718">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="aafd8-718">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="aafd8-719">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="aafd8-719">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="aafd8-720">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="aafd8-720">Azure.Storage</span></span>
* <span data-ttu-id="aafd8-721">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="aafd8-721">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="aafd8-722">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="aafd8-722">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="aafd8-723">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="aafd8-723">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="aafd8-724">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="aafd8-724">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="aafd8-725">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="aafd8-725">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="aafd8-726">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="aafd8-726">Az.CognitiveServices</span></span>
* <span data-ttu-id="aafd8-727">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="aafd8-727">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aafd8-728">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aafd8-728">Az.Compute</span></span>
* <span data-ttu-id="aafd8-729">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="aafd8-729">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="aafd8-730">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="aafd8-730">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="aafd8-731">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="aafd8-731">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="aafd8-732">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="aafd8-732">Az.DataFactoryV2</span></span>
* <span data-ttu-id="aafd8-733">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="aafd8-733">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aafd8-734">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aafd8-734">Az.Network</span></span>
* <span data-ttu-id="aafd8-735">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="aafd8-735">Added NetworkProfile functionality.</span></span> <span data-ttu-id="aafd8-736">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="aafd8-736">new cmdlets added</span></span>
    - <span data-ttu-id="aafd8-737">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="aafd8-737">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="aafd8-738">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="aafd8-738">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="aafd8-739">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="aafd8-739">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="aafd8-740">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="aafd8-740">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="aafd8-741">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="aafd8-741">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="aafd8-742">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="aafd8-742">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="aafd8-743">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="aafd8-743">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="aafd8-744">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="aafd8-744">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="aafd8-745">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="aafd8-745">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="aafd8-746">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="aafd8-746">Az.RedisCache</span></span>
* <span data-ttu-id="aafd8-747">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="aafd8-747">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="aafd8-748">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="aafd8-748">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="aafd8-749">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aafd8-749">Az.Resources</span></span>
* <span data-ttu-id="aafd8-750">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="aafd8-750">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="aafd8-751">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="aafd8-751">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="aafd8-752">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aafd8-752">Az.Sql</span></span>
* <span data-ttu-id="aafd8-753">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="aafd8-753">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="aafd8-754">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aafd8-754">Az.Websites</span></span>
* <span data-ttu-id="aafd8-755">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="aafd8-755">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="aafd8-756">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="aafd8-756">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="aafd8-757">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="aafd8-757">0.2.0 - September 2018</span></span>
 <span data-ttu-id="aafd8-758">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="aafd8-758">Initial Release</span></span>