---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 04/30/2019
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: 1cc7d6519ded41003daed558a8e78ee65ded072a
ms.sourcegitcommit: 8b3126b5c79f453464d90669f0046ba86b7a3424
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/01/2020
ms.locfileid: "89240969"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="44e3b-103">Notas de versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="44e3b-103">Azure PowerShell release notes</span></span>
## <a name="180---april-2019"></a><span data-ttu-id="44e3b-104">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="44e3b-104">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="44e3b-105">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="44e3b-105">Highlights since the last major release</span></span>
* <span data-ttu-id="44e3b-106">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="44e3b-106">General availability of `Az` module</span></span>
* <span data-ttu-id="44e3b-107">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="44e3b-107">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="44e3b-108">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="44e3b-108">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="44e3b-109">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="44e3b-109">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="44e3b-110">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="44e3b-110">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="44e3b-111">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="44e3b-111">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="44e3b-112">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="44e3b-112">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="44e3b-113">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="44e3b-113">Az.Accounts</span></span>
* <span data-ttu-id="44e3b-114">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="44e3b-114">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="44e3b-115">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="44e3b-115">Az.Batch</span></span>
* <span data-ttu-id="44e3b-116">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="44e3b-116">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="44e3b-117">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="44e3b-117">Az.Cdn</span></span>
* <span data-ttu-id="44e3b-118">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="44e3b-118">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="44e3b-119">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="44e3b-119">Az.CognitiveServices</span></span>
* <span data-ttu-id="44e3b-120">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="44e3b-120">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="44e3b-121">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="44e3b-121">Az.Compute</span></span>
* <span data-ttu-id="44e3b-122">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="44e3b-122">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="44e3b-123">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="44e3b-123">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="44e3b-124">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="44e3b-124">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="44e3b-125">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="44e3b-125">Az.DataFactory</span></span>
* <span data-ttu-id="44e3b-126">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="44e3b-126">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="44e3b-127">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="44e3b-127">Az.DataLakeStore</span></span>
* <span data-ttu-id="44e3b-128">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="44e3b-128">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="44e3b-129">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="44e3b-129">Az.EventGrid</span></span>
* <span data-ttu-id="44e3b-130">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="44e3b-130">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="44e3b-131">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="44e3b-131">Az.EventHub</span></span>
* <span data-ttu-id="44e3b-132">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="44e3b-132">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="44e3b-133">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="44e3b-133">Az.HDInsight</span></span>
* <span data-ttu-id="44e3b-134">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="44e3b-134">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="44e3b-135">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="44e3b-135">Az.IotHub</span></span>
* <span data-ttu-id="44e3b-136">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="44e3b-136">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="44e3b-137">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="44e3b-137">Az.KeyVault</span></span>
* <span data-ttu-id="44e3b-138">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="44e3b-138">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="44e3b-139">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="44e3b-139">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="44e3b-140">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="44e3b-140">Az.MachineLearning</span></span>
* <span data-ttu-id="44e3b-141">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="44e3b-141">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="44e3b-142">Az.Media</span><span class="sxs-lookup"><span data-stu-id="44e3b-142">Az.Media</span></span>
* <span data-ttu-id="44e3b-143">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="44e3b-143">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="44e3b-144">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="44e3b-144">Az.Monitor</span></span>
  * <span data-ttu-id="44e3b-145">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="44e3b-145">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="44e3b-146">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="44e3b-146">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="44e3b-147">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="44e3b-147">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="44e3b-148">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="44e3b-148">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="44e3b-149">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="44e3b-149">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="44e3b-150">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="44e3b-150">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="44e3b-151">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="44e3b-151">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="44e3b-152">Az.Network</span><span class="sxs-lookup"><span data-stu-id="44e3b-152">Az.Network</span></span>
