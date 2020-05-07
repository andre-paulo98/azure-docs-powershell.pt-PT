---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 04/30/2019
ms.openlocfilehash: 8a9a399f72ed9e3e9a3cbc09c8a4abaa91339c24
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/05/2020
ms.locfileid: "71319299"
---
## <a name="180---april-2019"></a><span data-ttu-id="99cfd-103">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="99cfd-103">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="99cfd-104">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="99cfd-104">Highlights since the last major release</span></span>
* <span data-ttu-id="99cfd-105">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="99cfd-105">General availability of `Az` module</span></span>
* <span data-ttu-id="99cfd-106">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="99cfd-106">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="99cfd-107">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="99cfd-107">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="99cfd-108">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="99cfd-108">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="99cfd-109">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="99cfd-109">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="99cfd-110">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="99cfd-110">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="99cfd-111">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="99cfd-111">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="99cfd-112">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="99cfd-112">Az.Accounts</span></span>
* <span data-ttu-id="99cfd-113">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="99cfd-113">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="99cfd-114">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="99cfd-114">Az.Batch</span></span>
* <span data-ttu-id="99cfd-115">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="99cfd-115">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="99cfd-116">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="99cfd-116">Az.Cdn</span></span>
* <span data-ttu-id="99cfd-117">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="99cfd-117">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="99cfd-118">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="99cfd-118">Az.CognitiveServices</span></span>
* <span data-ttu-id="99cfd-119">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="99cfd-119">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="99cfd-120">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="99cfd-120">Az.Compute</span></span>
* <span data-ttu-id="99cfd-121">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="99cfd-121">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="99cfd-122">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="99cfd-122">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="99cfd-123">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="99cfd-123">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="99cfd-124">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="99cfd-124">Az.DataFactory</span></span>
* <span data-ttu-id="99cfd-125">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="99cfd-125">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="99cfd-126">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="99cfd-126">Az.DataLakeStore</span></span>
* <span data-ttu-id="99cfd-127">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="99cfd-127">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="99cfd-128">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="99cfd-128">Az.EventGrid</span></span>
* <span data-ttu-id="99cfd-129">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="99cfd-129">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="99cfd-130">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="99cfd-130">Az.EventHub</span></span>
* <span data-ttu-id="99cfd-131">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="99cfd-131">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="99cfd-132">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="99cfd-132">Az.HDInsight</span></span>
* <span data-ttu-id="99cfd-133">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="99cfd-133">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="99cfd-134">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="99cfd-134">Az.IotHub</span></span>
* <span data-ttu-id="99cfd-135">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="99cfd-135">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="99cfd-136">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="99cfd-136">Az.KeyVault</span></span>
* <span data-ttu-id="99cfd-137">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="99cfd-137">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="99cfd-138">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="99cfd-138">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="99cfd-139">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="99cfd-139">Az.MachineLearning</span></span>
* <span data-ttu-id="99cfd-140">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="99cfd-140">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="99cfd-141">Az.Media</span><span class="sxs-lookup"><span data-stu-id="99cfd-141">Az.Media</span></span>
* <span data-ttu-id="99cfd-142">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="99cfd-142">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="99cfd-143">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="99cfd-143">Az.Monitor</span></span>
  * <span data-ttu-id="99cfd-144">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="99cfd-144">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="99cfd-145">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="99cfd-145">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="99cfd-146">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="99cfd-146">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="99cfd-147">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="99cfd-147">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="99cfd-148">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="99cfd-148">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="99cfd-149">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="99cfd-149">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="99cfd-150">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="99cfd-150">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="99cfd-151">Az.Network</span><span class="sxs-lookup"><span data-stu-id="99cfd-151">Az.Network</span></span>
* <span data-ttu-id="99cfd-152">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="99cfd-152">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="99cfd-153">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="99cfd-153">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="99cfd-154">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="99cfd-154">Az.NotificationHubs</span></span>
* <span data-ttu-id="99cfd-155">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="99cfd-155">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="99cfd-156">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="99cfd-156">Az.OperationalInsights</span></span>
* <span data-ttu-id="99cfd-157">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="99cfd-157">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="99cfd-158">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="99cfd-158">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="99cfd-159">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="99cfd-159">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="99cfd-160">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="99cfd-160">Az.RecoveryServices</span></span>
* <span data-ttu-id="99cfd-161">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="99cfd-161">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="99cfd-162">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="99cfd-162">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="99cfd-163">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="99cfd-163">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="99cfd-164">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="99cfd-164">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="99cfd-165">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="99cfd-165">Az.RedisCache</span></span>
* <span data-ttu-id="99cfd-166">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="99cfd-166">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="99cfd-167">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="99cfd-167">Az.Resources</span></span>
* <span data-ttu-id="99cfd-168">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="99cfd-168">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="99cfd-169">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="99cfd-169">Az.Sql</span></span>
* <span data-ttu-id="99cfd-170">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="99cfd-170">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="99cfd-171">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="99cfd-171">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="99cfd-172">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="99cfd-172">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="99cfd-173">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="99cfd-173">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="99cfd-174">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="99cfd-174">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="99cfd-175">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="99cfd-175">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="99cfd-176">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="99cfd-176">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="99cfd-177">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="99cfd-177">Az.Websites</span></span>
* <span data-ttu-id="99cfd-178">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="99cfd-178">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="99cfd-179">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="99cfd-179">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="99cfd-180">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="99cfd-180">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="99cfd-181">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="99cfd-181">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="99cfd-182">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="99cfd-182">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="99cfd-183">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="99cfd-183">Highlights since the last major release</span></span>
* <span data-ttu-id="99cfd-184">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="99cfd-184">General availability of `Az` module</span></span>
* <span data-ttu-id="99cfd-185">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="99cfd-185">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="99cfd-186">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="99cfd-186">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="99cfd-187">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="99cfd-187">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="99cfd-188">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="99cfd-188">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="99cfd-189">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="99cfd-189">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="99cfd-190">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="99cfd-190">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="99cfd-191">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="99cfd-191">Az.Accounts</span></span>
* <span data-ttu-id="99cfd-192">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="99cfd-192">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="99cfd-193">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="99cfd-193">Az.AnalysisServices</span></span>
* <span data-ttu-id="99cfd-194">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="99cfd-194">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="99cfd-195">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="99cfd-195">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="99cfd-196">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="99cfd-196">Az.Automation</span></span>
* <span data-ttu-id="99cfd-197">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="99cfd-197">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="99cfd-198">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="99cfd-198">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="99cfd-199">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="99cfd-199">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="99cfd-200">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="99cfd-200">Az.Compute</span></span>
* <span data-ttu-id="99cfd-201">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="99cfd-201">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="99cfd-202">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="99cfd-202">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="99cfd-203">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="99cfd-203">Az.ContainerInstance</span></span>
* <span data-ttu-id="99cfd-204">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="99cfd-204">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="99cfd-205">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="99cfd-205">Az.DataFactory</span></span>
* <span data-ttu-id="99cfd-206">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="99cfd-206">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="99cfd-207">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="99cfd-207">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="99cfd-208">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="99cfd-208">Az.Resources</span></span>
* <span data-ttu-id="99cfd-209">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="99cfd-209">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="99cfd-210">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="99cfd-210">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="99cfd-211">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="99cfd-211">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="99cfd-212">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="99cfd-212">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="99cfd-213">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="99cfd-213">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="99cfd-214">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="99cfd-214">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="99cfd-215">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="99cfd-215">Az.Sql</span></span>
* <span data-ttu-id="99cfd-216">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="99cfd-216">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="99cfd-217">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="99cfd-217">Az.Storage</span></span>
* <span data-ttu-id="99cfd-218">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="99cfd-218">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="99cfd-219">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="99cfd-219">New-AzStorageContext</span></span>
* <span data-ttu-id="99cfd-220">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="99cfd-220">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="99cfd-221">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="99cfd-221">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="99cfd-222">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="99cfd-222">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="99cfd-223">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="99cfd-223">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="99cfd-224">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="99cfd-224">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="99cfd-225">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="99cfd-225">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="99cfd-226">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="99cfd-226">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="99cfd-227">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="99cfd-227">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="99cfd-228">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="99cfd-228">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="99cfd-229">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="99cfd-229">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="99cfd-230">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="99cfd-230">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="99cfd-231">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="99cfd-231">Highlights since the last major release</span></span>
* <span data-ttu-id="99cfd-232">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="99cfd-232">General availability of `Az` module</span></span>
* <span data-ttu-id="99cfd-233">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="99cfd-233">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="99cfd-234">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="99cfd-234">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="99cfd-235">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="99cfd-235">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="99cfd-236">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="99cfd-236">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="99cfd-237">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="99cfd-237">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="99cfd-238">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="99cfd-238">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="99cfd-239">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="99cfd-239">Az.Automation</span></span>
* <span data-ttu-id="99cfd-240">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="99cfd-240">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="99cfd-241">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="99cfd-241">Dynamic grouping</span></span>
    * <span data-ttu-id="99cfd-242">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="99cfd-242">Pre-Post script</span></span>
    * <span data-ttu-id="99cfd-243">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="99cfd-243">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="99cfd-244">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="99cfd-244">Az.Compute</span></span>