* <span data-ttu-id="44e3b-153">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="44e3b-153">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="44e3b-154">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="44e3b-154">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="44e3b-155">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="44e3b-155">Az.NotificationHubs</span></span>
* <span data-ttu-id="44e3b-156">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="44e3b-156">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="44e3b-157">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="44e3b-157">Az.OperationalInsights</span></span>
* <span data-ttu-id="44e3b-158">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="44e3b-158">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="44e3b-159">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="44e3b-159">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="44e3b-160">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="44e3b-160">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="44e3b-161">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="44e3b-161">Az.RecoveryServices</span></span>
* <span data-ttu-id="44e3b-162">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="44e3b-162">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="44e3b-163">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="44e3b-163">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="44e3b-164">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="44e3b-164">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="44e3b-165">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="44e3b-165">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="44e3b-166">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="44e3b-166">Az.RedisCache</span></span>
* <span data-ttu-id="44e3b-167">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="44e3b-167">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="44e3b-168">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44e3b-168">Az.Resources</span></span>
* <span data-ttu-id="44e3b-169">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="44e3b-169">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="44e3b-170">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="44e3b-170">Az.Sql</span></span>
* <span data-ttu-id="44e3b-171">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="44e3b-171">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="44e3b-172">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="44e3b-172">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="44e3b-173">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="44e3b-173">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="44e3b-174">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="44e3b-174">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="44e3b-175">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="44e3b-175">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="44e3b-176">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="44e3b-176">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="44e3b-177">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="44e3b-177">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="44e3b-178">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="44e3b-178">Az.Websites</span></span>
* <span data-ttu-id="44e3b-179">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="44e3b-179">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="44e3b-180">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="44e3b-180">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="44e3b-181">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="44e3b-181">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="44e3b-182">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="44e3b-182">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="44e3b-183">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="44e3b-183">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="44e3b-184">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="44e3b-184">Highlights since the last major release</span></span>
* <span data-ttu-id="44e3b-185">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="44e3b-185">General availability of `Az` module</span></span>
* <span data-ttu-id="44e3b-186">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="44e3b-186">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="44e3b-187">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="44e3b-187">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="44e3b-188">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="44e3b-188">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="44e3b-189">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="44e3b-189">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="44e3b-190">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="44e3b-190">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="44e3b-191">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="44e3b-191">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="44e3b-192">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="44e3b-192">Az.Accounts</span></span>
* <span data-ttu-id="44e3b-193">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="44e3b-193">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="44e3b-194">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="44e3b-194">Az.AnalysisServices</span></span>
* <span data-ttu-id="44e3b-195">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="44e3b-195">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="44e3b-196">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="44e3b-196">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="44e3b-197">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="44e3b-197">Az.Automation</span></span>
* <span data-ttu-id="44e3b-198">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="44e3b-198">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="44e3b-199">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="44e3b-199">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="44e3b-200">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="44e3b-200">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="44e3b-201">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="44e3b-201">Az.Compute</span></span>
* <span data-ttu-id="44e3b-202">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="44e3b-202">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="44e3b-203">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="44e3b-203">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="44e3b-204">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="44e3b-204">Az.ContainerInstance</span></span>
* <span data-ttu-id="44e3b-205">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="44e3b-205">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="44e3b-206">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="44e3b-206">Az.DataFactory</span></span>
* <span data-ttu-id="44e3b-207">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="44e3b-207">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="44e3b-208">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="44e3b-208">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="44e3b-209">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44e3b-209">Az.Resources</span></span>
* <span data-ttu-id="44e3b-210">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="44e3b-210">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="44e3b-211">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="44e3b-211">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="44e3b-212">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="44e3b-212">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="44e3b-213">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="44e3b-213">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="44e3b-214">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="44e3b-214">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="44e3b-215">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="44e3b-215">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="44e3b-216">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="44e3b-216">Az.Sql</span></span>
* <span data-ttu-id="44e3b-217">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="44e3b-217">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="44e3b-218">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="44e3b-218">Az.Storage</span></span>
* <span data-ttu-id="44e3b-219">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="44e3b-219">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="44e3b-220">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="44e3b-220">New-AzStorageContext</span></span>
* <span data-ttu-id="44e3b-221">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="44e3b-221">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="44e3b-222">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="44e3b-222">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="44e3b-223">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="44e3b-223">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="44e3b-224">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="44e3b-224">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="44e3b-225">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="44e3b-225">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="44e3b-226">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="44e3b-226">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="44e3b-227">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="44e3b-227">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="44e3b-228">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="44e3b-228">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="44e3b-229">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="44e3b-229">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="44e3b-230">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="44e3b-230">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="44e3b-231">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="44e3b-231">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="44e3b-232">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="44e3b-232">Highlights since the last major release</span></span>
* <span data-ttu-id="44e3b-233">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="44e3b-233">General availability of `Az` module</span></span>
* <span data-ttu-id="44e3b-234">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="44e3b-234">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="44e3b-235">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="44e3b-235">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="44e3b-236">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="44e3b-236">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="44e3b-237">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="44e3b-237">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="44e3b-238">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="44e3b-238">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="44e3b-239">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="44e3b-239">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="44e3b-240">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="44e3b-240">Az.Automation</span></span>
* <span data-ttu-id="44e3b-241">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="44e3b-241">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="44e3b-242">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="44e3b-242">Dynamic grouping</span></span>
    * <span data-ttu-id="44e3b-243">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="44e3b-243">Pre-Post script</span></span>
    * <span data-ttu-id="44e3b-244">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="44e3b-244">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="44e3b-245">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="44e3b-245">Az.Compute</span></span>