* <span data-ttu-id="99cfd-245">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="99cfd-245">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="99cfd-246">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="99cfd-246">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="99cfd-247">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="99cfd-247">Az.KeyVault</span></span>
* <span data-ttu-id="99cfd-248">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="99cfd-248">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="99cfd-249">Az.Network</span><span class="sxs-lookup"><span data-stu-id="99cfd-249">Az.Network</span></span>
* <span data-ttu-id="99cfd-250">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="99cfd-250">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="99cfd-251">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="99cfd-251">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="99cfd-252">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="99cfd-252">Az.RecoveryServices</span></span>
* <span data-ttu-id="99cfd-253">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="99cfd-253">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="99cfd-254">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="99cfd-254">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="99cfd-255">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="99cfd-255">Az.Resources</span></span>
* <span data-ttu-id="99cfd-256">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="99cfd-256">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="99cfd-257">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="99cfd-257">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="99cfd-258">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="99cfd-258">Az.Sql</span></span>
* <span data-ttu-id="99cfd-259">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="99cfd-259">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="99cfd-260">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="99cfd-260">Az.Storage</span></span>
* <span data-ttu-id="99cfd-261">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="99cfd-261">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="99cfd-262">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="99cfd-262">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="99cfd-263">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="99cfd-263">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="99cfd-264">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="99cfd-264">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="99cfd-265">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="99cfd-265">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="99cfd-266">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="99cfd-266">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="99cfd-267">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="99cfd-267">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="99cfd-268">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="99cfd-268">Az.Websites</span></span>
* <span data-ttu-id="99cfd-269">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="99cfd-269">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="99cfd-270">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="99cfd-270">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="99cfd-271">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="99cfd-271">Az.Accounts</span></span>
* <span data-ttu-id="99cfd-272">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="99cfd-272">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="99cfd-273">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="99cfd-273">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="99cfd-274">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="99cfd-274">Az.Automation</span></span>
* <span data-ttu-id="99cfd-275">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="99cfd-275">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="99cfd-276">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="99cfd-276">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="99cfd-277">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="99cfd-277">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="99cfd-278">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="99cfd-278">Az.Cdn</span></span>
* <span data-ttu-id="99cfd-279">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="99cfd-279">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="99cfd-280">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="99cfd-280">Az.Compute</span></span>
* <span data-ttu-id="99cfd-281">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="99cfd-281">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="99cfd-282">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="99cfd-282">Az.DataFactory</span></span>
* <span data-ttu-id="99cfd-283">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="99cfd-283">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="99cfd-284">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="99cfd-284">Az.LogicApp</span></span>
* <span data-ttu-id="99cfd-285">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="99cfd-285">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="99cfd-286">Az.Network</span><span class="sxs-lookup"><span data-stu-id="99cfd-286">Az.Network</span></span>
* <span data-ttu-id="99cfd-287">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="99cfd-287">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="99cfd-288">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="99cfd-288">Az.RecoveryServices</span></span>
* <span data-ttu-id="99cfd-289">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="99cfd-289">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="99cfd-290">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="99cfd-290">SDK Update</span></span>
* <span data-ttu-id="99cfd-291">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="99cfd-291">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="99cfd-292">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="99cfd-292">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="99cfd-293">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="99cfd-293">Az.Resources</span></span>
* <span data-ttu-id="99cfd-294">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="99cfd-294">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="99cfd-295">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="99cfd-295">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="99cfd-296">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="99cfd-296">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="99cfd-297">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="99cfd-297">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="99cfd-298">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="99cfd-298">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="99cfd-299">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="99cfd-299">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="99cfd-300">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="99cfd-300">Az.Sql</span></span>
* <span data-ttu-id="99cfd-301">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="99cfd-301">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="99cfd-302">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="99cfd-302">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="99cfd-303">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="99cfd-303">Az.Storage</span></span>
* <span data-ttu-id="99cfd-304">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="99cfd-304">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="99cfd-305">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="99cfd-305">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="99cfd-306">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="99cfd-306">Az.AnalysisServices</span></span>
* <span data-ttu-id="99cfd-307">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="99cfd-307">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="99cfd-308">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="99cfd-308">Az.Automation</span></span>
* <span data-ttu-id="99cfd-309">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="99cfd-309">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="99cfd-310">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="99cfd-310">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="99cfd-311">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="99cfd-311">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="99cfd-312">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="99cfd-312">Az.CognitiveServices</span></span>
* <span data-ttu-id="99cfd-313">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="99cfd-313">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="99cfd-314">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="99cfd-314">Az.Compute</span></span>
* <span data-ttu-id="99cfd-315">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="99cfd-315">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="99cfd-316">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="99cfd-316">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="99cfd-317">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="99cfd-317">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="99cfd-318">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="99cfd-318">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="99cfd-319">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="99cfd-319">Az.DataLakeStore</span></span>
* <span data-ttu-id="99cfd-320">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="99cfd-320">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="99cfd-321">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="99cfd-321">Az.EventHub</span></span>
* <span data-ttu-id="99cfd-322">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="99cfd-322">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="99cfd-323">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="99cfd-323">Az.KeyVault</span></span>
* <span data-ttu-id="99cfd-324">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="99cfd-324">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="99cfd-325">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="99cfd-325">Az.LogicApp</span></span>
* <span data-ttu-id="99cfd-326">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="99cfd-326">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="99cfd-327">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="99cfd-327">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="99cfd-328">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="99cfd-328">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="99cfd-329">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="99cfd-329">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="99cfd-330">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="99cfd-330">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="99cfd-331">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="99cfd-331">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="99cfd-332">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="99cfd-332">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="99cfd-333">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="99cfd-333">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="99cfd-334">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="99cfd-334">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="99cfd-335">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="99cfd-335">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="99cfd-336">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="99cfd-336">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="99cfd-337">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="99cfd-337">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="99cfd-338">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="99cfd-338">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="99cfd-339">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="99cfd-339">Az.Monitor</span></span>
* <span data-ttu-id="99cfd-340">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="99cfd-340">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="99cfd-341">Az.Network</span><span class="sxs-lookup"><span data-stu-id="99cfd-341">Az.Network</span></span>
* <span data-ttu-id="99cfd-342">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="99cfd-342">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="99cfd-343">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="99cfd-343">Az.OperationalInsights</span></span>
* <span data-ttu-id="99cfd-344">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="99cfd-344">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="99cfd-345">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="99cfd-345">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="99cfd-346">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="99cfd-346">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="99cfd-347">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="99cfd-347">Az.Resources</span></span>
* <span data-ttu-id="99cfd-348">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="99cfd-348">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="99cfd-349">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="99cfd-349">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="99cfd-350">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="99cfd-350">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="99cfd-351">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="99cfd-351">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="99cfd-352">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="99cfd-352">Az.Sql</span></span>
* <span data-ttu-id="99cfd-353">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="99cfd-353">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="99cfd-354">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="99cfd-354">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="99cfd-355">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="99cfd-355">Az.Websites</span></span>
* <span data-ttu-id="99cfd-356">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="99cfd-356">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="99cfd-357">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="99cfd-357">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="99cfd-358">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="99cfd-358">Az.Accounts</span></span>
* <span data-ttu-id="99cfd-359">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="99cfd-359">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="99cfd-360">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="99cfd-360">Az.AnalysisServices</span></span>
<span data-ttu-id="99cfd-361">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="99cfd-361">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="99cfd-362">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="99cfd-362">Az.Compute</span></span>
* <span data-ttu-id="99cfd-363">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="99cfd-363">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="99cfd-364">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="99cfd-364">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="99cfd-365">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="99cfd-365">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="99cfd-366">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="99cfd-366">Az.RecoveryServices</span></span>
<span data-ttu-id="99cfd-367">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="99cfd-367">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="99cfd-368">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="99cfd-368">Az.Resources</span></span>
* <span data-ttu-id="99cfd-369">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="99cfd-369">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="99cfd-370">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="99cfd-370">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="99cfd-371">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="99cfd-371">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="99cfd-372">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="99cfd-372">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="99cfd-373">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="99cfd-373">Az.Sql</span></span>
* <span data-ttu-id="99cfd-374">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="99cfd-374">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="99cfd-375">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="99cfd-375">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="99cfd-376">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="99cfd-376">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="99cfd-377">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="99cfd-377">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="99cfd-378">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="99cfd-378">Az.Accounts</span></span>
* <span data-ttu-id="99cfd-379">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="99cfd-379">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="99cfd-380">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="99cfd-380">Az.AnalysisServices</span></span>
* <span data-ttu-id="99cfd-381">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="99cfd-381">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="99cfd-382">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="99cfd-382">Az.RecoveryServices</span></span>
* <span data-ttu-id="99cfd-383">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="99cfd-383">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="99cfd-384">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="99cfd-384">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="99cfd-385">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="99cfd-385">Az.Accounts</span></span>
* <span data-ttu-id="99cfd-386">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="99cfd-386">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="99cfd-387">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="99cfd-387">Update incorrect online help URLs</span></span>
* <span data-ttu-id="99cfd-388">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="99cfd-388">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="99cfd-389">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="99cfd-389">Az.Aks</span></span>
* <span data-ttu-id="99cfd-390">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="99cfd-390">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="99cfd-391">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="99cfd-391">Az.Automation</span></span>
* <span data-ttu-id="99cfd-392">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="99cfd-392">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="99cfd-393">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="99cfd-393">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="99cfd-394">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="99cfd-394">Az.Cdn</span></span>
* <span data-ttu-id="99cfd-395">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="99cfd-395">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="99cfd-396">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="99cfd-396">Az.Compute</span></span>
* <span data-ttu-id="99cfd-397">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="99cfd-397">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="99cfd-398">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="99cfd-398">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="99cfd-399">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="99cfd-399">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="99cfd-400">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="99cfd-400">Az.ContainerRegistry</span></span>
* <span data-ttu-id="99cfd-401">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="99cfd-401">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="99cfd-402">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="99cfd-402">Az.DataFactory</span></span>
* <span data-ttu-id="99cfd-403">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="99cfd-403">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="99cfd-404">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="99cfd-404">Az.DataLakeStore</span></span>
* <span data-ttu-id="99cfd-405">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="99cfd-405">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="99cfd-406">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="99cfd-406">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="99cfd-407">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="99cfd-407">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="99cfd-408">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="99cfd-408">Az.IotHub</span></span>
* <span data-ttu-id="99cfd-409">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="99cfd-409">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="99cfd-410">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="99cfd-410">Az.KeyVault</span></span>
* <span data-ttu-id="99cfd-411">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="99cfd-411">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="99cfd-412">Az.Network</span><span class="sxs-lookup"><span data-stu-id="99cfd-412">Az.Network</span></span>
* <span data-ttu-id="99cfd-413">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="99cfd-413">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="99cfd-414">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="99cfd-414">Az.Resources</span></span>
* <span data-ttu-id="99cfd-415">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="99cfd-415">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="99cfd-416">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="99cfd-416">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="99cfd-417">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="99cfd-417">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="99cfd-418">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="99cfd-418">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="99cfd-419">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="99cfd-419">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="99cfd-420">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="99cfd-420">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="99cfd-421">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="99cfd-421">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="99cfd-422">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="99cfd-422">Az.ServiceFabric</span></span>
* <span data-ttu-id="99cfd-423">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="99cfd-423">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="99cfd-424">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="99cfd-424">Fix some error messages.</span></span>
* <span data-ttu-id="99cfd-425">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="99cfd-425">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="99cfd-426">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="99cfd-426">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="99cfd-427">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="99cfd-427">Az.SignalR</span></span>
* <span data-ttu-id="99cfd-428">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="99cfd-428">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="99cfd-429">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="99cfd-429">Az.Sql</span></span>
* <span data-ttu-id="99cfd-430">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="99cfd-430">Update incorrect online help URLs</span></span>
* <span data-ttu-id="99cfd-431">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="99cfd-431">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="99cfd-432">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="99cfd-432">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="99cfd-433">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="99cfd-433">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="99cfd-434">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="99cfd-434">Az.Storage</span></span>
* <span data-ttu-id="99cfd-435">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="99cfd-435">Update incorrect online help URLs</span></span>
* <span data-ttu-id="99cfd-436">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="99cfd-436">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="99cfd-437">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="99cfd-437">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="99cfd-438">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="99cfd-438">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="99cfd-439">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="99cfd-439">Az.TrafficManager</span></span>
* <span data-ttu-id="99cfd-440">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="99cfd-440">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="99cfd-441">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="99cfd-441">Az.Websites</span></span>
* <span data-ttu-id="99cfd-442">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="99cfd-442">Update incorrect online help URLs</span></span>
* <span data-ttu-id="99cfd-443">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="99cfd-443">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="99cfd-444">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="99cfd-444">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="99cfd-445">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="99cfd-445">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="99cfd-446">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="99cfd-446">Az.Accounts</span></span>
* <span data-ttu-id="99cfd-447">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="99cfd-447">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="99cfd-448">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="99cfd-448">Az.Compute</span></span>
* <span data-ttu-id="99cfd-449">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="99cfd-449">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="99cfd-450">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="99cfd-450">Updated the description of ID in help files</span></span>
* <span data-ttu-id="99cfd-451">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="99cfd-451">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="99cfd-452">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="99cfd-452">Az.DataLakeStore</span></span>
* <span data-ttu-id="99cfd-453">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="99cfd-453">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="99cfd-454">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="99cfd-454">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="99cfd-455">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="99cfd-455">Az.EventGrid</span></span>
* <span data-ttu-id="99cfd-456">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="99cfd-456">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="99cfd-457">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="99cfd-457">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="99cfd-458">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="99cfd-458">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="99cfd-459">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="99cfd-459">Event Time-To-Live,</span></span>
        - <span data-ttu-id="99cfd-460">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="99cfd-460">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="99cfd-461">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="99cfd-461">Dead letter endpoint.</span></span>
    - <span data-ttu-id="99cfd-462">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="99cfd-462">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="99cfd-463">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="99cfd-463">Event Time-To-Live,</span></span>
        - <span data-ttu-id="99cfd-464">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="99cfd-464">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="99cfd-465">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="99cfd-465">Dead letter endpoint.</span></span>
* <span data-ttu-id="99cfd-466">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="99cfd-466">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="99cfd-467">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="99cfd-467">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="99cfd-468">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="99cfd-468">Az.IotHub</span></span>
* <span data-ttu-id="99cfd-469">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="99cfd-469">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="99cfd-470">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="99cfd-470">Az.LogicApp</span></span>
* <span data-ttu-id="99cfd-471">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="99cfd-471">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="99cfd-472">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="99cfd-472">Az.Resources</span></span>
* <span data-ttu-id="99cfd-473">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="99cfd-473">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="99cfd-474">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="99cfd-474">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="99cfd-475">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="99cfd-475">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="99cfd-476">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="99cfd-476">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="99cfd-477">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="99cfd-477">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="99cfd-478">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="99cfd-478">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="99cfd-479">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="99cfd-479">Az.SignalR</span></span>
* <span data-ttu-id="99cfd-480">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="99cfd-480">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="99cfd-481">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="99cfd-481">Az.Sql</span></span>
* <span data-ttu-id="99cfd-482">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="99cfd-482">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="99cfd-483">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="99cfd-483">Az.Storage</span></span>
* <span data-ttu-id="99cfd-484">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="99cfd-484">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="99cfd-485">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="99cfd-485">New-AzStorageContext</span></span>
* <span data-ttu-id="99cfd-486">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="99cfd-486">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="99cfd-487">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="99cfd-487">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="99cfd-488">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="99cfd-488">Az.Websites</span></span>
* <span data-ttu-id="99cfd-489">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="99cfd-489">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="99cfd-490">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="99cfd-490">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="99cfd-491">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="99cfd-491">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="99cfd-492">Geral</span><span class="sxs-lookup"><span data-stu-id="99cfd-492">General</span></span>