* <span data-ttu-id="44e3b-246">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="44e3b-246">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="44e3b-247">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="44e3b-247">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="44e3b-248">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="44e3b-248">Az.KeyVault</span></span>
* <span data-ttu-id="44e3b-249">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="44e3b-249">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="44e3b-250">Az.Network</span><span class="sxs-lookup"><span data-stu-id="44e3b-250">Az.Network</span></span>
* <span data-ttu-id="44e3b-251">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="44e3b-251">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="44e3b-252">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="44e3b-252">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="44e3b-253">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="44e3b-253">Az.RecoveryServices</span></span>
* <span data-ttu-id="44e3b-254">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="44e3b-254">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="44e3b-255">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="44e3b-255">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="44e3b-256">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44e3b-256">Az.Resources</span></span>
* <span data-ttu-id="44e3b-257">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="44e3b-257">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="44e3b-258">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="44e3b-258">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="44e3b-259">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="44e3b-259">Az.Sql</span></span>
* <span data-ttu-id="44e3b-260">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="44e3b-260">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="44e3b-261">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="44e3b-261">Az.Storage</span></span>
* <span data-ttu-id="44e3b-262">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="44e3b-262">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="44e3b-263">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="44e3b-263">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="44e3b-264">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="44e3b-264">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="44e3b-265">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="44e3b-265">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="44e3b-266">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="44e3b-266">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="44e3b-267">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="44e3b-267">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="44e3b-268">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="44e3b-268">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="44e3b-269">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="44e3b-269">Az.Websites</span></span>
* <span data-ttu-id="44e3b-270">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="44e3b-270">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="44e3b-271">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="44e3b-271">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="44e3b-272">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="44e3b-272">Az.Accounts</span></span>
* <span data-ttu-id="44e3b-273">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="44e3b-273">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="44e3b-274">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="44e3b-274">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="44e3b-275">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="44e3b-275">Az.Automation</span></span>
* <span data-ttu-id="44e3b-276">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="44e3b-276">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="44e3b-277">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="44e3b-277">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="44e3b-278">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="44e3b-278">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="44e3b-279">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="44e3b-279">Az.Cdn</span></span>
* <span data-ttu-id="44e3b-280">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="44e3b-280">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="44e3b-281">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="44e3b-281">Az.Compute</span></span>
* <span data-ttu-id="44e3b-282">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="44e3b-282">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="44e3b-283">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="44e3b-283">Az.DataFactory</span></span>
* <span data-ttu-id="44e3b-284">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="44e3b-284">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="44e3b-285">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="44e3b-285">Az.LogicApp</span></span>
* <span data-ttu-id="44e3b-286">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="44e3b-286">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="44e3b-287">Az.Network</span><span class="sxs-lookup"><span data-stu-id="44e3b-287">Az.Network</span></span>
* <span data-ttu-id="44e3b-288">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="44e3b-288">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="44e3b-289">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="44e3b-289">Az.RecoveryServices</span></span>
* <span data-ttu-id="44e3b-290">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="44e3b-290">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="44e3b-291">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="44e3b-291">SDK Update</span></span>
* <span data-ttu-id="44e3b-292">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="44e3b-292">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="44e3b-293">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="44e3b-293">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="44e3b-294">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44e3b-294">Az.Resources</span></span>
* <span data-ttu-id="44e3b-295">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="44e3b-295">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="44e3b-296">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="44e3b-296">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="44e3b-297">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="44e3b-297">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="44e3b-298">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="44e3b-298">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="44e3b-299">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="44e3b-299">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="44e3b-300">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="44e3b-300">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="44e3b-301">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="44e3b-301">Az.Sql</span></span>
* <span data-ttu-id="44e3b-302">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="44e3b-302">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="44e3b-303">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="44e3b-303">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="44e3b-304">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="44e3b-304">Az.Storage</span></span>
* <span data-ttu-id="44e3b-305">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="44e3b-305">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="44e3b-306">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="44e3b-306">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="44e3b-307">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="44e3b-307">Az.AnalysisServices</span></span>
* <span data-ttu-id="44e3b-308">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="44e3b-308">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="44e3b-309">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="44e3b-309">Az.Automation</span></span>
* <span data-ttu-id="44e3b-310">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="44e3b-310">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="44e3b-311">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="44e3b-311">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="44e3b-312">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="44e3b-312">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="44e3b-313">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="44e3b-313">Az.CognitiveServices</span></span>
* <span data-ttu-id="44e3b-314">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="44e3b-314">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="44e3b-315">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="44e3b-315">Az.Compute</span></span>
* <span data-ttu-id="44e3b-316">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="44e3b-316">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="44e3b-317">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="44e3b-317">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="44e3b-318">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="44e3b-318">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="44e3b-319">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="44e3b-319">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="44e3b-320">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="44e3b-320">Az.DataLakeStore</span></span>
* <span data-ttu-id="44e3b-321">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="44e3b-321">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="44e3b-322">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="44e3b-322">Az.EventHub</span></span>
* <span data-ttu-id="44e3b-323">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="44e3b-323">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="44e3b-324">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="44e3b-324">Az.KeyVault</span></span>
* <span data-ttu-id="44e3b-325">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="44e3b-325">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="44e3b-326">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="44e3b-326">Az.LogicApp</span></span>
* <span data-ttu-id="44e3b-327">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="44e3b-327">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="44e3b-328">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="44e3b-328">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="44e3b-329">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="44e3b-329">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="44e3b-330">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="44e3b-330">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="44e3b-331">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="44e3b-331">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="44e3b-332">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="44e3b-332">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="44e3b-333">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="44e3b-333">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="44e3b-334">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="44e3b-334">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="44e3b-335">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="44e3b-335">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="44e3b-336">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="44e3b-336">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="44e3b-337">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="44e3b-337">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="44e3b-338">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="44e3b-338">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="44e3b-339">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="44e3b-339">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="44e3b-340">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="44e3b-340">Az.Monitor</span></span>
* <span data-ttu-id="44e3b-341">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="44e3b-341">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="44e3b-342">Az.Network</span><span class="sxs-lookup"><span data-stu-id="44e3b-342">Az.Network</span></span>
* <span data-ttu-id="44e3b-343">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="44e3b-343">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="44e3b-344">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="44e3b-344">Az.OperationalInsights</span></span>
* <span data-ttu-id="44e3b-345">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="44e3b-345">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="44e3b-346">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="44e3b-346">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="44e3b-347">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="44e3b-347">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="44e3b-348">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44e3b-348">Az.Resources</span></span>
* <span data-ttu-id="44e3b-349">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="44e3b-349">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="44e3b-350">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="44e3b-350">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="44e3b-351">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="44e3b-351">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="44e3b-352">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="44e3b-352">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="44e3b-353">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="44e3b-353">Az.Sql</span></span>
* <span data-ttu-id="44e3b-354">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="44e3b-354">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="44e3b-355">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="44e3b-355">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="44e3b-356">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="44e3b-356">Az.Websites</span></span>
* <span data-ttu-id="44e3b-357">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="44e3b-357">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="44e3b-358">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="44e3b-358">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="44e3b-359">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="44e3b-359">Az.Accounts</span></span>
* <span data-ttu-id="44e3b-360">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="44e3b-360">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="44e3b-361">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="44e3b-361">Az.AnalysisServices</span></span>
<span data-ttu-id="44e3b-362">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="44e3b-362">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="44e3b-363">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="44e3b-363">Az.Compute</span></span>
* <span data-ttu-id="44e3b-364">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="44e3b-364">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="44e3b-365">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="44e3b-365">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="44e3b-366">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="44e3b-366">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="44e3b-367">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="44e3b-367">Az.RecoveryServices</span></span>
<span data-ttu-id="44e3b-368">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="44e3b-368">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="44e3b-369">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44e3b-369">Az.Resources</span></span>
* <span data-ttu-id="44e3b-370">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="44e3b-370">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="44e3b-371">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="44e3b-371">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="44e3b-372">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="44e3b-372">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="44e3b-373">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="44e3b-373">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="44e3b-374">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="44e3b-374">Az.Sql</span></span>
* <span data-ttu-id="44e3b-375">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="44e3b-375">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="44e3b-376">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="44e3b-376">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="44e3b-377">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="44e3b-377">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="44e3b-378">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="44e3b-378">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="44e3b-379">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="44e3b-379">Az.Accounts</span></span>
* <span data-ttu-id="44e3b-380">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="44e3b-380">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="44e3b-381">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="44e3b-381">Az.AnalysisServices</span></span>
* <span data-ttu-id="44e3b-382">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="44e3b-382">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="44e3b-383">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="44e3b-383">Az.RecoveryServices</span></span>
* <span data-ttu-id="44e3b-384">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="44e3b-384">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="44e3b-385">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="44e3b-385">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="44e3b-386">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="44e3b-386">Az.Accounts</span></span>
* <span data-ttu-id="44e3b-387">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="44e3b-387">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="44e3b-388">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="44e3b-388">Update incorrect online help URLs</span></span>
* <span data-ttu-id="44e3b-389">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="44e3b-389">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="44e3b-390">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="44e3b-390">Az.Aks</span></span>
* <span data-ttu-id="44e3b-391">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="44e3b-391">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="44e3b-392">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="44e3b-392">Az.Automation</span></span>
* <span data-ttu-id="44e3b-393">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="44e3b-393">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="44e3b-394">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="44e3b-394">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="44e3b-395">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="44e3b-395">Az.Cdn</span></span>
* <span data-ttu-id="44e3b-396">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="44e3b-396">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="44e3b-397">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="44e3b-397">Az.Compute</span></span>
* <span data-ttu-id="44e3b-398">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="44e3b-398">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="44e3b-399">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="44e3b-399">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="44e3b-400">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="44e3b-400">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="44e3b-401">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="44e3b-401">Az.ContainerRegistry</span></span>
* <span data-ttu-id="44e3b-402">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="44e3b-402">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="44e3b-403">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="44e3b-403">Az.DataFactory</span></span>
* <span data-ttu-id="44e3b-404">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="44e3b-404">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="44e3b-405">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="44e3b-405">Az.DataLakeStore</span></span>
* <span data-ttu-id="44e3b-406">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="44e3b-406">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="44e3b-407">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="44e3b-407">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="44e3b-408">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="44e3b-408">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="44e3b-409">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="44e3b-409">Az.IotHub</span></span>
* <span data-ttu-id="44e3b-410">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="44e3b-410">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="44e3b-411">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="44e3b-411">Az.KeyVault</span></span>
* <span data-ttu-id="44e3b-412">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="44e3b-412">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="44e3b-413">Az.Network</span><span class="sxs-lookup"><span data-stu-id="44e3b-413">Az.Network</span></span>
* <span data-ttu-id="44e3b-414">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="44e3b-414">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="44e3b-415">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44e3b-415">Az.Resources</span></span>
* <span data-ttu-id="44e3b-416">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="44e3b-416">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="44e3b-417">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="44e3b-417">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="44e3b-418">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="44e3b-418">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="44e3b-419">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="44e3b-419">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="44e3b-420">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="44e3b-420">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="44e3b-421">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="44e3b-421">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="44e3b-422">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="44e3b-422">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="44e3b-423">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="44e3b-423">Az.ServiceFabric</span></span>
* <span data-ttu-id="44e3b-424">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="44e3b-424">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="44e3b-425">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="44e3b-425">Fix some error messages.</span></span>
* <span data-ttu-id="44e3b-426">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="44e3b-426">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="44e3b-427">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="44e3b-427">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="44e3b-428">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="44e3b-428">Az.SignalR</span></span>
* <span data-ttu-id="44e3b-429">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="44e3b-429">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="44e3b-430">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="44e3b-430">Az.Sql</span></span>
* <span data-ttu-id="44e3b-431">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="44e3b-431">Update incorrect online help URLs</span></span>
* <span data-ttu-id="44e3b-432">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="44e3b-432">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="44e3b-433">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="44e3b-433">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="44e3b-434">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="44e3b-434">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="44e3b-435">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="44e3b-435">Az.Storage</span></span>
* <span data-ttu-id="44e3b-436">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="44e3b-436">Update incorrect online help URLs</span></span>
* <span data-ttu-id="44e3b-437">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="44e3b-437">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="44e3b-438">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="44e3b-438">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="44e3b-439">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="44e3b-439">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="44e3b-440">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="44e3b-440">Az.TrafficManager</span></span>
* <span data-ttu-id="44e3b-441">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="44e3b-441">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="44e3b-442">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="44e3b-442">Az.Websites</span></span>
* <span data-ttu-id="44e3b-443">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="44e3b-443">Update incorrect online help URLs</span></span>
* <span data-ttu-id="44e3b-444">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="44e3b-444">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="44e3b-445">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="44e3b-445">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="44e3b-446">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="44e3b-446">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="44e3b-447">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="44e3b-447">Az.Accounts</span></span>
* <span data-ttu-id="44e3b-448">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="44e3b-448">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="44e3b-449">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="44e3b-449">Az.Compute</span></span>
* <span data-ttu-id="44e3b-450">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="44e3b-450">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="44e3b-451">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="44e3b-451">Updated the description of ID in help files</span></span>
* <span data-ttu-id="44e3b-452">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="44e3b-452">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="44e3b-453">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="44e3b-453">Az.DataLakeStore</span></span>
* <span data-ttu-id="44e3b-454">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="44e3b-454">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="44e3b-455">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="44e3b-455">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="44e3b-456">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="44e3b-456">Az.EventGrid</span></span>
* <span data-ttu-id="44e3b-457">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="44e3b-457">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="44e3b-458">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="44e3b-458">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="44e3b-459">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="44e3b-459">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="44e3b-460">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="44e3b-460">Event Time-To-Live,</span></span>
        - <span data-ttu-id="44e3b-461">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="44e3b-461">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="44e3b-462">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="44e3b-462">Dead letter endpoint.</span></span>
    - <span data-ttu-id="44e3b-463">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="44e3b-463">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="44e3b-464">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="44e3b-464">Event Time-To-Live,</span></span>
        - <span data-ttu-id="44e3b-465">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="44e3b-465">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="44e3b-466">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="44e3b-466">Dead letter endpoint.</span></span>