- <span data-ttu-id="99cfd-493">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="99cfd-493">General Availability of Az Module</span></span>
- <span data-ttu-id="99cfd-494">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="99cfd-494">Online help for each module</span></span>
- <span data-ttu-id="99cfd-495">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="99cfd-495">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="99cfd-496">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="99cfd-496">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="99cfd-497">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="99cfd-497">Az.Accounts</span></span>
- <span data-ttu-id="99cfd-498">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="99cfd-498">Changed from Az.Profile</span></span>
- <span data-ttu-id="99cfd-499">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="99cfd-499">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="99cfd-500">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="99cfd-500">Az.ApiManagement</span></span>
- <span data-ttu-id="99cfd-501">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="99cfd-501">Fixes for #7002</span></span>
- <span data-ttu-id="99cfd-502">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="99cfd-502">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="99cfd-503">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="99cfd-503">Az.Batch</span></span>
- <span data-ttu-id="99cfd-504">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="99cfd-504">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="99cfd-505">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="99cfd-505">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="99cfd-506">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="99cfd-506">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="99cfd-507">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="99cfd-507">Az.Billing</span></span>
- <span data-ttu-id="99cfd-508">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="99cfd-508">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="99cfd-509">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="99cfd-509">Az.CognitivServices</span></span>
- <span data-ttu-id="99cfd-510">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="99cfd-510">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="99cfd-511">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="99cfd-511">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="99cfd-512">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="99cfd-512">Az.ContainerInstance</span></span>
- <span data-ttu-id="99cfd-513">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="99cfd-513">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="99cfd-514">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="99cfd-514">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="99cfd-515">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="99cfd-515">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="99cfd-516">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="99cfd-516">Az.DataLakeStore</span></span>
- <span data-ttu-id="99cfd-517">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="99cfd-517">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="99cfd-518">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="99cfd-518">Az.Monitor</span></span>
- <span data-ttu-id="99cfd-519">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="99cfd-519">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="99cfd-520">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="99cfd-520">Az.KeyVault</span></span>
- <span data-ttu-id="99cfd-521">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="99cfd-521">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="99cfd-522">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="99cfd-522">Az.MachineLearning</span></span>
- <span data-ttu-id="99cfd-523">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="99cfd-523">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="99cfd-524">Az.Media</span><span class="sxs-lookup"><span data-stu-id="99cfd-524">Az.Media</span></span>
- <span data-ttu-id="99cfd-525">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="99cfd-525">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="99cfd-526">Az.Network</span><span class="sxs-lookup"><span data-stu-id="99cfd-526">Az.Network</span></span>
<span data-ttu-id="99cfd-527">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="99cfd-527">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="99cfd-528">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="99cfd-528">New cmdlets added:</span></span>
        - <span data-ttu-id="99cfd-529">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="99cfd-529">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="99cfd-530">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="99cfd-530">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="99cfd-531">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="99cfd-531">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="99cfd-532">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="99cfd-532">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="99cfd-533">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="99cfd-533">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="99cfd-534">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="99cfd-534">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="99cfd-535">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="99cfd-535">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="99cfd-536">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="99cfd-536">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="99cfd-537">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="99cfd-537">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="99cfd-538">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="99cfd-538">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="99cfd-539">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="99cfd-539">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="99cfd-540">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="99cfd-540">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="99cfd-541">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="99cfd-541">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="99cfd-542">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="99cfd-542">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="99cfd-543">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="99cfd-543">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="99cfd-544">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="99cfd-544">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="99cfd-545">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="99cfd-545">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="99cfd-546">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="99cfd-546">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="99cfd-547">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="99cfd-547">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="99cfd-548">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="99cfd-548">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="99cfd-549">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="99cfd-549">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="99cfd-550">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="99cfd-550">Az.OperationalInsights</span></span>
- <span data-ttu-id="99cfd-551">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="99cfd-551">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="99cfd-552">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="99cfd-552">Az.Profile</span></span>
- <span data-ttu-id="99cfd-553">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="99cfd-553">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="99cfd-554">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="99cfd-554">Az.RecoveryServices</span></span>
- <span data-ttu-id="99cfd-555">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="99cfd-555">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="99cfd-556">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="99cfd-556">Az.Resources</span></span>
- <span data-ttu-id="99cfd-557">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="99cfd-557">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="99cfd-558">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="99cfd-558">Az.ServiceFabric</span></span>
- <span data-ttu-id="99cfd-559">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="99cfd-559">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="99cfd-560">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="99cfd-560">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="99cfd-561">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="99cfd-561">Az.SIgnalR</span></span>
- <span data-ttu-id="99cfd-562">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="99cfd-562">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="99cfd-563">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="99cfd-563">Az.Sql</span></span>
- <span data-ttu-id="99cfd-564">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="99cfd-564">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="99cfd-565">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="99cfd-565">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="99cfd-566">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="99cfd-566">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="99cfd-567">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="99cfd-567">Az.Storage</span></span>
- <span data-ttu-id="99cfd-568">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="99cfd-568">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="99cfd-569">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="99cfd-569">Az.Websites</span></span>
- <span data-ttu-id="99cfd-570">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="99cfd-570">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="99cfd-571">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="99cfd-571">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="99cfd-572">Geral</span><span class="sxs-lookup"><span data-stu-id="99cfd-572">General</span></span>

* <span data-ttu-id="99cfd-573">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="99cfd-573">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="99cfd-574">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="99cfd-574">Az.Compute</span></span>

* <span data-ttu-id="99cfd-575">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="99cfd-575">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="99cfd-576">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="99cfd-576">Az.DataLakeStore</span></span>

* <span data-ttu-id="99cfd-577">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="99cfd-577">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="99cfd-578">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="99cfd-578">Az.FrontDoor</span></span>

* <span data-ttu-id="99cfd-579">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="99cfd-579">Fixed some broken links</span></span>
    - <span data-ttu-id="99cfd-580">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="99cfd-580">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="99cfd-581">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="99cfd-581">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="99cfd-582">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="99cfd-582">Az.RecoveryServices</span></span>

* <span data-ttu-id="99cfd-583">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="99cfd-583">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="99cfd-584">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="99cfd-584">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="99cfd-585">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="99cfd-585">Az.Resources</span></span>