* <span data-ttu-id="44e3b-467">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="44e3b-467">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="44e3b-468">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="44e3b-468">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="44e3b-469">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="44e3b-469">Az.IotHub</span></span>
* <span data-ttu-id="44e3b-470">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="44e3b-470">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="44e3b-471">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="44e3b-471">Az.LogicApp</span></span>
* <span data-ttu-id="44e3b-472">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="44e3b-472">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="44e3b-473">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44e3b-473">Az.Resources</span></span>
* <span data-ttu-id="44e3b-474">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="44e3b-474">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="44e3b-475">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="44e3b-475">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="44e3b-476">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="44e3b-476">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="44e3b-477">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="44e3b-477">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="44e3b-478">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="44e3b-478">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="44e3b-479">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="44e3b-479">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="44e3b-480">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="44e3b-480">Az.SignalR</span></span>
* <span data-ttu-id="44e3b-481">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="44e3b-481">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="44e3b-482">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="44e3b-482">Az.Sql</span></span>
* <span data-ttu-id="44e3b-483">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="44e3b-483">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="44e3b-484">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="44e3b-484">Az.Storage</span></span>
* <span data-ttu-id="44e3b-485">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="44e3b-485">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="44e3b-486">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="44e3b-486">New-AzStorageContext</span></span>
* <span data-ttu-id="44e3b-487">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="44e3b-487">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="44e3b-488">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="44e3b-488">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="44e3b-489">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="44e3b-489">Az.Websites</span></span>
* <span data-ttu-id="44e3b-490">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="44e3b-490">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="44e3b-491">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="44e3b-491">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="44e3b-492">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="44e3b-492">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="44e3b-493">Geral</span><span class="sxs-lookup"><span data-stu-id="44e3b-493">General</span></span>