* <span data-ttu-id="99cfd-586">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="99cfd-586">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="99cfd-587">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="99cfd-587">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="99cfd-588">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="99cfd-588">Az.Sql</span></span>

* <span data-ttu-id="99cfd-589">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="99cfd-589">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="99cfd-590">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="99cfd-590">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="99cfd-591">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="99cfd-591">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="99cfd-592">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="99cfd-592">Az.Storage</span></span>

* <span data-ttu-id="99cfd-593">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="99cfd-593">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="99cfd-594">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="99cfd-594">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="99cfd-595">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="99cfd-595">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="99cfd-596">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="99cfd-596">Support Static Website configuration</span></span>
    - <span data-ttu-id="99cfd-597">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="99cfd-597">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="99cfd-598">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="99cfd-598">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="99cfd-599">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="99cfd-599">Az.Websites</span></span>

* <span data-ttu-id="99cfd-600">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="99cfd-600">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="99cfd-601">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="99cfd-601">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="99cfd-602">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="99cfd-602">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="99cfd-603">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="99cfd-603">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="99cfd-604">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="99cfd-604">Az.ApiManagement</span></span>
* <span data-ttu-id="99cfd-605">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="99cfd-605">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="99cfd-606">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="99cfd-606">Az.Automation</span></span>
* <span data-ttu-id="99cfd-607">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="99cfd-607">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="99cfd-608">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="99cfd-608">Added Update Management cmdlets</span></span>
* <span data-ttu-id="99cfd-609">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="99cfd-609">Added Source Control cmdlets</span></span>
* <span data-ttu-id="99cfd-610">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="99cfd-610">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="99cfd-611">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="99cfd-611">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="99cfd-612">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="99cfd-612">Az.Compute</span></span>
* <span data-ttu-id="99cfd-613">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="99cfd-613">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="99cfd-614">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="99cfd-614">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="99cfd-615">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="99cfd-615">Az.ContainerInstance</span></span>
* <span data-ttu-id="99cfd-616">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="99cfd-616">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="99cfd-617">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="99cfd-617">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="99cfd-618">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="99cfd-618">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="99cfd-619">Az.Network</span><span class="sxs-lookup"><span data-stu-id="99cfd-619">Az.Network</span></span>
* <span data-ttu-id="99cfd-620">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="99cfd-620">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="99cfd-621">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="99cfd-621">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="99cfd-622">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="99cfd-622">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="99cfd-623">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="99cfd-623">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="99cfd-624">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="99cfd-624">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="99cfd-625">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="99cfd-625">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="99cfd-626">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="99cfd-626">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="99cfd-627">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="99cfd-627">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="99cfd-628">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="99cfd-628">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="99cfd-629">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="99cfd-629">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="99cfd-630">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="99cfd-630">Az.Relay</span></span>
* <span data-ttu-id="99cfd-631">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="99cfd-631">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="99cfd-632">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="99cfd-632">Az.Resources</span></span>
* <span data-ttu-id="99cfd-633">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="99cfd-633">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="99cfd-634">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="99cfd-634">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="99cfd-635">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="99cfd-635">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="99cfd-636">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="99cfd-636">Az.ServiceFabric</span></span>
* <span data-ttu-id="99cfd-637">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="99cfd-637">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="99cfd-638">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="99cfd-638">Az.Sql</span></span>
* <span data-ttu-id="99cfd-639">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="99cfd-639">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="99cfd-640">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="99cfd-640">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="99cfd-641">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="99cfd-641">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="99cfd-642">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="99cfd-642">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="99cfd-643">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="99cfd-643">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="99cfd-644">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="99cfd-644">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="99cfd-645">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="99cfd-645">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="99cfd-646">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="99cfd-646">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="99cfd-647">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="99cfd-647">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="99cfd-648">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="99cfd-648">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="99cfd-649">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="99cfd-649">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="99cfd-650">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="99cfd-650">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="99cfd-651">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="99cfd-651">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="99cfd-652">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="99cfd-652">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="99cfd-653">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="99cfd-653">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="99cfd-654">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="99cfd-654">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="99cfd-655">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="99cfd-655">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="99cfd-656">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="99cfd-656">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="99cfd-657">Geral</span><span class="sxs-lookup"><span data-stu-id="99cfd-657">General</span></span>
* <span data-ttu-id="99cfd-658">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="99cfd-658">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="99cfd-659">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="99cfd-659">Az.Profile</span></span>
* <span data-ttu-id="99cfd-660">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="99cfd-660">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="99cfd-661">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="99cfd-661">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="99cfd-662">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="99cfd-662">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="99cfd-663">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="99cfd-663">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="99cfd-664">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="99cfd-664">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="99cfd-665">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="99cfd-665">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="99cfd-666">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="99cfd-666">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="99cfd-667">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="99cfd-667">Az.CognitiveServices</span></span>
* <span data-ttu-id="99cfd-668">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="99cfd-668">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="99cfd-669">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="99cfd-669">Az.Compute</span></span>
* <span data-ttu-id="99cfd-670">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="99cfd-670">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="99cfd-671">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="99cfd-671">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="99cfd-672">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="99cfd-672">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="99cfd-673">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="99cfd-673">Az.DataLakeStore</span></span>
* <span data-ttu-id="99cfd-674">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="99cfd-674">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="99cfd-675">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="99cfd-675">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="99cfd-676">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="99cfd-676">Az.Insights</span></span>
* <span data-ttu-id="99cfd-677">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="99cfd-677">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="99cfd-678">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="99cfd-678">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="99cfd-679">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="99cfd-679">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="99cfd-680">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="99cfd-680">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="99cfd-681">Az.Network</span><span class="sxs-lookup"><span data-stu-id="99cfd-681">Az.Network</span></span>
* <span data-ttu-id="99cfd-682">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="99cfd-682">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="99cfd-683">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="99cfd-683">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="99cfd-684">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="99cfd-684">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="99cfd-685">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="99cfd-685">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="99cfd-686">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="99cfd-686">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="99cfd-687">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="99cfd-687">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="99cfd-688">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="99cfd-688">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="99cfd-689">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="99cfd-689">Az.PolicyInsights</span></span>
* <span data-ttu-id="99cfd-690">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="99cfd-690">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="99cfd-691">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="99cfd-691">Az.Resources</span></span>
* <span data-ttu-id="99cfd-692">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="99cfd-692">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="99cfd-693">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="99cfd-693">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="99cfd-694">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="99cfd-694">Az.ServiceBus</span></span>
* <span data-ttu-id="99cfd-695">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="99cfd-695">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="99cfd-696">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="99cfd-696">Az.ServiceFabric</span></span>
* <span data-ttu-id="99cfd-697">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="99cfd-697">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="99cfd-698">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="99cfd-698">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="99cfd-699">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="99cfd-699">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="99cfd-700">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="99cfd-700">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="99cfd-701">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="99cfd-701">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="99cfd-702">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="99cfd-702">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="99cfd-703">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="99cfd-703">Az.Profile</span></span>
* <span data-ttu-id="99cfd-704">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="99cfd-704">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="99cfd-705">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="99cfd-705">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="99cfd-706">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="99cfd-706">Az.Compute</span></span>
* <span data-ttu-id="99cfd-707">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="99cfd-707">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="99cfd-708">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="99cfd-708">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="99cfd-709">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="99cfd-709">Az.DataLakeStore</span></span>
* <span data-ttu-id="99cfd-710">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="99cfd-710">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="99cfd-711">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="99cfd-711">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="99cfd-712">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="99cfd-712">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="99cfd-713">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="99cfd-713">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="99cfd-714">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="99cfd-714">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="99cfd-715">Az.Network</span><span class="sxs-lookup"><span data-stu-id="99cfd-715">Az.Network</span></span>
* <span data-ttu-id="99cfd-716">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="99cfd-716">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="99cfd-717">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="99cfd-717">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="99cfd-718">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="99cfd-718">Az.Resources</span></span>
* <span data-ttu-id="99cfd-719">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="99cfd-719">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="99cfd-720">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="99cfd-720">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="99cfd-721">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="99cfd-721">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="99cfd-722">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="99cfd-722">Azure.Storage</span></span>
* <span data-ttu-id="99cfd-723">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="99cfd-723">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="99cfd-724">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="99cfd-724">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="99cfd-725">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="99cfd-725">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="99cfd-726">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="99cfd-726">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="99cfd-727">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="99cfd-727">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="99cfd-728">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="99cfd-728">Az.CognitiveServices</span></span>
* <span data-ttu-id="99cfd-729">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="99cfd-729">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="99cfd-730">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="99cfd-730">Az.Compute</span></span>
* <span data-ttu-id="99cfd-731">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="99cfd-731">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="99cfd-732">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="99cfd-732">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="99cfd-733">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="99cfd-733">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="99cfd-734">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="99cfd-734">Az.DataFactoryV2</span></span>
* <span data-ttu-id="99cfd-735">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="99cfd-735">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="99cfd-736">Az.Network</span><span class="sxs-lookup"><span data-stu-id="99cfd-736">Az.Network</span></span>
* <span data-ttu-id="99cfd-737">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="99cfd-737">Added NetworkProfile functionality.</span></span> <span data-ttu-id="99cfd-738">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="99cfd-738">new cmdlets added</span></span>
    - <span data-ttu-id="99cfd-739">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="99cfd-739">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="99cfd-740">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="99cfd-740">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="99cfd-741">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="99cfd-741">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="99cfd-742">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="99cfd-742">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="99cfd-743">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="99cfd-743">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="99cfd-744">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="99cfd-744">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="99cfd-745">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="99cfd-745">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="99cfd-746">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="99cfd-746">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="99cfd-747">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="99cfd-747">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="99cfd-748">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="99cfd-748">Az.RedisCache</span></span>
* <span data-ttu-id="99cfd-749">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="99cfd-749">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="99cfd-750">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="99cfd-750">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="99cfd-751">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="99cfd-751">Az.Resources</span></span>
* <span data-ttu-id="99cfd-752">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="99cfd-752">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="99cfd-753">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="99cfd-753">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="99cfd-754">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="99cfd-754">Az.Sql</span></span>
* <span data-ttu-id="99cfd-755">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="99cfd-755">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="99cfd-756">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="99cfd-756">Az.Websites</span></span>
* <span data-ttu-id="99cfd-757">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="99cfd-757">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="99cfd-758">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="99cfd-758">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="99cfd-759">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="99cfd-759">0.2.0 - September 2018</span></span>
 <span data-ttu-id="99cfd-760">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="99cfd-760">Initial Release</span></span>