- <span data-ttu-id="44e3b-494">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="44e3b-494">General Availability of Az Module</span></span>
- <span data-ttu-id="44e3b-495">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="44e3b-495">Online help for each module</span></span>
- <span data-ttu-id="44e3b-496">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="44e3b-496">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="44e3b-497">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="44e3b-497">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="44e3b-498">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="44e3b-498">Az.Accounts</span></span>
- <span data-ttu-id="44e3b-499">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="44e3b-499">Changed from Az.Profile</span></span>
- <span data-ttu-id="44e3b-500">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="44e3b-500">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="44e3b-501">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="44e3b-501">Az.ApiManagement</span></span>
- <span data-ttu-id="44e3b-502">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="44e3b-502">Fixes for #7002</span></span>
- <span data-ttu-id="44e3b-503">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44e3b-503">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="44e3b-504">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="44e3b-504">Az.Batch</span></span>
- <span data-ttu-id="44e3b-505">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="44e3b-505">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="44e3b-506">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="44e3b-506">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="44e3b-507">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44e3b-507">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="44e3b-508">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="44e3b-508">Az.Billing</span></span>
- <span data-ttu-id="44e3b-509">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44e3b-509">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="44e3b-510">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="44e3b-510">Az.CognitivServices</span></span>
- <span data-ttu-id="44e3b-511">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="44e3b-511">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="44e3b-512">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="44e3b-512">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="44e3b-513">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="44e3b-513">Az.ContainerInstance</span></span>
- <span data-ttu-id="44e3b-514">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="44e3b-514">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="44e3b-515">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="44e3b-515">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="44e3b-516">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44e3b-516">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="44e3b-517">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="44e3b-517">Az.DataLakeStore</span></span>
- <span data-ttu-id="44e3b-518">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44e3b-518">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="44e3b-519">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="44e3b-519">Az.Monitor</span></span>
- <span data-ttu-id="44e3b-520">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44e3b-520">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="44e3b-521">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="44e3b-521">Az.KeyVault</span></span>
- <span data-ttu-id="44e3b-522">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="44e3b-522">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="44e3b-523">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="44e3b-523">Az.MachineLearning</span></span>
- <span data-ttu-id="44e3b-524">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="44e3b-524">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="44e3b-525">Az.Media</span><span class="sxs-lookup"><span data-stu-id="44e3b-525">Az.Media</span></span>
- <span data-ttu-id="44e3b-526">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="44e3b-526">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="44e3b-527">Az.Network</span><span class="sxs-lookup"><span data-stu-id="44e3b-527">Az.Network</span></span>
<span data-ttu-id="44e3b-528">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="44e3b-528">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="44e3b-529">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="44e3b-529">New cmdlets added:</span></span>
        - <span data-ttu-id="44e3b-530">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="44e3b-530">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="44e3b-531">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="44e3b-531">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="44e3b-532">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="44e3b-532">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="44e3b-533">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="44e3b-533">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="44e3b-534">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="44e3b-534">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="44e3b-535">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="44e3b-535">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="44e3b-536">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="44e3b-536">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="44e3b-537">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="44e3b-537">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="44e3b-538">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="44e3b-538">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="44e3b-539">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="44e3b-539">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="44e3b-540">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="44e3b-540">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="44e3b-541">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="44e3b-541">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="44e3b-542">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="44e3b-542">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="44e3b-543">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="44e3b-543">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="44e3b-544">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="44e3b-544">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="44e3b-545">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="44e3b-545">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="44e3b-546">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="44e3b-546">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="44e3b-547">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="44e3b-547">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="44e3b-548">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="44e3b-548">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="44e3b-549">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="44e3b-549">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="44e3b-550">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44e3b-550">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="44e3b-551">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="44e3b-551">Az.OperationalInsights</span></span>
- <span data-ttu-id="44e3b-552">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44e3b-552">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="44e3b-553">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="44e3b-553">Az.Profile</span></span>
- <span data-ttu-id="44e3b-554">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="44e3b-554">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="44e3b-555">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="44e3b-555">Az.RecoveryServices</span></span>
- <span data-ttu-id="44e3b-556">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44e3b-556">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="44e3b-557">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44e3b-557">Az.Resources</span></span>
- <span data-ttu-id="44e3b-558">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44e3b-558">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="44e3b-559">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="44e3b-559">Az.ServiceFabric</span></span>
- <span data-ttu-id="44e3b-560">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="44e3b-560">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="44e3b-561">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44e3b-561">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="44e3b-562">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="44e3b-562">Az.SIgnalR</span></span>
- <span data-ttu-id="44e3b-563">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="44e3b-563">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="44e3b-564">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="44e3b-564">Az.Sql</span></span>
- <span data-ttu-id="44e3b-565">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="44e3b-565">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="44e3b-566">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="44e3b-566">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="44e3b-567">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44e3b-567">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="44e3b-568">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="44e3b-568">Az.Storage</span></span>
- <span data-ttu-id="44e3b-569">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44e3b-569">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="44e3b-570">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="44e3b-570">Az.Websites</span></span>
- <span data-ttu-id="44e3b-571">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="44e3b-571">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="44e3b-572">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="44e3b-572">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="44e3b-573">Geral</span><span class="sxs-lookup"><span data-stu-id="44e3b-573">General</span></span>

* <span data-ttu-id="44e3b-574">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="44e3b-574">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="44e3b-575">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="44e3b-575">Az.Compute</span></span>

* <span data-ttu-id="44e3b-576">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="44e3b-576">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="44e3b-577">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="44e3b-577">Az.DataLakeStore</span></span>

* <span data-ttu-id="44e3b-578">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="44e3b-578">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="44e3b-579">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="44e3b-579">Az.FrontDoor</span></span>

* <span data-ttu-id="44e3b-580">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="44e3b-580">Fixed some broken links</span></span>
    - <span data-ttu-id="44e3b-581">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="44e3b-581">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="44e3b-582">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="44e3b-582">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="44e3b-583">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="44e3b-583">Az.RecoveryServices</span></span>

* <span data-ttu-id="44e3b-584">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="44e3b-584">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="44e3b-585">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="44e3b-585">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="44e3b-586">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44e3b-586">Az.Resources</span></span>

* <span data-ttu-id="44e3b-587">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="44e3b-587">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="44e3b-588">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="44e3b-588">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="44e3b-589">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="44e3b-589">Az.Sql</span></span>

* <span data-ttu-id="44e3b-590">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="44e3b-590">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="44e3b-591">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="44e3b-591">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="44e3b-592">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="44e3b-592">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="44e3b-593">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="44e3b-593">Az.Storage</span></span>

* <span data-ttu-id="44e3b-594">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="44e3b-594">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="44e3b-595">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="44e3b-595">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="44e3b-596">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="44e3b-596">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="44e3b-597">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="44e3b-597">Support Static Website configuration</span></span>
    - <span data-ttu-id="44e3b-598">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="44e3b-598">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="44e3b-599">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="44e3b-599">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="44e3b-600">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="44e3b-600">Az.Websites</span></span>

* <span data-ttu-id="44e3b-601">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="44e3b-601">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="44e3b-602">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="44e3b-602">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="44e3b-603">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="44e3b-603">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="44e3b-604">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="44e3b-604">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="44e3b-605">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="44e3b-605">Az.ApiManagement</span></span>
* <span data-ttu-id="44e3b-606">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="44e3b-606">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="44e3b-607">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="44e3b-607">Az.Automation</span></span>
* <span data-ttu-id="44e3b-608">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="44e3b-608">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="44e3b-609">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="44e3b-609">Added Update Management cmdlets</span></span>
* <span data-ttu-id="44e3b-610">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="44e3b-610">Added Source Control cmdlets</span></span>
* <span data-ttu-id="44e3b-611">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="44e3b-611">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="44e3b-612">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="44e3b-612">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="44e3b-613">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="44e3b-613">Az.Compute</span></span>
* <span data-ttu-id="44e3b-614">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="44e3b-614">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="44e3b-615">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="44e3b-615">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="44e3b-616">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="44e3b-616">Az.ContainerInstance</span></span>
* <span data-ttu-id="44e3b-617">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="44e3b-617">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="44e3b-618">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="44e3b-618">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="44e3b-619">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="44e3b-619">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="44e3b-620">Az.Network</span><span class="sxs-lookup"><span data-stu-id="44e3b-620">Az.Network</span></span>
* <span data-ttu-id="44e3b-621">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="44e3b-621">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="44e3b-622">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="44e3b-622">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="44e3b-623">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="44e3b-623">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="44e3b-624">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="44e3b-624">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="44e3b-625">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="44e3b-625">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="44e3b-626">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="44e3b-626">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="44e3b-627">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="44e3b-627">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="44e3b-628">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="44e3b-628">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="44e3b-629">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="44e3b-629">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="44e3b-630">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="44e3b-630">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="44e3b-631">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="44e3b-631">Az.Relay</span></span>
* <span data-ttu-id="44e3b-632">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="44e3b-632">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="44e3b-633">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44e3b-633">Az.Resources</span></span>
* <span data-ttu-id="44e3b-634">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="44e3b-634">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="44e3b-635">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="44e3b-635">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="44e3b-636">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="44e3b-636">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="44e3b-637">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="44e3b-637">Az.ServiceFabric</span></span>
* <span data-ttu-id="44e3b-638">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="44e3b-638">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="44e3b-639">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="44e3b-639">Az.Sql</span></span>
* <span data-ttu-id="44e3b-640">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="44e3b-640">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="44e3b-641">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="44e3b-641">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="44e3b-642">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="44e3b-642">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="44e3b-643">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="44e3b-643">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="44e3b-644">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="44e3b-644">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="44e3b-645">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="44e3b-645">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="44e3b-646">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="44e3b-646">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="44e3b-647">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="44e3b-647">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="44e3b-648">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="44e3b-648">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="44e3b-649">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="44e3b-649">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="44e3b-650">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="44e3b-650">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="44e3b-651">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="44e3b-651">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="44e3b-652">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="44e3b-652">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="44e3b-653">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="44e3b-653">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="44e3b-654">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="44e3b-654">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="44e3b-655">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="44e3b-655">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="44e3b-656">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="44e3b-656">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="44e3b-657">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="44e3b-657">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="44e3b-658">Geral</span><span class="sxs-lookup"><span data-stu-id="44e3b-658">General</span></span>
* <span data-ttu-id="44e3b-659">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="44e3b-659">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="44e3b-660">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="44e3b-660">Az.Profile</span></span>
* <span data-ttu-id="44e3b-661">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="44e3b-661">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="44e3b-662">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="44e3b-662">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="44e3b-663">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="44e3b-663">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="44e3b-664">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="44e3b-664">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="44e3b-665">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="44e3b-665">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="44e3b-666">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="44e3b-666">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="44e3b-667">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="44e3b-667">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="44e3b-668">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="44e3b-668">Az.CognitiveServices</span></span>
* <span data-ttu-id="44e3b-669">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="44e3b-669">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="44e3b-670">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="44e3b-670">Az.Compute</span></span>
* <span data-ttu-id="44e3b-671">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="44e3b-671">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="44e3b-672">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="44e3b-672">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="44e3b-673">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="44e3b-673">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="44e3b-674">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="44e3b-674">Az.DataLakeStore</span></span>
* <span data-ttu-id="44e3b-675">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="44e3b-675">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="44e3b-676">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="44e3b-676">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="44e3b-677">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="44e3b-677">Az.Insights</span></span>
* <span data-ttu-id="44e3b-678">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="44e3b-678">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="44e3b-679">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="44e3b-679">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="44e3b-680">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="44e3b-680">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="44e3b-681">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="44e3b-681">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="44e3b-682">Az.Network</span><span class="sxs-lookup"><span data-stu-id="44e3b-682">Az.Network</span></span>
* <span data-ttu-id="44e3b-683">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="44e3b-683">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="44e3b-684">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="44e3b-684">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="44e3b-685">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="44e3b-685">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="44e3b-686">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="44e3b-686">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="44e3b-687">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="44e3b-687">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="44e3b-688">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="44e3b-688">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="44e3b-689">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="44e3b-689">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="44e3b-690">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="44e3b-690">Az.PolicyInsights</span></span>
* <span data-ttu-id="44e3b-691">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="44e3b-691">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="44e3b-692">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44e3b-692">Az.Resources</span></span>
* <span data-ttu-id="44e3b-693">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="44e3b-693">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="44e3b-694">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="44e3b-694">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="44e3b-695">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="44e3b-695">Az.ServiceBus</span></span>
* <span data-ttu-id="44e3b-696">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="44e3b-696">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="44e3b-697">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="44e3b-697">Az.ServiceFabric</span></span>
* <span data-ttu-id="44e3b-698">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="44e3b-698">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="44e3b-699">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="44e3b-699">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="44e3b-700">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="44e3b-700">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="44e3b-701">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="44e3b-701">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="44e3b-702">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="44e3b-702">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="44e3b-703">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="44e3b-703">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="44e3b-704">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="44e3b-704">Az.Profile</span></span>
* <span data-ttu-id="44e3b-705">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="44e3b-705">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="44e3b-706">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="44e3b-706">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="44e3b-707">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="44e3b-707">Az.Compute</span></span>
* <span data-ttu-id="44e3b-708">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="44e3b-708">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="44e3b-709">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="44e3b-709">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="44e3b-710">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="44e3b-710">Az.DataLakeStore</span></span>
* <span data-ttu-id="44e3b-711">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="44e3b-711">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="44e3b-712">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="44e3b-712">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="44e3b-713">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="44e3b-713">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="44e3b-714">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="44e3b-714">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="44e3b-715">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="44e3b-715">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="44e3b-716">Az.Network</span><span class="sxs-lookup"><span data-stu-id="44e3b-716">Az.Network</span></span>
* <span data-ttu-id="44e3b-717">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="44e3b-717">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="44e3b-718">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="44e3b-718">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="44e3b-719">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44e3b-719">Az.Resources</span></span>
* <span data-ttu-id="44e3b-720">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="44e3b-720">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="44e3b-721">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="44e3b-721">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="44e3b-722">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="44e3b-722">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="44e3b-723">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="44e3b-723">Azure.Storage</span></span>
* <span data-ttu-id="44e3b-724">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="44e3b-724">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="44e3b-725">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="44e3b-725">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="44e3b-726">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="44e3b-726">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="44e3b-727">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="44e3b-727">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="44e3b-728">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="44e3b-728">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="44e3b-729">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="44e3b-729">Az.CognitiveServices</span></span>
* <span data-ttu-id="44e3b-730">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="44e3b-730">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="44e3b-731">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="44e3b-731">Az.Compute</span></span>
* <span data-ttu-id="44e3b-732">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="44e3b-732">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="44e3b-733">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="44e3b-733">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="44e3b-734">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="44e3b-734">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="44e3b-735">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="44e3b-735">Az.DataFactoryV2</span></span>
* <span data-ttu-id="44e3b-736">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="44e3b-736">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="44e3b-737">Az.Network</span><span class="sxs-lookup"><span data-stu-id="44e3b-737">Az.Network</span></span>
* <span data-ttu-id="44e3b-738">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="44e3b-738">Added NetworkProfile functionality.</span></span> <span data-ttu-id="44e3b-739">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="44e3b-739">new cmdlets added</span></span>
    - <span data-ttu-id="44e3b-740">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="44e3b-740">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="44e3b-741">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="44e3b-741">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="44e3b-742">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="44e3b-742">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="44e3b-743">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="44e3b-743">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="44e3b-744">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="44e3b-744">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="44e3b-745">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="44e3b-745">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="44e3b-746">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="44e3b-746">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="44e3b-747">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="44e3b-747">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="44e3b-748">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="44e3b-748">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="44e3b-749">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="44e3b-749">Az.RedisCache</span></span>
* <span data-ttu-id="44e3b-750">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="44e3b-750">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="44e3b-751">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="44e3b-751">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="44e3b-752">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="44e3b-752">Az.Resources</span></span>
* <span data-ttu-id="44e3b-753">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="44e3b-753">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="44e3b-754">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="44e3b-754">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="44e3b-755">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="44e3b-755">Az.Sql</span></span>
* <span data-ttu-id="44e3b-756">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="44e3b-756">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="44e3b-757">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="44e3b-757">Az.Websites</span></span>
* <span data-ttu-id="44e3b-758">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="44e3b-758">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="44e3b-759">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="44e3b-759">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="44e3b-760">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="44e3b-760">0.2.0 - September 2018</span></span>
 <span data-ttu-id="44e3b-761">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="44e3b-761">Initial Release</span></span>
