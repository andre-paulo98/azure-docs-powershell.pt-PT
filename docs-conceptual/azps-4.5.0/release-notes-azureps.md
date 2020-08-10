---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.openlocfilehash: 77cbbeb01f5c6fcbf0f61bfab3d3f63b74a53bc4
ms.sourcegitcommit: edfe63c6949cd59127028ac8a13bb4a8827d555c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/04/2020
ms.locfileid: "87566415"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="01b15-103">Notas de versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="01b15-103">Azure PowerShell release notes</span></span>

## <a name="450---august-2020"></a><span data-ttu-id="01b15-104">4.5.0 - Agosto de 2020</span><span class="sxs-lookup"><span data-stu-id="01b15-104">4.5.0 - August 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="01b15-105">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-105">Az.Accounts</span></span>
* <span data-ttu-id="01b15-106">"Connect-AzAccount" atualizado para aceitar o parâmetro "MaxContextPopulation" [#9865]</span><span class="sxs-lookup"><span data-stu-id="01b15-106">Updated 'Connect-AzAccount' to accept parameter 'MaxContextPopulation' [#9865]</span></span>
* <span data-ttu-id="01b15-107">Versão de SubscriptionClient atualizada para a de 2019-06-01 e apresentação de domínios de inquilino [#9838]</span><span class="sxs-lookup"><span data-stu-id="01b15-107">Updated SubscriptionClient version to 2019-06-01 and display tenant domains [#9838]</span></span>
* <span data-ttu-id="01b15-108">Inquilino principal suportado e informações do inquilino managedBy da subscrição</span><span class="sxs-lookup"><span data-stu-id="01b15-108">Supported home tenant and managedBy tenant information of subscription</span></span>
* <span data-ttu-id="01b15-109">Nome do módulo corrigido, informações da versão nos dados telemétricos</span><span class="sxs-lookup"><span data-stu-id="01b15-109">Corrected module name, version info in telemetry data</span></span>
* <span data-ttu-id="01b15-110">SqlDatabaseDnsSuffix e ServiceManagementUrl ajustados se o ponto final dos metadados do ambiente devolverem valores incompatíveis</span><span class="sxs-lookup"><span data-stu-id="01b15-110">Adjusted SqlDatabaseDnsSuffix and ServiceManagementUrl if environment metadata endpoint returns incompatible value</span></span>

#### <a name="azaks"></a><span data-ttu-id="01b15-111">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="01b15-111">Az.Aks</span></span>
* <span data-ttu-id="01b15-112">"ClientIdAndSecret" removido para "ServicePrincipalIdAndSecret" e "ClientIdAndSecret" definido como um alias [#12381].</span><span class="sxs-lookup"><span data-stu-id="01b15-112">Removed 'ClientIdAndSecret' to 'ServicePrincipalIdAndSecret' and set 'ClientIdAndSecret' as an alias [#12381].</span></span>
* <span data-ttu-id="01b15-113">"Get-AzAks"/"New-AzAks"/"Remove-AzAks"/"Set-AzAks" removidos para "Get-AzAksCluster"/"New-AzAksCluster"/"Remove-AzAksCluster"/"Set-AzAksCluster" e definição dos valores originais como alias [#12373].</span><span class="sxs-lookup"><span data-stu-id="01b15-113">Removed 'Get-AzAks'/'New-AzAks'/'Remove-AzAks'/'Set-AzAks' to 'Get-AzAksCluster'/'New-AzAksCluster'/'Remove-AzAksCluster'/'Set-AzAksCluster' and set the original ones as alias [#12373].</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="01b15-114">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="01b15-114">Az.ApiManagement</span></span>
* <span data-ttu-id="01b15-115">Novo cmdlet "Add-AzApiManagementApiToGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="01b15-115">Added new 'Add-AzApiManagementApiToGateway' cmdlet.</span></span>
* <span data-ttu-id="01b15-116">Novo cmdlet "Get-AzApiManagementGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="01b15-116">Added new 'Get-AzApiManagementGateway' cmdlet.</span></span>
* <span data-ttu-id="01b15-117">Novo cmdlet "Get-AzApiManagementGatewayHostnameConfiguration" adicionado.</span><span class="sxs-lookup"><span data-stu-id="01b15-117">Added new 'Get-AzApiManagementGatewayHostnameConfiguration' cmdlet.</span></span>
* <span data-ttu-id="01b15-118">Novo cmdlet "Get-AzApiManagementGatewayKey" adicionado.</span><span class="sxs-lookup"><span data-stu-id="01b15-118">Added new 'Get-AzApiManagementGatewayKey' cmdlet.</span></span>
* <span data-ttu-id="01b15-119">Novo cmdlet "New-AzApiManagementGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="01b15-119">Added new 'New-AzApiManagementGateway' cmdlet.</span></span>
* <span data-ttu-id="01b15-120">Novo cmdlet "New-AzApiManagementGatewayHostnameConfiguration" adicionado.</span><span class="sxs-lookup"><span data-stu-id="01b15-120">Added new 'New-AzApiManagementGatewayHostnameConfiguration' cmdlet.</span></span>
* <span data-ttu-id="01b15-121">Novo cmdlet "New-AzApiManagementResourceLocationObject" adicionado.</span><span class="sxs-lookup"><span data-stu-id="01b15-121">Added new 'New-AzApiManagementResourceLocationObject' cmdlet.</span></span>
* <span data-ttu-id="01b15-122">Novo cmdlet "Remove-AzApiManagementApiFromGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="01b15-122">Added new 'Remove-AzApiManagementApiFromGateway' cmdlet.</span></span>
* <span data-ttu-id="01b15-123">Novo cmdlet "Remove-AzApiManagementGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="01b15-123">Added new 'Remove-AzApiManagementGateway' cmdlet.</span></span>
* <span data-ttu-id="01b15-124">Novo cmdlet "Remove-AzApiManagementGatewayHostnameConfiguration" adicionado.</span><span class="sxs-lookup"><span data-stu-id="01b15-124">Added new 'Remove-AzApiManagementGatewayHostnameConfiguration' cmdlet.</span></span>
* <span data-ttu-id="01b15-125">Novo cmdlet "Update-AzApiManagementGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="01b15-125">Added new 'Update-AzApiManagementGateway' cmdlet.</span></span>
* <span data-ttu-id="01b15-126">Foi adicionado um novo parâmetro [-GatewayId] opcional ao cmdlet "Get-AzApiManagementApi".</span><span class="sxs-lookup"><span data-stu-id="01b15-126">Added new optional [-GatewayId] parameter to the 'Get-AzApiManagementApi' cmdlet.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="01b15-127">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="01b15-127">Az.CognitiveServices</span></span>
* <span data-ttu-id="01b15-128">Utilizado "Deny" especificamente como ação NetworkRules predefinida.</span><span class="sxs-lookup"><span data-stu-id="01b15-128">Used 'Deny' specifically as NetworkRules default action.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="01b15-129">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="01b15-129">Az.FrontDoor</span></span>
* <span data-ttu-id="01b15-130">Foi resolvido um problema em que é gerada uma exceção quando Enum.Parse tenta limitar um valor nulo a um valor de enumeração Enabled ou Disabled [#12344]</span><span class="sxs-lookup"><span data-stu-id="01b15-130">Fixed an issue where an exception is being thrown when Enum.Parse tries to coerce a null value to an Enabled or Disabled enum values [#12344]</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="01b15-131">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="01b15-131">Az.HDInsight</span></span>
* <span data-ttu-id="01b15-132">É suportada a criação de clusters com encriptação na funcionalidade de trânsito.</span><span class="sxs-lookup"><span data-stu-id="01b15-132">Supported creating cluster with encryption in transit feature.</span></span>
    - <span data-ttu-id="01b15-133">Foi adicionado o novo parâmetro "EncryptionInTransit" ao cmdlet "New-AzHDInsightCluster"</span><span class="sxs-lookup"><span data-stu-id="01b15-133">Add new parameter 'EncryptionInTransit' to the cmdlet 'New-AzHDInsightCluster'</span></span>
    - <span data-ttu-id="01b15-134">Foi adicionado o novo parâmetro "EncryptionInTransit" ao cmdlet "New-AzHDInsightClusterConfig"</span><span class="sxs-lookup"><span data-stu-id="01b15-134">Add new parameter 'EncryptionInTransit' to the cmdlet 'New-AzHDInsightClusterConfig'</span></span>
* <span data-ttu-id="01b15-135">É suportada a criação de clusters com a funcionalidade de ligação privada:</span><span class="sxs-lookup"><span data-stu-id="01b15-135">Supported creating cluster with private link feature:</span></span>
    - <span data-ttu-id="01b15-136">Novos parâmetros "PublicNetworkAccessType" e "OutboundPublicNetworkAccessType" adicionados ao cmdlet "New-AzHDInsightCluster"</span><span class="sxs-lookup"><span data-stu-id="01b15-136">Add new parameter 'PublicNetworkAccessType' and 'OutboundPublicNetworkAccessType' to the cmdlet 'New-AzHDInsightCluster'</span></span>
    - <span data-ttu-id="01b15-137">Novos parâmetros "PublicNetworkAccessType" e "OutboundPublicNetworkAccessType" adicionados ao cmdlet "New-AzHDInsightClusterConfig"</span><span class="sxs-lookup"><span data-stu-id="01b15-137">Add new parameter 'PublicNetworkAccessType' and 'OutboundPublicNetworkAccessType' to the cmdlet 'New-AzHDInsightClusterConfig'</span></span>
* <span data-ttu-id="01b15-138">Informações de rede virtual devolvidas ao chamar "New-AzHDInsightCluster" ou "Get-AzHDInsightCluster"</span><span class="sxs-lookup"><span data-stu-id="01b15-138">Returned virtual network information when calling 'New-AzHDInsightCluster' or 'Get-AzHDInsightCluster'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-139">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-139">Az.Network</span></span>
* <span data-ttu-id="01b15-140">Adição de suporte para o parâmetro AddressPrefixType a "Remove-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="01b15-140">Added support for AddressPrefixType parameter to 'Remove-AzExpressRouteCircuitConnectionConfig'</span></span>
* <span data-ttu-id="01b15-141">Alterações não interruptivas adicionadas: Funcionalidade PeerAddressType para Peering Privado em "Remove-AzExpressRouteCircutPeeringConfig".</span><span class="sxs-lookup"><span data-stu-id="01b15-141">Added non-breaking changes: PeerAddressType functionality for Private Peering in 'Remove-AzExpressRouteCircutPeeringConfig'.</span></span>
* <span data-ttu-id="01b15-142">Código alterado para ignorar caso dos parâmetros AddressPrefixType e PeerAddressType.</span><span class="sxs-lookup"><span data-stu-id="01b15-142">Code changed to ignore case for AddressPrefixType and PeerAddressType parameter.</span></span>
* <span data-ttu-id="01b15-143">Foi modificada a mensagem de aviso de "New-AzLoadBalancerFrontendIpConfig", "New-AzPublicIpAddress" e "New-AzPublicIpPrefix".</span><span class="sxs-lookup"><span data-stu-id="01b15-143">Modified the warning message for 'New-AzLoadBalancerFrontendIpConfig', 'New-AzPublicIpAddress' and 'New-AzPublicIpPrefix'.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="01b15-144">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-144">Az.OperationalInsights</span></span>
* <span data-ttu-id="01b15-145">Opção "-ForceDelete" adicionada para "Remove-AzOperationalInsightsworkspace"</span><span class="sxs-lookup"><span data-stu-id="01b15-145">Added '-ForceDelete' option for 'Remove-AzOperationalInsightsworkspace'</span></span>
* <span data-ttu-id="01b15-146">Novo cmdlet "Get-AzOperationalInsightsDeletedWorkspace" adicionado</span><span class="sxs-lookup"><span data-stu-id="01b15-146">Added new cmdlet 'Get-AzOperationalInsightsDeletedWorkspace'</span></span>
* <span data-ttu-id="01b15-147">Novo cmdlet "Restore-AzOperationalInsightsWorkspace" adicionado</span><span class="sxs-lookup"><span data-stu-id="01b15-147">Added new cmdlet 'Restore-AzOperationalInsightsWorkspace'</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-148">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-148">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-149">Experiência de deteção de contentores/itens do Azure Backup melhorada.</span><span class="sxs-lookup"><span data-stu-id="01b15-149">Improved the Azure Backup container/item discovery experience.</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-150">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-150">Az.Resources</span></span>
* <span data-ttu-id="01b15-151">Propriedades "Condition", "ConditionVersion" e "Description" adicionadas a "New-AzRoleAssignment"</span><span class="sxs-lookup"><span data-stu-id="01b15-151">Added properties 'Condition', 'ConditionVersion' and 'Description' to 'New-AzRoleAssignment'</span></span>
    - <span data-ttu-id="01b15-152">Isto incluiu todas as alterações relevantes aos modelos de dados</span><span class="sxs-lookup"><span data-stu-id="01b15-152">This included all the relevant changes to the data models</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-153">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-153">Az.Sql</span></span>
* <span data-ttu-id="01b15-154">Foi corrigido o potencial erro de nome do servidor não sensível a maiúsculas e minúsculas em "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="01b15-154">Fixed potential server name case insensitive error in 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="01b15-155">Foi corrigido o erro em que era devolvido um nome de base de dados incorreto numa base de dados existente em "New-AzSqlDatabaseSecondary"</span><span class="sxs-lookup"><span data-stu-id="01b15-155">Fixed wrong database name returned on existing database error in 'New-AzSqlDatabaseSecondary'</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-156">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-156">Az.Storage</span></span>
* <span data-ttu-id="01b15-157">Criação de tokens de SAS de contentores/blobs suportada com nova permissão x,t</span><span class="sxs-lookup"><span data-stu-id="01b15-157">Supported create container/blob Sas token with new permission x,t</span></span>
    -  <span data-ttu-id="01b15-158">"New-AzStorageBlobSASToken"</span><span class="sxs-lookup"><span data-stu-id="01b15-158">'New-AzStorageBlobSASToken'</span></span>
    -  <span data-ttu-id="01b15-159">"New-AzStorageContainerSASToken"</span><span class="sxs-lookup"><span data-stu-id="01b15-159">'New-AzStorageContainerSASToken'</span></span>
* <span data-ttu-id="01b15-160">Criação de tokens de SAS de contas suportada com nova permissão x,t,f</span><span class="sxs-lookup"><span data-stu-id="01b15-160">Supported create account Sas token with new permission x,t,f</span></span>
    -  <span data-ttu-id="01b15-161">"New-AzStorageAccountSASToken"</span><span class="sxs-lookup"><span data-stu-id="01b15-161">'New-AzStorageAccountSASToken'</span></span>
* <span data-ttu-id="01b15-162">Obtenção da utilização de partilha de ficheiros única suportada</span><span class="sxs-lookup"><span data-stu-id="01b15-162">Supported get single file share usage</span></span>
    - <span data-ttu-id="01b15-163">"Get-AzRmStorageShare"</span><span class="sxs-lookup"><span data-stu-id="01b15-163">'Get-AzRmStorageShare'</span></span>

## <a name="440---july-2020"></a><span data-ttu-id="01b15-164">4.4.0 - Julho de 2020</span><span class="sxs-lookup"><span data-stu-id="01b15-164">4.4.0 - July 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="01b15-165">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-165">Az.Accounts</span></span>
* <span data-ttu-id="01b15-166">Adição do novo cmdlet "Invoke-AzRestMethod"</span><span class="sxs-lookup"><span data-stu-id="01b15-166">Added new cmdlet 'Invoke-AzRestMethod'</span></span>
* <span data-ttu-id="01b15-167">Correção de um problema que pode causar erros de autenticação em cenários de vários processos, tais como executar vários cmdlets do Azure PowerShell utilizando "Start-Job" [#9448]</span><span class="sxs-lookup"><span data-stu-id="01b15-167">Fixed an issue that may cause authentication errors in multi-process scenarios such as running multiple Azure PowerShell cmdlets using 'Start-Job' [#9448]</span></span>

#### <a name="azaks"></a><span data-ttu-id="01b15-168">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="01b15-168">Az.Aks</span></span>
* <span data-ttu-id="01b15-169">Correção do erro "Get-AzAks" uma vez que não recebe todos os clusters [#12296]</span><span class="sxs-lookup"><span data-stu-id="01b15-169">Fixed bug 'Get-AzAks' doesn't get all clusters [#12296]</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="01b15-170">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="01b15-170">Az.AnalysisServices</span></span>
* <span data-ttu-id="01b15-171">Remoção da referência do projeto para Autenticação</span><span class="sxs-lookup"><span data-stu-id="01b15-171">Removed project reference to Authentication</span></span>

#### <a name="azautomation"></a><span data-ttu-id="01b15-172">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="01b15-172">Az.Automation</span></span>
* <span data-ttu-id="01b15-173">Correção do problema em que a cadeia com chars de fuga não pode ser convertida num objeto json.</span><span class="sxs-lookup"><span data-stu-id="01b15-173">Fixed the issue that string with escape chars cannot be converted into json object.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-174">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-174">Az.Compute</span></span>
* <span data-ttu-id="01b15-175">Adição do aviso ao utilizar "New-AzVmss" sem a versão de imagem "mais recente"</span><span class="sxs-lookup"><span data-stu-id="01b15-175">Added warning when using 'New-AzVmss' without 'latest' image version</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="01b15-176">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="01b15-176">Az.DataFactory</span></span>
* <span data-ttu-id="01b15-177">Adição de parâmetros globais ao Data Factory.</span><span class="sxs-lookup"><span data-stu-id="01b15-177">Added global parameters to Data Factory.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="01b15-178">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="01b15-178">Az.EventGrid</span></span>
* <span data-ttu-id="01b15-179">Atualização para utilizar a versão de API 2020-06-01.</span><span class="sxs-lookup"><span data-stu-id="01b15-179">Updated to use the 2020-06-01 API version.</span></span>
* <span data-ttu-id="01b15-180">Novas funcionalidades adicionadas:</span><span class="sxs-lookup"><span data-stu-id="01b15-180">Added new features:</span></span>
    - <span data-ttu-id="01b15-181">Mapeamento de entrada</span><span class="sxs-lookup"><span data-stu-id="01b15-181">Input mapping</span></span>
    - <span data-ttu-id="01b15-182">Esquema de Entrega de Eventos</span><span class="sxs-lookup"><span data-stu-id="01b15-182">Event Delivery Schema</span></span>
    - <span data-ttu-id="01b15-183">Ligação Privada</span><span class="sxs-lookup"><span data-stu-id="01b15-183">Private Link</span></span>
    - <span data-ttu-id="01b15-184">Esquema de Eventos na Cloud V10</span><span class="sxs-lookup"><span data-stu-id="01b15-184">Cloud Event V10 Schema</span></span>
    - <span data-ttu-id="01b15-185">Tópico do Service Bus como Destino</span><span class="sxs-lookup"><span data-stu-id="01b15-185">Service Bus Topic As Destination</span></span>
    - <span data-ttu-id="01b15-186">Função do Azure como Destino</span><span class="sxs-lookup"><span data-stu-id="01b15-186">Azure Function As Destination</span></span>
    - <span data-ttu-id="01b15-187">Criação de batches do WebHook</span><span class="sxs-lookup"><span data-stu-id="01b15-187">WebHook Batching</span></span>
    - <span data-ttu-id="01b15-188">Webhook seguro (suporte de AAD)</span><span class="sxs-lookup"><span data-stu-id="01b15-188">Secure webhook (AAD support)</span></span>
    - <span data-ttu-id="01b15-189">IpFiltering</span><span class="sxs-lookup"><span data-stu-id="01b15-189">IpFiltering</span></span>
* <span data-ttu-id="01b15-190">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="01b15-190">Updated cmdlets:</span></span>
    - <span data-ttu-id="01b15-191">"New-AzEventGridSubscription"/"Update-AzEventGridSubscription":</span><span class="sxs-lookup"><span data-stu-id="01b15-191">'New-AzEventGridSubscription'/'Update-AzEventGridSubscription':</span></span>
        - <span data-ttu-id="01b15-192">Adicionar novos parâmetros opcionais para suportar a criação de batches do webhook.</span><span class="sxs-lookup"><span data-stu-id="01b15-192">Add new optional parameters to support webhook batching.</span></span>
        - <span data-ttu-id="01b15-193">Adicionar novos parâmetros opcionais para suportar o webhook seguro através do AAD.</span><span class="sxs-lookup"><span data-stu-id="01b15-193">Add new optional parameters to support secured webhook using AAD.</span></span>
        - <span data-ttu-id="01b15-194">Adicionar uma nova enumeração para o parâmetro EndpointType para suportar a função do Azure e o tópico do Service Bus enquanto novos destinos.</span><span class="sxs-lookup"><span data-stu-id="01b15-194">Add new enum for EndpointType parameter to support azure function and service bus topic as new destinations.</span></span>
        - <span data-ttu-id="01b15-195">Adicionar novo parâmetro opcional para o esquema de entrega.</span><span class="sxs-lookup"><span data-stu-id="01b15-195">Add new optional parameter for delivery schema.</span></span>
    - <span data-ttu-id="01b15-196">"New-AzEventGridTopic"/"Update-AzEventGridTopic" e "New-AzEventGridDomain"/"Update-AzEventGridDomain":</span><span class="sxs-lookup"><span data-stu-id="01b15-196">'New-AzEventGridTopic'/'Update-AzEventGridTopic' and 'New-AzEventGridDomain'/'Update-AzEventGridDomain':</span></span>
        - <span data-ttu-id="01b15-197">Adicionar novos parâmetros opcionais para suportar IpFiltering.</span><span class="sxs-lookup"><span data-stu-id="01b15-197">Add new optional parameters to support IpFiltering.</span></span>
    - <span data-ttu-id="01b15-198">"New-AzEventGridTopic"/"New-AzEventGridDomain":</span><span class="sxs-lookup"><span data-stu-id="01b15-198">'New-AzEventGridTopic'/'New-AzEventGridDomain':</span></span>
        - <span data-ttu-id="01b15-199">Adicionar novos parâmetros opcionais para suportar o Mapeamento de entrada.</span><span class="sxs-lookup"><span data-stu-id="01b15-199">Add new optional parameters to support Input mapping.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="01b15-200">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="01b15-200">Az.FrontDoor</span></span>
* <span data-ttu-id="01b15-201">Módulo atualizado para utilizar a API 2020-05-01</span><span class="sxs-lookup"><span data-stu-id="01b15-201">Updated module to use API 2020-05-01</span></span>
* <span data-ttu-id="01b15-202">Adição de suporte do Private Link para recursos de Armazenamento, Cofre de chaves e Serviço de Aplicações Web</span><span class="sxs-lookup"><span data-stu-id="01b15-202">Added Private link support for Storage, Keyvault and Web App Service resources</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="01b15-203">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="01b15-203">Az.HDInsight</span></span>
* <span data-ttu-id="01b15-204">Suporte para a criação de cluster com armazenamento ADLSGen1/2 em clouds nacionais.</span><span class="sxs-lookup"><span data-stu-id="01b15-204">Supported creating cluster with ADLSGen1/2 storage in national clouds.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="01b15-205">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="01b15-205">Az.Monitor</span></span>
* <span data-ttu-id="01b15-206">Correção do erro em "Get-AzDiagnosticSetting" quando as métricas ou registos são nulos [#12272]</span><span class="sxs-lookup"><span data-stu-id="01b15-206">Fixed bug for 'Get-AzDiagnosticSetting' when metrics or logs are null [#12272]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-207">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-207">Az.Network</span></span>
* <span data-ttu-id="01b15-208">Correção da troca de parâmetros na ligação VWan HubVnet</span><span class="sxs-lookup"><span data-stu-id="01b15-208">Fixed parameters swap in VWan HubVnet connection</span></span>
* <span data-ttu-id="01b15-209">Adição de novos cmdlets para Sites de Aplicações Virtuais da Rede Azure</span><span class="sxs-lookup"><span data-stu-id="01b15-209">Added new cmdlets for Azure Network Virtual Appliance Sites</span></span>
    - <span data-ttu-id="01b15-210">"Get-AzVirtualApplianceSite"</span><span class="sxs-lookup"><span data-stu-id="01b15-210">'Get-AzVirtualApplianceSite'</span></span>
    - <span data-ttu-id="01b15-211">"New-AzVirtualApplianceSite"</span><span class="sxs-lookup"><span data-stu-id="01b15-211">'New-AzVirtualApplianceSite'</span></span>
    - <span data-ttu-id="01b15-212">"Remove-AzVirtualApplianceSite"</span><span class="sxs-lookup"><span data-stu-id="01b15-212">'Remove-AzVirtualApplianceSite'</span></span>
    - <span data-ttu-id="01b15-213">"Update-AzVirtualApplianceSite"</span><span class="sxs-lookup"><span data-stu-id="01b15-213">'Update-AzVirtualApplianceSite'</span></span>
    - <span data-ttu-id="01b15-214">"New-AzOffice365PolicyProperty"</span><span class="sxs-lookup"><span data-stu-id="01b15-214">'New-AzOffice365PolicyProperty'</span></span>
* <span data-ttu-id="01b15-215">Adição de novos cmdlets para Aplicações Virtuais da Rede Azure</span><span class="sxs-lookup"><span data-stu-id="01b15-215">Added new cmdlets for Azure Network Virtual Appliance</span></span>
    - <span data-ttu-id="01b15-216">"Get-AzNetworkVirtualAppliance"</span><span class="sxs-lookup"><span data-stu-id="01b15-216">'Get-AzNetworkVirtualAppliance'</span></span>
    - <span data-ttu-id="01b15-217">"New-AzNetworkVirtualAppliance"</span><span class="sxs-lookup"><span data-stu-id="01b15-217">'New-AzNetworkVirtualAppliance'</span></span>
    - <span data-ttu-id="01b15-218">"Remove-AzNetworkVirtualAppliance"</span><span class="sxs-lookup"><span data-stu-id="01b15-218">'Remove-AzNetworkVirtualAppliance'</span></span>
    - <span data-ttu-id="01b15-219">"Update-AzNetworkVirtualAppliance"</span><span class="sxs-lookup"><span data-stu-id="01b15-219">'Update-AzNetworkVirtualAppliance'</span></span>
    - <span data-ttu-id="01b15-220">"Get-AzNetworkVirtualApplianceSku"</span><span class="sxs-lookup"><span data-stu-id="01b15-220">'Get-AzNetworkVirtualApplianceSku'</span></span>
    - <span data-ttu-id="01b15-221">"New-AzVirtualApplianceSkuProperty"</span><span class="sxs-lookup"><span data-stu-id="01b15-221">'New-AzVirtualApplianceSkuProperty'</span></span>
* <span data-ttu-id="01b15-222">Gateway de Aplicação integrado para Cmdlets Comuns do Private Link</span><span class="sxs-lookup"><span data-stu-id="01b15-222">Onboarded Application Gateway to Private Link Common Cmdlets</span></span>
* <span data-ttu-id="01b15-223">StorageSync integrado para Cmdlets Comuns do Private Link</span><span class="sxs-lookup"><span data-stu-id="01b15-223">Onboarded StorageSync to Private Link Common Cmdlets</span></span>
* <span data-ttu-id="01b15-224">SignalR integrado para Cmdlets Comuns do Private Link</span><span class="sxs-lookup"><span data-stu-id="01b15-224">Onboarded SignalR to Private Link Common Cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-225">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-225">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-226">Remoção da referência do projeto para Autenticação</span><span class="sxs-lookup"><span data-stu-id="01b15-226">Removed project reference to Authentication</span></span>
* <span data-ttu-id="01b15-227">Os cmdlets afinados do Azure Backup ajudam o texto a ser mais preciso.</span><span class="sxs-lookup"><span data-stu-id="01b15-227">Azure Backup tuned cmdlets help text to be more accurate.</span></span>
* <span data-ttu-id="01b15-228">O Azure Backup adicionou suporte para obter tarefas de agentes MAB através do cmdlet "Get-AzRecoveryServicesBackupJob".</span><span class="sxs-lookup"><span data-stu-id="01b15-228">Azure Backup added support for fetching MAB agent jobs using 'Get-AzRecoveryServicesBackupJob' cmdlet.</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-229">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-229">Az.Resources</span></span>
* <span data-ttu-id="01b15-230">Atualização de "Save-AzResourceGroupDeploymentTemplate" para utilizar o SDK.</span><span class="sxs-lookup"><span data-stu-id="01b15-230">Updated 'Save-AzResourceGroupDeploymentTemplate' to use the SDK.</span></span>
* <span data-ttu-id="01b15-231">Adição do cmdlet "Unregister-AzResourceProvider".</span><span class="sxs-lookup"><span data-stu-id="01b15-231">Added 'Unregister-AzResourceProvider' cmdlet.</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-232">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-232">Az.Sql</span></span>
* <span data-ttu-id="01b15-233">Adição de suporte para o Principal de serviço e utilizadores convidados no cmdlet Set-AzSqlInstanceActiveDirectoryAdministrator</span><span class="sxs-lookup"><span data-stu-id="01b15-233">Added support for Service principal and guest users in Set-AzSqlInstanceActiveDirectoryAdministrator cmdlet'</span></span>
* <span data-ttu-id="01b15-234">Correção de um erro em cmdlets de Classificação de Dados.</span><span class="sxs-lookup"><span data-stu-id="01b15-234">Fixed a bug in Data Classification cmdlets.'</span></span>
* <span data-ttu-id="01b15-235">Adição de suporte para a ativação pós-falha do Azure SQL Managed Instance: "Invoke-AzSqlInstanceFailover"</span><span class="sxs-lookup"><span data-stu-id="01b15-235">Added support for Azure SQL Managed Instance failover: 'Invoke-AzSqlInstanceFailover'</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-236">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-236">Az.Storage</span></span>
* <span data-ttu-id="01b15-237">Correção do erro de que o UserAgent não é adicionado para alguns cmdlets do plano de dados.</span><span class="sxs-lookup"><span data-stu-id="01b15-237">Fixed the issue that UserAgent is not added for some data plane cmdlets.</span></span>
* <span data-ttu-id="01b15-238">Suporte para a criação/atualização da Conta de armazenamento com MinimumTlsVersion e AllowBlobPublicAccess</span><span class="sxs-lookup"><span data-stu-id="01b15-238">Supported create/update Storage account with MinimumTlsVersion and AllowBlobPublicAccess</span></span>
    -  <span data-ttu-id="01b15-239">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="01b15-239">'New-AzStorageAccount'</span></span>
    -  <span data-ttu-id="01b15-240">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="01b15-240">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="01b15-241">Suporte para Permitir/desativar o controlo de versões no Serviço Blob de uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="01b15-241">Support enable/disable versioning on Blob Service of a Storage account</span></span>
    - <span data-ttu-id="01b15-242">"Update-AzStorageBlobServiceProperty"</span><span class="sxs-lookup"><span data-stu-id="01b15-242">'Update-AzStorageBlobServiceProperty'</span></span>
* <span data-ttu-id="01b15-243">Suporte para a lista de blobs com versões de blobs</span><span class="sxs-lookup"><span data-stu-id="01b15-243">Support list blobs with blob versions</span></span>
    - <span data-ttu-id="01b15-244">"Get-AzStorageBlob"</span><span class="sxs-lookup"><span data-stu-id="01b15-244">'Get-AzStorageBlob'</span></span>
* <span data-ttu-id="01b15-245">Suporte para obter/remover instantâneo de blob único ou versão do blob</span><span class="sxs-lookup"><span data-stu-id="01b15-245">Support get/remove single blob snapshot or blob version</span></span>
    - <span data-ttu-id="01b15-246">"Get-AzStorageBlob"</span><span class="sxs-lookup"><span data-stu-id="01b15-246">'Get-AzStorageBlob'</span></span>
    - <span data-ttu-id="01b15-247">"Remove-AzStorageBlob"</span><span class="sxs-lookup"><span data-stu-id="01b15-247">'Remove-AzStorageBlob'</span></span>
* <span data-ttu-id="01b15-248">Suporte para pipeline a partir do objeto de blob gerado a partir de Azure.Storage.Blobs V12</span><span class="sxs-lookup"><span data-stu-id="01b15-248">Support pipeline from blob object generated from Azure.Storage.Blobs V12</span></span>
    - <span data-ttu-id="01b15-249">"Get-AzStorageBlobContent"</span><span class="sxs-lookup"><span data-stu-id="01b15-249">'Get-AzStorageBlobContent'</span></span>
    - <span data-ttu-id="01b15-250">"New-AzStorageBlobSASToken"</span><span class="sxs-lookup"><span data-stu-id="01b15-250">'New-AzStorageBlobSASToken'</span></span>
    - <span data-ttu-id="01b15-251">"Remove-AzStorageBlob"</span><span class="sxs-lookup"><span data-stu-id="01b15-251">'Remove-AzStorageBlob'</span></span>
    - <span data-ttu-id="01b15-252">"Set-AzStorageBlobContent"</span><span class="sxs-lookup"><span data-stu-id="01b15-252">'Set-AzStorageBlobContent'</span></span>
    - <span data-ttu-id="01b15-253">"Start-AzStorageBlobCopy"</span><span class="sxs-lookup"><span data-stu-id="01b15-253">'Start-AzStorageBlobCopy'</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="01b15-254">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="01b15-254">Az.StorageSync</span></span>
* <span data-ttu-id="01b15-255">Adição de uma nova versão StorageSync SDK para ApiVersion 2020-03-01</span><span class="sxs-lookup"><span data-stu-id="01b15-255">Added a new version StorageSync SDK targeting ApiVersion 2020-03-01</span></span>
* <span data-ttu-id="01b15-256">Adição de cmdlet do Serviço de Sincronização de Armazenamento de Atualização</span><span class="sxs-lookup"><span data-stu-id="01b15-256">Added Update Storage Sync Service cmdlet</span></span>
    - <span data-ttu-id="01b15-257">"Set-AzStorageSyncService"</span><span class="sxs-lookup"><span data-stu-id="01b15-257">'Set-AzStorageSyncService'</span></span>
* <span data-ttu-id="01b15-258">Adição de IncomingTrafficPolicy e PrivateEndpointConnections para cmdlets StorageSyncService.</span><span class="sxs-lookup"><span data-stu-id="01b15-258">Added IncomingTrafficPolicy and PrivateEndpointConnections to StorageSyncService cmdlets.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="01b15-259">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-259">Az.Websites</span></span>
* <span data-ttu-id="01b15-260">Adição de suporte para a realização de operações para Slots em grupos de recursos diferentes do Plano do Serviço de Aplicações</span><span class="sxs-lookup"><span data-stu-id="01b15-260">Added support to perform operations for Slots not in the same resource group as the App Service Plan</span></span>

## <a name="430---june-2020"></a><span data-ttu-id="01b15-261">4.3.0 - Junho de 2020</span><span class="sxs-lookup"><span data-stu-id="01b15-261">4.3.0 - June 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="01b15-262">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-262">Az.Accounts</span></span>
* <span data-ttu-id="01b15-263">Suporte para a deteção da definição do ambiente por predefinição e adição de ambiente através de "Add-AzEnvironment"</span><span class="sxs-lookup"><span data-stu-id="01b15-263">Supported discovering environment setting by default and adding environment via 'Add-AzEnvironment'</span></span>
* <span data-ttu-id="01b15-264">Atualizar assemblagens pré-carregadas [#12024], [#11976]</span><span class="sxs-lookup"><span data-stu-id="01b15-264">Update preloaded assemblies [#12024], [#11976]</span></span>
* <span data-ttu-id="01b15-265">Atualização da assemblagem Azure.Core</span><span class="sxs-lookup"><span data-stu-id="01b15-265">Updated Azure.Core assembly</span></span>
* <span data-ttu-id="01b15-266">Correção de um problema que pode provocar a falha de "Connect-AzAccount" numa execução de múltiplos threads [#11201]</span><span class="sxs-lookup"><span data-stu-id="01b15-266">Fixed an issue that may cause 'Connect-AzAccount' to fail in multi-threaded execution [#11201]</span></span>

#### <a name="azaks"></a><span data-ttu-id="01b15-267">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="01b15-267">Az.Aks</span></span>
* <span data-ttu-id="01b15-268">Substituição da utilização da [API AccessProfile](https://docs.microsoft.com/rest/api/aks/managedclusters/getaccessprofile) antiga por chamadas para as APIs [ListClusterAdmin](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusteradmincredentials) e [ListClusterUser](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusterusercredentials)</span><span class="sxs-lookup"><span data-stu-id="01b15-268">Replaced usage of old [AccessProfile API](https://docs.microsoft.com/rest/api/aks/managedclusters/getaccessprofile) with calls to [ListClusterAdmin](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusteradmincredentials) and [ListClusterUser](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusterusercredentials) APIs</span></span>

#### <a name="azbatch"></a><span data-ttu-id="01b15-269">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="01b15-269">Az.Batch</span></span>
* <span data-ttu-id="01b15-270">Atualização da versão do SDK de Az.Batch para utilizar "Microsoft.Azure.Management.Batch" para 11.0.0</span><span class="sxs-lookup"><span data-stu-id="01b15-270">Updated Az.Batch to use 'Microsoft.Azure.Management.Batch' SDK version to 11.0.0</span></span>
* <span data-ttu-id="01b15-271">Adição da capacidade de definir a Identidade BatchAccount no cmdlet "New-AzBatchAccount"</span><span class="sxs-lookup"><span data-stu-id="01b15-271">Added the ability to set the BatchAccount Identity in the 'New-AzBatchAccount' cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="01b15-272">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="01b15-272">Az.CognitiveServices</span></span>
* <span data-ttu-id="01b15-273">Suporte para a apresentação das capacidades da conta.</span><span class="sxs-lookup"><span data-stu-id="01b15-273">Supported displaying account capabilities.</span></span>
* <span data-ttu-id="01b15-274">Suporte para a modificação de PublicNetworkAccess.</span><span class="sxs-lookup"><span data-stu-id="01b15-274">Supported modifying PublicNetworkAccess.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-275">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-275">Az.Compute</span></span>
* <span data-ttu-id="01b15-276">Adição do parâmetro SimulateEviction aos cmdlets Set-AzVM e Set-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="01b15-276">Added SimulateEviction parameter to Set-AzVM and Set-AzVmssVM cmdlets.</span></span>
* <span data-ttu-id="01b15-277">Adição de "Premium_LRS" ao mecanismo de preenchimento de argumentos do parâmetro StorageAccountType para o cmdlet New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="01b15-277">Added 'Premium_LRS' to the argument completer of StorageAccountType parameter for New-AzGalleryImageVersion cmdlet.</span></span>
* <span data-ttu-id="01b15-278">Adição de subestados a VMCustomScriptExtension [#11297]</span><span class="sxs-lookup"><span data-stu-id="01b15-278">Added Substatuses to VMCustomScriptExtension [#11297]</span></span>
* <span data-ttu-id="01b15-279">Adição de "Delete" ao mecanismo de preenchimento de argumentos do parâmetro EvictionPolicy para os cmdlets New-AzVM e New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="01b15-279">Added 'Delete' to the argument completer of EvictionPolicy parameter for New-AzVM and New-AzVMConfig cmdlets.</span></span>
* <span data-ttu-id="01b15-280">Correção do nome da nova Extensão de VM para SAP</span><span class="sxs-lookup"><span data-stu-id="01b15-280">Fixed name of new VM Extension for SAP</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="01b15-281">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="01b15-281">Az.DataFactory</span></span>
* <span data-ttu-id="01b15-282">Atualização da versão do SDK de .Net do ADF para 4.9.0</span><span class="sxs-lookup"><span data-stu-id="01b15-282">Updated ADF .Net SDK version to 4.9.0</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="01b15-283">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="01b15-283">Az.EventHub</span></span>
* <span data-ttu-id="01b15-284">Adição de parâmetros de Identidade Gerida aos cmdlets "New-AzEventHubNamespace" e "Set-AzEventHubNamespace"</span><span class="sxs-lookup"><span data-stu-id="01b15-284">Added Managed Identity parameters to 'New-AzEventHubNamespace' and 'Set-AzEventHubNamespace' cmdlets</span></span>

#### <a name="azfunctions"></a><span data-ttu-id="01b15-285">Az.Functions</span><span class="sxs-lookup"><span data-stu-id="01b15-285">Az.Functions</span></span>
* <span data-ttu-id="01b15-286">Adição de suporte para a criação de aplicações de funções do PowerShell 7.0 e de Java 11</span><span class="sxs-lookup"><span data-stu-id="01b15-286">Added support to create PowerShell 7.0 and Java 11 function apps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="01b15-287">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="01b15-287">Az.HDInsight</span></span>
* <span data-ttu-id="01b15-288">Suporte para listagem de anfitriões e reinício de anfitriões específicos do cluster HDInsight.</span><span class="sxs-lookup"><span data-stu-id="01b15-288">Supported listing hosts and restart specific hosts of the HDInsight cluster.</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="01b15-289">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="01b15-289">Az.HealthcareApis</span></span>
* <span data-ttu-id="01b15-290">Atualização da versão do SDK para 1.1.0</span><span class="sxs-lookup"><span data-stu-id="01b15-290">Updated the SDK version to 1.1.0</span></span>
* <span data-ttu-id="01b15-291">Adição de suporte para as definições de Exportação e a Identidade Gerida</span><span class="sxs-lookup"><span data-stu-id="01b15-291">Added support for Export settings and Managed Identity</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="01b15-292">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="01b15-292">Az.Monitor</span></span>
* <span data-ttu-id="01b15-293">Correção do parâmetro de objeto de entrada para "Set-AzActivityLogAlert"</span><span class="sxs-lookup"><span data-stu-id="01b15-293">Fixed input object parameter for 'Set-AzActivityLogAlert'</span></span>
* <span data-ttu-id="01b15-294">Correção do parâmetro "InputObject" para "Set-AzActionGroup" [#10868]</span><span class="sxs-lookup"><span data-stu-id="01b15-294">Fixed 'InputObject' parameter for 'Set-AzActionGroup' [#10868]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-295">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-295">Az.Network</span></span>
* <span data-ttu-id="01b15-296">Adição de suporte para o parâmetro AddressPrefixType a "Remove-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="01b15-296">Added support for AddressPrefixType parameter to 'Remove-AzExpressRouteCircuitConnectionConfig'</span></span>
* <span data-ttu-id="01b15-297">Adição de novos cmdlets para a Política de Firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="01b15-297">Added new cmdlets for Azure FirewallPolicy</span></span>
    - <span data-ttu-id="01b15-298">"New-AzFirewallPolicyDnsSetting"</span><span class="sxs-lookup"><span data-stu-id="01b15-298">'New-AzFirewallPolicyDnsSetting'</span></span>
    - <span data-ttu-id="01b15-299">Suporte para FQDN de Destino nas Regras de Rede para a Política de Firewall</span><span class="sxs-lookup"><span data-stu-id="01b15-299">Support for Destination FQDN in Network Rules for Firewall Policy</span></span>
* <span data-ttu-id="01b15-300">Adição de suporte para operações de conjuntos de endereços back-end</span><span class="sxs-lookup"><span data-stu-id="01b15-300">Added support for backend address pool operations</span></span>
    - <span data-ttu-id="01b15-301">"New-AzLoadBalancerBackendAddressConfig"</span><span class="sxs-lookup"><span data-stu-id="01b15-301">'New-AzLoadBalancerBackendAddressConfig'</span></span>
    - <span data-ttu-id="01b15-302">"New-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="01b15-302">'New-AzLoadBalancerBackendAddressPool'</span></span>
    - <span data-ttu-id="01b15-303">"Set-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="01b15-303">'Set-AzLoadBalancerBackendAddressPool'</span></span>
    - <span data-ttu-id="01b15-304">"Remove-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="01b15-304">'Remove-AzLoadBalancerBackendAddressPool'</span></span>
    - <span data-ttu-id="01b15-305">"Get-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="01b15-305">'Get-AzLoadBalancerBackendAddressPool'</span></span>
* <span data-ttu-id="01b15-306">Adição de validação de nomes para "New-AzIpGroup"</span><span class="sxs-lookup"><span data-stu-id="01b15-306">Added name validation for 'New-AzIpGroup'</span></span>
* <span data-ttu-id="01b15-307">Adição de novos cmdlets para a Política de Firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="01b15-307">Added new cmdlets for Azure FirewallPolicy</span></span>
    - <span data-ttu-id="01b15-308">"New-AzFirewallPolicyThreatIntelWhitelist"</span><span class="sxs-lookup"><span data-stu-id="01b15-308">'New-AzFirewallPolicyThreatIntelWhitelist'</span></span>
* <span data-ttu-id="01b15-309">Foram atualizados os seguintes comandos para a funcionalidade: Definição/remoção de servidores DNS personalizados no P2SVpnGateway de VirtualWan.</span><span class="sxs-lookup"><span data-stu-id="01b15-309">Updated below commands for feature: Custom dns servers set/remove on VirtualWan P2SVpnGateway.</span></span>
    - <span data-ttu-id="01b15-310">Atualização de New-AzP2sVpnGateway: Adição do parâmetro opcional "-CustomDnsServer" para os clientes especificarem os respetivos servidores DNS a definir no P2SVpnGateway, o qual pode ser utilizado por clientes do tipo Ponto a site.</span><span class="sxs-lookup"><span data-stu-id="01b15-310">Updated New-AzP2sVpnGateway: Added optional parameter '-CustomDnsServer' for customers to specify their dns servers to set on P2SVpnGateway, which can be used by Point to site clients.</span></span>
    - <span data-ttu-id="01b15-311">Atualização de Update-AzP2sVpnGateway: Adição do parâmetro opcional "-CustomDnsServer" para os clientes especificarem os respetivos servidores DNS a definir no P2SVpnGateway, o qual pode ser utilizado por clientes do tipo Ponto a site.</span><span class="sxs-lookup"><span data-stu-id="01b15-311">Updated Update-AzP2sVpnGateway: Added optional parameter '-CustomDnsServer' for customers to specify their dns servers to set on P2SVpnGateway, which can be used by Point to site clients.</span></span>
* <span data-ttu-id="01b15-312">Atualização de "Update-AzVpnGateway"</span><span class="sxs-lookup"><span data-stu-id="01b15-312">Updated 'Update-AzVpnGateway'</span></span>
    - <span data-ttu-id="01b15-313">Adição do parâmetro opcional "-BgpPeeringAddress" para os clientes especificarem os respetivos bgps personalizados a definir no VpnGateway.</span><span class="sxs-lookup"><span data-stu-id="01b15-313">Added optional parameter '-BgpPeeringAddress' for customers to specify their custom bgps to set on VpnGateway.</span></span>
* <span data-ttu-id="01b15-314">Adição de novo cmdlet para suportar a reposição do estado de encaminhamento de um recurso VirtualHub:</span><span class="sxs-lookup"><span data-stu-id="01b15-314">Added new cmdlet to support resetting the routing state of a VirtualHub resource:</span></span>
    - <span data-ttu-id="01b15-315">"Reset-AzHubRouter"</span><span class="sxs-lookup"><span data-stu-id="01b15-315">'Reset-AzHubRouter'</span></span>
* <span data-ttu-id="01b15-316">Atualização dos elementos indicados abaixo com base na alteração recente de Swagger para a Política de Firewall</span><span class="sxs-lookup"><span data-stu-id="01b15-316">Updated below things based on recent swagger change for Firewall Policy</span></span>
    - <span data-ttu-id="01b15-317">Alteração de nomes para RuleGroup, RuleCollectionGroup e RuleType</span><span class="sxs-lookup"><span data-stu-id="01b15-317">Changes names for RuleGroup, RuleCollectionGroup and RuleType</span></span>
    - <span data-ttu-id="01b15-318">Adição de suporte para Coleções de Regras de NAT da Política de Firewall para suportar várias Coleções de Regras de NAT</span><span class="sxs-lookup"><span data-stu-id="01b15-318">Added support for Firewall Policy NAT Rule Collections to support multiple NAT Rule Collection</span></span>
* <span data-ttu-id="01b15-319">[Alteração Interruptiva] Adição do parâmetro obrigatório "SourceIpGroup" para "New-AzFirewallPolicyApplicationRule" e "New-AzFirewallPolicyNetworkRule".</span><span class="sxs-lookup"><span data-stu-id="01b15-319">[Breaking Change] Added mandatory parameter 'SourceIpGroup' for 'New-AzFirewallPolicyApplicationRule' and 'New-AzFirewallPolicyNetworkRule'.</span></span>
* <span data-ttu-id="01b15-320">[Alteração Interruptiva] Correção do parâmetro "SourceAddress" de "New-AzFirewallPolicyApplicationRule" de modo a ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01b15-320">[Breaking Change] Fixed 'New-AzFirewallPolicyApplicationRule', parameter 'SourceAddress' to be mandatory.</span></span>
* <span data-ttu-id="01b15-321">[Alteração Interruptiva] Correção do parâmetro "SourceAddress" de "New-AzFirewallPolicyApplicationRule" de modo a ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01b15-321">[Breaking Change] Fixed 'New-AzFirewallPolicyApplicationRule', parameter 'SourceAddress' to be mandatory.</span></span>
* <span data-ttu-id="01b15-322">[Alteração Interruptiva] Remoção de parâmetros obrigatórios: "TranslatedAddress", "TranslatedPort" para "New-AzFirewallPolicyNatRuleCollection".</span><span class="sxs-lookup"><span data-stu-id="01b15-322">[Breaking Change] Removed mandatory parameters: 'TranslatedAddress', 'TranslatedPort' for 'New-AzFirewallPolicyNatRuleCollection'.</span></span>
* <span data-ttu-id="01b15-323">Adição de novos cmdlets para suportar PrivateLink no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="01b15-323">Added new cmdlets to support PrivateLink On Application Gateway</span></span>
    - <span data-ttu-id="01b15-324">"New-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="01b15-324">'New-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="01b15-325">"Get-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="01b15-325">'Get-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="01b15-326">"New-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="01b15-326">'New-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="01b15-327">"Set-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="01b15-327">'Set-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="01b15-328">"Remove-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="01b15-328">'Remove-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="01b15-329">"New-AzApplicationGatewayPrivateLinkIpConfiguration"</span><span class="sxs-lookup"><span data-stu-id="01b15-329">'New-AzApplicationGatewayPrivateLinkIpConfiguration'</span></span>
* <span data-ttu-id="01b15-330">Adição de novos cmdlets para o recurso subordinado HubRouteTables de VirtualHub.</span><span class="sxs-lookup"><span data-stu-id="01b15-330">Added new cmdlets for HubRouteTables child resource of VirtualHub.</span></span>
    - <span data-ttu-id="01b15-331">"New-AzVHubRoute"</span><span class="sxs-lookup"><span data-stu-id="01b15-331">'New-AzVHubRoute'</span></span>
    - <span data-ttu-id="01b15-332">"New-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="01b15-332">'New-AzVHubRouteTable'</span></span>
    - <span data-ttu-id="01b15-333">"Get-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="01b15-333">'Get-AzVHubRouteTable'</span></span>
    - <span data-ttu-id="01b15-334">"Update-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="01b15-334">'Update-AzVHubRouteTable'</span></span>
    - <span data-ttu-id="01b15-335">"Remove-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="01b15-335">'Remove-AzVHubRouteTable'</span></span>
* <span data-ttu-id="01b15-336">Atualização dos cmdlets existentes para suportar o parâmetro de entrada opcional RoutingConfiguration para encaminhamento personalizado em VirtualWan.</span><span class="sxs-lookup"><span data-stu-id="01b15-336">Updated existing cmdlets to support optional RoutingConfiguration input parameter for custom routing in VirtualWan.</span></span>
    - <span data-ttu-id="01b15-337">"New-AzExpressRouteConnection"</span><span class="sxs-lookup"><span data-stu-id="01b15-337">'New-AzExpressRouteConnection'</span></span>
    - <span data-ttu-id="01b15-338">"Set-AzExpressRouteConnection"</span><span class="sxs-lookup"><span data-stu-id="01b15-338">'Set-AzExpressRouteConnection'</span></span>
    - <span data-ttu-id="01b15-339">"New-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="01b15-339">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="01b15-340">"Update-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="01b15-340">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="01b15-341">"New-AzVpnConnection"</span><span class="sxs-lookup"><span data-stu-id="01b15-341">'New-AzVpnConnection'</span></span>
    - <span data-ttu-id="01b15-342">"Update-AzVpnConnection"</span><span class="sxs-lookup"><span data-stu-id="01b15-342">'Update-AzVpnConnection'</span></span>
    - <span data-ttu-id="01b15-343">"New-AzP2sVpnGateway"</span><span class="sxs-lookup"><span data-stu-id="01b15-343">'New-AzP2sVpnGateway'</span></span>
    - <span data-ttu-id="01b15-344">"Update-AzP2sVpnGateway"</span><span class="sxs-lookup"><span data-stu-id="01b15-344">'Update-AzP2sVpnGateway'</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="01b15-345">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-345">Az.OperationalInsights</span></span>
* <span data-ttu-id="01b15-346">Correção do erro PSWorkspace não implementa IOperationalInsightsWorkspace [#12135]</span><span class="sxs-lookup"><span data-stu-id="01b15-346">Fixed bug PSWorkspace doesn't implement IOperationalInsightsWorkspace [#12135]</span></span>
* <span data-ttu-id="01b15-347">Adição de "pergb2018" ao conjunto de valores válidos do parâmetro "Sku" em "Set-AzOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="01b15-347">Added 'pergb2018' to valid value set of parameter 'Sku' in 'Set-AzOperationalInsightsWorkspace'</span></span> 
* <span data-ttu-id="01b15-348">Adição do alias "FunctionParameters" para o parâmetro "FunctionParameter" a</span><span class="sxs-lookup"><span data-stu-id="01b15-348">Added alias 'FunctionParameters' for parameter 'FunctionParameter' to</span></span>
    - <span data-ttu-id="01b15-349">"New-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="01b15-349">'New-AzOperationalInsightsSavedSearch'</span></span>
    - <span data-ttu-id="01b15-350">"Set-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="01b15-350">'Set-AzOperationalInsightsSavedSearch'</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-351">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-351">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-352">Adição de suporte no Azure Backup para a obtenção de itens de MAB.</span><span class="sxs-lookup"><span data-stu-id="01b15-352">Azure Backup added support for fetching MAB items.</span></span>
* <span data-ttu-id="01b15-353">Suporte do Azure Site Recovery para o tipo de disco "StandardSSD_LRS"</span><span class="sxs-lookup"><span data-stu-id="01b15-353">Azure Site Recovery supports disk type 'StandardSSD_LRS'</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-354">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-354">Az.Resources</span></span>
* <span data-ttu-id="01b15-355">Adição de "UsageLocation", "GivenName", "Surname", "AccountEnabled", "MailNickname", "Mail" em "PSADUser" [#10526] [#10497]</span><span class="sxs-lookup"><span data-stu-id="01b15-355">Added 'UsageLocation', 'GivenName', 'Surname', 'AccountEnabled', 'MailNickname', 'Mail' on 'PSADUser' [#10526] [#10497]</span></span>
* <span data-ttu-id="01b15-356">Correção do problema em que "-Mail" não funciona em "Get-AzADUser" [#11981]</span><span class="sxs-lookup"><span data-stu-id="01b15-356">Fixed issue that '-Mail' doesn't work on 'Get-AzADUser' [#11981]</span></span>
* <span data-ttu-id="01b15-357">Adição do parâmetro "-ExcludeChangeType" a "Get-AzDeploymentWhatIfResult" e "Get-AzResourceGroupDeploymentWhatIfResult"</span><span class="sxs-lookup"><span data-stu-id="01b15-357">Added '-ExcludeChangeType' parameter to 'Get-AzDeploymentWhatIfResult' and 'Get-AzResourceGroupDeploymentWhatIfResult'</span></span>
* <span data-ttu-id="01b15-358">Adição do parâmetro "-WhatIfExcludeChangeType" a "New-AzDeployment" e "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="01b15-358">Added '-WhatIfExcludeChangeType' parameter to 'New-AzDeployment' and 'New-AzResourceGroupDeployment'</span></span>
* <span data-ttu-id="01b15-359">Atualização de cmdlets "Test-Az\*Deployment" para apresentação de mensagens de erro melhores</span><span class="sxs-lookup"><span data-stu-id="01b15-359">Updated 'Test-Az\*Deployment' cmdlets to show better error messages</span></span>
* <span data-ttu-id="01b15-360">Correção da mensagem de ajuda para o parâmetro "-Name" de criação de implementação e cmdlets What-If</span><span class="sxs-lookup"><span data-stu-id="01b15-360">Fixed help message for '-Name' parameter of deployment create and What-If cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-361">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-361">Az.Sql</span></span>
* <span data-ttu-id="01b15-362">Adição de suporte para o principal de serviço para o cmdlet Set SQL Server Azure Active Directory Admin</span><span class="sxs-lookup"><span data-stu-id="01b15-362">Added support for service principal for Set SQL Server Azure Active Directory Admin cmdlet</span></span>
* <span data-ttu-id="01b15-363">Correção de problema de sincronização em cmdlets de Classificação de Dados.</span><span class="sxs-lookup"><span data-stu-id="01b15-363">Fixed sync issue in Data Classification cmdlets.</span></span>
* <span data-ttu-id="01b15-364">Suporte para a pesquisa de utilizador por correio em "Set-AzSqlServerActiveDirectoryAdministrator" [#12192]</span><span class="sxs-lookup"><span data-stu-id="01b15-364">Supported searching user by mail on 'Set-AzSqlServerActiveDirectoryAdministrator' [#12192]</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-365">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-365">Az.Storage</span></span>
* <span data-ttu-id="01b15-366">Suporte para a criação de Conta de armazenamento com RequireInfrastructureEncryption</span><span class="sxs-lookup"><span data-stu-id="01b15-366">Supported create Storage account with RequireInfrastructureEncryption</span></span>
    -  <span data-ttu-id="01b15-367">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="01b15-367">'New-AzStorageAccount'</span></span>
* <span data-ttu-id="01b15-368">Mudança da lógica de carregamento de Azure.Core para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-368">Moved the logic of loading Azure.Core to Az.Accounts</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="01b15-369">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-369">Az.Websites</span></span>
* <span data-ttu-id="01b15-370">Adição de salvaguarda para eliminar a aplicação Web criada em caso de falha do restauro em "Restore-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="01b15-370">Added safeguard to delete created webapp if restore failed in 'Restore-AzDeletedWebApp'</span></span>
* <span data-ttu-id="01b15-371">Adição de "SourceWebApp.Location" para "New-AzWebApp" e "New-AzWebAppSlot"</span><span class="sxs-lookup"><span data-stu-id="01b15-371">Added 'SourceWebApp.Location' for 'New-AzWebApp' and 'New-AzWebAppSlot'</span></span>
* <span data-ttu-id="01b15-372">Correção do erro que impedia a alteração de definições de Contentor em "Set-AzWebApp" e "Set-AzWebAppSlot"</span><span class="sxs-lookup"><span data-stu-id="01b15-372">Fixed bug that prevented changing Container settings in 'Set-AzWebApp' and 'Set-AzWebAppSlot'</span></span>
* <span data-ttu-id="01b15-373">Correção do erro para obter SiteConfig quando -Name não é fornecido para Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="01b15-373">Fixed bug to get SiteConfig when -Name is not given for Get-AzWebApp</span></span>
* <span data-ttu-id="01b15-374">Adição de suporte para a criação de ASP para Aplicações Linux</span><span class="sxs-lookup"><span data-stu-id="01b15-374">Added a support to create ASP for Linux Apps</span></span>
* <span data-ttu-id="01b15-375">Adição de exceções para clonagem entre grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="01b15-375">Added exceptions for clone across resource groups</span></span>

## <a name="420---june-2020"></a><span data-ttu-id="01b15-376">4.2.0 - Junho de 2020</span><span class="sxs-lookup"><span data-stu-id="01b15-376">4.2.0 - June 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="01b15-377">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-377">Az.Accounts</span></span>
* <span data-ttu-id="01b15-378">Correção de um problema que fazia com que o Az ignorasse registos nas tarefas da Automatização do Azure ou do PowerShell [#11492]</span><span class="sxs-lookup"><span data-stu-id="01b15-378">Fixed an issue that may cause Az to skip logs in Azure Automation or PowerShell jobs [#11492]</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="01b15-379">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="01b15-379">Az.AnalysisServices</span></span>
* <span data-ttu-id="01b15-380">Atualização da versão de assemblagem dos cmdlets de plano de dados</span><span class="sxs-lookup"><span data-stu-id="01b15-380">Updated assembly version of data plane cmdlets</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="01b15-381">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="01b15-381">Az.ApiManagement</span></span>
* <span data-ttu-id="01b15-382">Atualização da versão de assemblagem dos cmdlets de gestão de serviços</span><span class="sxs-lookup"><span data-stu-id="01b15-382">Updated assembly version of service management cmdlets</span></span>

#### <a name="azbilling"></a><span data-ttu-id="01b15-383">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="01b15-383">Az.Billing</span></span>
* <span data-ttu-id="01b15-384">Atualização da versão de assemblagem dos cmdlets de consumo</span><span class="sxs-lookup"><span data-stu-id="01b15-384">Updated assembly version of consumption cmdlets</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="01b15-385">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="01b15-385">Az.CognitiveServices</span></span>
* <span data-ttu-id="01b15-386">Suporte para o controlo de PrivateEndpoint e PublicNetworkAccess.</span><span class="sxs-lookup"><span data-stu-id="01b15-386">Support PrivateEndpoint and PublicNetworkAccess control.</span></span> 

#### <a name="azdatafactory"></a><span data-ttu-id="01b15-387">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="01b15-387">Az.DataFactory</span></span>
* <span data-ttu-id="01b15-388">Atualização da versão de assemblagem dos cmdlets V2 de fábrica de dados</span><span class="sxs-lookup"><span data-stu-id="01b15-388">Updated assembly version of data factory V2 cmdlets</span></span>

#### <a name="azdatashare"></a><span data-ttu-id="01b15-389">Az.DataShare</span><span class="sxs-lookup"><span data-stu-id="01b15-389">Az.DataShare</span></span>
* <span data-ttu-id="01b15-390">Disponibilidade geral do módulo "Az.DataShare"</span><span class="sxs-lookup"><span data-stu-id="01b15-390">General availability of ''Az.DataShare'' module</span></span>

#### <a name="azdesktopvirtualization"></a><span data-ttu-id="01b15-391">Az.DesktopVirtualization</span><span class="sxs-lookup"><span data-stu-id="01b15-391">Az.DesktopVirtualization</span></span>
* <span data-ttu-id="01b15-392">Disponibilidade geral do módulo "Az.DesktopVirtualization"</span><span class="sxs-lookup"><span data-stu-id="01b15-392">General availability of ''Az.DesktopVirtualization'' module</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="01b15-393">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-393">Az.OperationalInsights</span></span>
* <span data-ttu-id="01b15-394">Atualização do SDK para a versão 0.21.0</span><span class="sxs-lookup"><span data-stu-id="01b15-394">Upgraded SDK to 0.21.0</span></span>
* <span data-ttu-id="01b15-395">Adição de parâmetros opcionais a</span><span class="sxs-lookup"><span data-stu-id="01b15-395">Added optional parameters to</span></span> 
    - <span data-ttu-id="01b15-396">"New-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="01b15-396">'New-AzOperationalInsightsSavedSearch'</span></span>
    - <span data-ttu-id="01b15-397">"Set-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="01b15-397">'Set-AzOperationalInsightsSavedSearch'</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="01b15-398">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-398">Az.PolicyInsights</span></span>
* <span data-ttu-id="01b15-399">Correção do exemplo 3 de "Start-AzPolicyComplianceScan"</span><span class="sxs-lookup"><span data-stu-id="01b15-399">Corrected example 3 for 'Start-AzPolicyComplianceScan'</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="01b15-400">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="01b15-400">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="01b15-401">Atualização da versão de assemblagem dos cmdlets do PowerBI</span><span class="sxs-lookup"><span data-stu-id="01b15-401">Updated assembly version of PowerBI cmdlets</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="01b15-402">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="01b15-402">Az.PrivateDns</span></span>
* <span data-ttu-id="01b15-403">Correção da formatação da cadeia de saída verbosa de Remove-AzPrivateDnsRecordSet</span><span class="sxs-lookup"><span data-stu-id="01b15-403">Corrected verbose output string formatting for Remove-AzPrivateDnsRecordSet</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-404">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-404">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-405">Suporte do Azure Site Recovery para a criação de um plano de recuperação para replicação zona a zona a partir de uma entrada xml.</span><span class="sxs-lookup"><span data-stu-id="01b15-405">Azure Site Recovery support for creating recovery plan for zone to zone replication from xml input.</span></span>
* <span data-ttu-id="01b15-406">Atualização da versão de assemblagem dos cmdlets do SiteRecovery e Backup</span><span class="sxs-lookup"><span data-stu-id="01b15-406">Updated assembly version of SiteRecovery and Backup cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-407">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-407">Az.Resources</span></span>
* <span data-ttu-id="01b15-408">Adição do parâmetro Tail aos cmdlets Get-AzDeploymentScriptLog e Save-AzDeploymentScriptLog</span><span class="sxs-lookup"><span data-stu-id="01b15-408">Added Tail parameter to Get-AzDeploymentScriptLog and Save-AzDeploymentScriptLog cmdlets</span></span>
* <span data-ttu-id="01b15-409">Formatação da propriedade Output e apresentação da mesma na saída do cmdlet Get-AzDeploymentScript</span><span class="sxs-lookup"><span data-stu-id="01b15-409">Formatted Output property and show it on the Get-AzDeploymentScript cmdlet output</span></span>
* <span data-ttu-id="01b15-410">Mudança de nome do parâmetro -DeploymentScriptInputObject para -DeploymentScriptObject</span><span class="sxs-lookup"><span data-stu-id="01b15-410">Renamed -DeploymentScriptInputObject parameter to -DeploymentScriptObject</span></span>
* <span data-ttu-id="01b15-411">Correção do nome em falta do ficheiro/destino nas mensagens de cmdlet.</span><span class="sxs-lookup"><span data-stu-id="01b15-411">Fixed missing file/target name in cmdlet messages.</span></span>
* <span data-ttu-id="01b15-412">Atualização da versão de assemblagem dos cmdlets de gestor de recursos e de etiquetas</span><span class="sxs-lookup"><span data-stu-id="01b15-412">Updated assembly version of resource manager and tags cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-413">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-413">Az.Sql</span></span>
* <span data-ttu-id="01b15-414">Adição de UsePrivateLinkConnection a "New-AzSqlSyncGroup", "Update-AzSqlSyncGroup", "New-AzSqlSyncMember" e "Update-AzSqlSyncMember"</span><span class="sxs-lookup"><span data-stu-id="01b15-414">Added UsePrivateLinkConnection to 'New-AzSqlSyncGroup', 'Update-AzSqlSyncGroup', 'New-AzSqlSyncMember' and 'Update-AzSqlSyncMember'</span></span>
* <span data-ttu-id="01b15-415">Adição de SyncMemberAzureDatabaseResourceId a "New-AzSqlSyncMember" e "Update-AzSqlSyncMember"</span><span class="sxs-lookup"><span data-stu-id="01b15-415">Added SyncMemberAzureDatabaseResourceId to 'New-AzSqlSyncMember' and 'Update-AzSqlSyncMember'</span></span>
* <span data-ttu-id="01b15-416">Adição do suporte de pesquisa de Utilizador convidado ao cmdlet Set SQL Server Azure Active Directory Admin</span><span class="sxs-lookup"><span data-stu-id="01b15-416">Added Guest user lookup support to Set SQL Server Azure Active Directory Admin cmdlet</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-417">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-417">Az.Storage</span></span>
* <span data-ttu-id="01b15-418">Atualização da versão de assemblagem dos cmdlets de plano de dados</span><span class="sxs-lookup"><span data-stu-id="01b15-418">Updated assembly version of data plane cmdlets</span></span>

## <a name="410---may-2020"></a><span data-ttu-id="01b15-419">4.1.0 - Maio de 2020</span><span class="sxs-lookup"><span data-stu-id="01b15-419">4.1.0 - May 2020</span></span>
### <a name="highlights-since-the-last-release"></a><span data-ttu-id="01b15-420">Destaques desde a última versão</span><span class="sxs-lookup"><span data-stu-id="01b15-420">Highlights since the last release</span></span>
* <span data-ttu-id="01b15-421">Versões do PowerShell suportadas: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span><span class="sxs-lookup"><span data-stu-id="01b15-421">Supported PowerShell versions: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span></span>
* <span data-ttu-id="01b15-422">Disponibilidade geral de Az.Functions</span><span class="sxs-lookup"><span data-stu-id="01b15-422">General availability of Az.Functions</span></span> 
* <span data-ttu-id="01b15-423">Az.ApiManagement, Az.Batch, Az.Compute, Az.KeyVault, Az.Monitor, Az.Network, Az.OperationalInsights, Az.Resources e Az.Storage são alvo de grandes versões</span><span class="sxs-lookup"><span data-stu-id="01b15-423">Az.ApiManagement, Az.Batch, Az.Compute, Az.KeyVault, Az.Monitor, Az.Network, Az.OperationalInsights, Az.Resources, and Az.Storage have major release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="01b15-424">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-424">Az.Accounts</span></span>
* <span data-ttu-id="01b15-425">"Add-AzEnvironment" e "Set-AzEnvironment" foram atualizados para aceitar os parâmetros "AzureSynapseAnalyticsEndpointResourceId" e "AzureSynapseAnalyticsEndpointSuffix"</span><span class="sxs-lookup"><span data-stu-id="01b15-425">Updated 'Add-AzEnvironment' and 'Set-AzEnvironment' to accept parameters 'AzureSynapseAnalyticsEndpointResourceId' and 'AzureSynapseAnalyticsEndpointSuffix'</span></span>
* <span data-ttu-id="01b15-426">Foram adicionadas assemblagens relacionadas ao Azure.Core em Az.Accounts; as plataformas suportadas do PowerShell incluem Windows PowerShell 5.1, PowerShell Core 6.2.4, PowerShell 7+</span><span class="sxs-lookup"><span data-stu-id="01b15-426">Added Azure.Core related assemblies into Az.Accounts, supported PowerShell platforms include Windows PowerShell 5.1, PowerShell Core 6.2.4, PowerShell 7+</span></span>

#### <a name="azaks"></a><span data-ttu-id="01b15-427">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="01b15-427">Az.Aks</span></span>
* <span data-ttu-id="01b15-428">Versão da API atualizada para 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="01b15-428">Upgraded API Version to 2019-10-01</span></span>
* <span data-ttu-id="01b15-429">Suportado para criar o AKS com contentores do Windows</span><span class="sxs-lookup"><span data-stu-id="01b15-429">Supported to create AKS using Windows container</span></span>
* <span data-ttu-id="01b15-430">Novos cmdlets fornecidos: "New-AzAksNodePool", "Update-AzAksNodePool", "Remove-AzAksNodePool",        "Get-AzAksNodePool", "Install-AzAksKubectl", "Get-AzAksVersion"</span><span class="sxs-lookup"><span data-stu-id="01b15-430">Provided new cmdlets: 'New-AzAksNodePool', 'Update-AzAksNodePool', 'Remove-AzAksNodePool',        'Get-AzAksNodePool', 'Install-AzAksKubectl', 'Get-AzAksVersion'</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="01b15-431">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="01b15-431">Az.ApiManagement</span></span>
* <span data-ttu-id="01b15-432">"New-AzApiManagement" e "Set-AzApiManagement": o nome do parâmetro [-AssignIdentity] foi mudado para [-SystemAssignedIdentity]</span><span class="sxs-lookup"><span data-stu-id="01b15-432">'New-AzApiManagement' and 'Set-AzApiManagement': [-AssignIdentity] parameter renamed as [-SystemAssignedIdentity]</span></span>
* <span data-ttu-id="01b15-433">"New-AzApiManagement" e "Set-AzApiManagement": Novo parâmetro adicionado: [-UserAssignedIdentity <String[]>]</span><span class="sxs-lookup"><span data-stu-id="01b15-433">'New-AzApiManagement' and 'Set-AzApiManagement': New parameter added: [-UserAssignedIdentity <String[]>]</span></span>
* <span data-ttu-id="01b15-434">"Get-AzApiManagementProperty": o nome foi mudado para "Get-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="01b15-434">'Get-AzApiManagementProperty': renamed as 'Get-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="01b15-435">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="01b15-435">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="01b15-436">"New-AzApiManagementProperty": o nome foi mudado para "New-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="01b15-436">'New-AzApiManagementProperty': renamed as 'New-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="01b15-437">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="01b15-437">PropertyId parameter renamed as NamedValueId.</span></span> 
* <span data-ttu-id="01b15-438">"Set-AzApiManagementProperty": o nome foi mudado para "Set-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="01b15-438">'Set-AzApiManagementProperty': renamed as 'Set-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="01b15-439">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="01b15-439">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="01b15-440">"Remove-AzApiManagementProperty": o nome foi mudado para "Remove-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="01b15-440">'Remove-AzApiManagementProperty': renamed as 'Remove-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="01b15-441">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="01b15-441">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="01b15-442">Foi adicionado o cmdlet novo "Get-AzApiManagementAuthorizationServerClientSecret" e "Get-AzApiManagementAuthorizationServer" vai deixar de devolver o segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="01b15-442">Added new 'Get-AzApiManagementAuthorizationServerClientSecret' cmdlet and 'Get-AzApiManagementAuthorizationServer' will not return client secret anymore.</span></span>
* <span data-ttu-id="01b15-443">Foi adicionado o cmdlet novo "Get-AzApiManagementNamedValueSecretValue" e "Get-AzApiManagementNamedValue" vai deixar de devolver o valor do segredo.</span><span class="sxs-lookup"><span data-stu-id="01b15-443">Added new 'Get-AzApiManagementNamedValueSecretValue' cmdlet and 'Get-AzApiManagementNamedValue' will not return secret value.</span></span>
* <span data-ttu-id="01b15-444">Foi adicionado o cmdlet novo "Get-AzApiManagementOpenIdConnectProviderClientSecret" e "Get-AzApiManagementOpenIdConnectProvider" vai deixar de devolver o segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="01b15-444">Added new 'Get-AzApiManagementOpenIdConnectProviderClientSecret' cmdlet and 'Get-AzApiManagementOpenIdConnectProvider' will not return client secret anymore.</span></span>
* <span data-ttu-id="01b15-445">Foi adicionado o cmdlet "Get-AzApiManagementSubscriptionKey" e "Get-AzApiManagementSubscription" vai deixar de devolver chaves de subscrições.</span><span class="sxs-lookup"><span data-stu-id="01b15-445">Added new 'Get-AzApiManagementSubscriptionKey' cmdlet and 'Get-AzApiManagementSubscription' will not return subscription keys anymore.</span></span>
* <span data-ttu-id="01b15-446">Foi adicionado o cmdlet novo "Get-AzApiManagementTenantAccessSecret" e "Get-AzApiManagementTenantAccess" vai deixar de devolver chaves.</span><span class="sxs-lookup"><span data-stu-id="01b15-446">Added new 'Get-AzApiManagementTenantAccessSecret' cmdlet and 'Get-AzApiManagementTenantAccess' will not return keys anymore.</span></span>
* <span data-ttu-id="01b15-447">Foi adicionado o cmdlet novo "Get-AzApiManagementTenantGitAccessSecret" e "Get-AzApiManagementTenantGitAccess" vai deixar de devolver chaves.</span><span class="sxs-lookup"><span data-stu-id="01b15-447">Added new 'Get-AzApiManagementTenantGitAccessSecret' cmdlet and 'Get-AzApiManagementTenantGitAccess' will not return keys anymore.</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="01b15-448">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-448">Az.ApplicationInsights</span></span>
* <span data-ttu-id="01b15-449">Parâmetros adicionados: "RetentionInDays" "PublicNetworkAccessForIngestion" "PublicNetworkAccessForQuery" a "New-AzApplicationInsights"</span><span class="sxs-lookup"><span data-stu-id="01b15-449">Added Parameters: 'RetentionInDays' 'PublicNetworkAccessForIngestion' 'PublicNetworkAccessForQuery' for 'New-AzApplicationInsights'</span></span>
* <span data-ttu-id="01b15-450">Foi criado o cmdlet "Update-AzApplicationInsights”</span><span class="sxs-lookup"><span data-stu-id="01b15-450">Created cmdlet 'Update-AzApplicationInsights'</span></span>
* <span data-ttu-id="01b15-451">Foram criados cmdlets para a Conta de Armazenamento Associada</span><span class="sxs-lookup"><span data-stu-id="01b15-451">Created cmdlets for Linked Storage Account</span></span>

#### <a name="azbatch"></a><span data-ttu-id="01b15-452">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="01b15-452">Az.Batch</span></span>
* <span data-ttu-id="01b15-453">Az.Batch foi atualizado para utilizar a versão do SDK "Microsoft.Azure.Batc" 13.0.0 e a versão do SDK "Microsoft.Azure.Management.Batch" 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="01b15-453">Updated Az.Batch to use 'Microsoft.Azure.Batch' SDK version 13.0.0 and 'Microsoft.Azure.Management.Batch' SDK version 9.0.0.</span></span>
* <span data-ttu-id="01b15-454">Foi adicionada a capacidade de selecionar o tipo de certificado que vai ser adicionado mediante a utilização do novo parâmetro "-CertificateKind" para "New-AzBatchCertificate".</span><span class="sxs-lookup"><span data-stu-id="01b15-454">Added the ability to select the kind of certificate being added using the new '-CertificateKind' parameter to 'New-AzBatchCertificate'.</span></span>
* <span data-ttu-id="01b15-455">A propriedade "ApplicationPackages" foi removida de "PSApplication", que anteriormente era sempre ''.</span><span class="sxs-lookup"><span data-stu-id="01b15-455">Removed 'ApplicationPackages' property from 'PSApplication' which was previously always ''.</span></span>
  - <span data-ttu-id="01b15-456">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com "Get-AzBatchApplicationPackage".</span><span class="sxs-lookup"><span data-stu-id="01b15-456">The specific packages inside of an application now can be retrieved using 'Get-AzBatchApplicationPackage'.</span></span> <span data-ttu-id="01b15-457">Por exemplo: "Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication".</span><span class="sxs-lookup"><span data-stu-id="01b15-457">For example: 'Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication'.</span></span>
* <span data-ttu-id="01b15-458">Agora, ao utilizar "New-AzBatchPool" para criar um conjunto, a propriedade "VirtualMachineImageId" de "PSImageReference" só pode fazer referência a uma imagem do Shared Image Gallery.</span><span class="sxs-lookup"><span data-stu-id="01b15-458">When creating a pool using 'New-AzBatchPool', the 'VirtualMachineImageId' property of 'PSImageReference' can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="01b15-459">Ao utilizar "New-AzBatchPool" para criar um conjunto, o conjunto pode ser aprovisionado sem um IP público mediante a utilização da nova propriedade "PublicIPAddressConfiguration" de "PSNetworkConfiguration".</span><span class="sxs-lookup"><span data-stu-id="01b15-459">When creating a pool using 'New-AzBatchPool', the pool can be provisioned without a public IP using the new 'PublicIPAddressConfiguration' property of 'PSNetworkConfiguration'.</span></span>
  - <span data-ttu-id="01b15-460">A propriedade "PublicIPs" de "PSNetworkConfiguration" foi igualmente movida para "PSPublicIPAddressConfiguration".</span><span class="sxs-lookup"><span data-stu-id="01b15-460">The 'PublicIPs' property of 'PSNetworkConfiguration' has moved in to 'PSPublicIPAddressConfiguration' as well.</span></span> <span data-ttu-id="01b15-461">Esta propriedade só pode ser especificada se "IPAddressProvisioningType" for "UserManaged".</span><span class="sxs-lookup"><span data-stu-id="01b15-461">This property can only be specified if 'IPAddressProvisioningType' is 'UserManaged'.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-462">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-462">Az.Compute</span></span>
* <span data-ttu-id="01b15-463">Foi adicionado o parâmetro HostId ao cmdlet "Update-AzVM"</span><span class="sxs-lookup"><span data-stu-id="01b15-463">Added HostId parameter to 'Update-AzVM' cmdlet</span></span>
* <span data-ttu-id="01b15-464">Os documentos de Ajuda para os cmdlets "New-AzVMConfig", "New-AzVmssConfig", "Update-AzVmss", "Set-AzVMOperatingSystem" e "Set-AzVmssOsProfile" foram atualizados.</span><span class="sxs-lookup"><span data-stu-id="01b15-464">Updated Help documents for 'New-AzVMConfig', 'New-AzVmssConfig', 'Update-AzVmss', 'Set-AzVMOperatingSystem' and 'Set-AzVmssOsProfile' cmdlets.</span></span>
* <span data-ttu-id="01b15-465">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="01b15-465">Breaking changes</span></span>
    - <span data-ttu-id="01b15-466">O parâmetro FilterExpression foi removido do cmdlet "Get-AzVMImage".</span><span class="sxs-lookup"><span data-stu-id="01b15-466">FilterExpression parameter is removed from 'Get-AzVMImage' cmdlet.</span></span>
    - <span data-ttu-id="01b15-467">O parâmetro AssignIdentity foi removido dos cmdlets "New-AzVmssConfig", "New-AzVMConfig" e "Update-AzVM".</span><span class="sxs-lookup"><span data-stu-id="01b15-467">AssignIdentity parameter is removed from 'New-AzVmssConfig', 'New-AzVMConfig' and 'Update-AzVM' cmdlets.</span></span>
    - <span data-ttu-id="01b15-468">AutomaticRepairMaxInstanceRepairsPercent foi removido dos cmdlets "New-AzVmssConfig" e "Update-AzVmss".</span><span class="sxs-lookup"><span data-stu-id="01b15-468">AutomaticRepairMaxInstanceRepairsPercent is removed from 'New-AzVmssConfig' and 'Update-AzVmss' cmdlets.</span></span>
    - <span data-ttu-id="01b15-469">As propriedades AvailabilitySetsColocationStatus, VirtualMachinesColocationStatus e VirtualMachineScaleSetsColocationStatus foram removidas de ProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="01b15-469">AvailabilitySetsColocationStatus, VirtualMachinesColocationStatus and VirtualMachineScaleSetsColocationStatus properties are removed from ProximityPlacementGroup.</span></span>
    - <span data-ttu-id="01b15-470">A propriedade MaxInstanceRepairsPercent foi removida de AutomaticRepairsPolicy.</span><span class="sxs-lookup"><span data-stu-id="01b15-470">MaxInstanceRepairsPercent property is removed from AutomaticRepairsPolicy.</span></span>
    - <span data-ttu-id="01b15-471">Os tipos de AvailabilitySets, VirtualMachines e VirtualMachineScaleSets foram alterados de IList<SubResource> para IList<SubResourceWithColocationStatus>.</span><span class="sxs-lookup"><span data-stu-id="01b15-471">The types of AvailabilitySets, VirtualMachines and VirtualMachineScaleSets are changed from IList<SubResource> to IList<SubResourceWithColocationStatus>.</span></span>
* <span data-ttu-id="01b15-472">A descrição do cmdlet "Get-AzVM" foi atualizada para o descrever melhor.</span><span class="sxs-lookup"><span data-stu-id="01b15-472">Description for 'Get-AzVM' cmdlet has been updated to better describe it.</span></span> 

#### <a name="azdatafactory"></a><span data-ttu-id="01b15-473">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="01b15-473">Az.DataFactory</span></span>
* <span data-ttu-id="01b15-474">CRUD suportado das propriedades de fluxo de dados no IR Gerido.</span><span class="sxs-lookup"><span data-stu-id="01b15-474">Supported CRUD of data flow runtime properties in Managed IR.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="01b15-475">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="01b15-475">Az.FrontDoor</span></span>
* <span data-ttu-id="01b15-476">Foram adicionados cmdlets novos para criação, atualização, obtenção e eliminação do objeto de Motor de Regras do Front Door</span><span class="sxs-lookup"><span data-stu-id="01b15-476">Added new cmdlets for creation, update, retreival, and deletion of Front Door Rules Engine object</span></span>
* <span data-ttu-id="01b15-477">Foram adicionados cmdlets de programas auxiliares para construção do objeto de Motor de Regras do Front Door</span><span class="sxs-lookup"><span data-stu-id="01b15-477">Added helper cmdlets for construction of Front Door Rules Engine object</span></span>
* <span data-ttu-id="01b15-478">Foi adicionada a referência ao Motor de Regras ao objeto Regra de Encaminhamento do Front Door.</span><span class="sxs-lookup"><span data-stu-id="01b15-478">Added Rules Engine reference to Front Door Routing Rule object.</span></span>
* <span data-ttu-id="01b15-479">Foram adicionados parâmetros do Private Link ao objeto de Back-end do Front Door</span><span class="sxs-lookup"><span data-stu-id="01b15-479">Added Private Link parameters to Front Door Backend object</span></span>

#### <a name="azfunctions"></a><span data-ttu-id="01b15-480">Az.Functions</span><span class="sxs-lookup"><span data-stu-id="01b15-480">Az.Functions</span></span>
* <span data-ttu-id="01b15-481">Disponibilidade geral do módulo Az.Functions</span><span class="sxs-lookup"><span data-stu-id="01b15-481">General availability of ''Az.Functions'' module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="01b15-482">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="01b15-482">Az.HDInsight</span></span>
* <span data-ttu-id="01b15-483">Encriptação de discos de chave gerida pelo cliente suportada</span><span class="sxs-lookup"><span data-stu-id="01b15-483">Supported Customer-managed key disk encryption.</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="01b15-484">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="01b15-484">Az.HealthcareApis</span></span>
* <span data-ttu-id="01b15-485">As políticas de acesso já não são predefinidas para o principal atual</span><span class="sxs-lookup"><span data-stu-id="01b15-485">Access policies are no longer defaulted to the current principal</span></span>

#### <a name="aziothub"></a><span data-ttu-id="01b15-486">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="01b15-486">Az.IotHub</span></span>
* <span data-ttu-id="01b15-487">Foi adicionado um cmdlet para invocar uma consulta num hub IoT para obter informações mediante a utilização de uma linguagem tipo SQL.</span><span class="sxs-lookup"><span data-stu-id="01b15-487">Added cmdlet to invoke a query in an IoT hub to retrieve information using a SQL-like language.</span></span>
* <span data-ttu-id="01b15-488">Foi corrigido um problema em que "Add-AzIotHubDevice" falha ao criar um Dispositivo Compatível com o Edge sem dispositivos subordinados [#11597]</span><span class="sxs-lookup"><span data-stu-id="01b15-488">Fix issue that 'Add-AzIotHubDevice' fails to create Edge Enabled Device without child devices [#11597]</span></span>
* <span data-ttu-id="01b15-489">Foi adicionado o cmdlet para gerar o token de SAS para o Hub IoT, um dispositivo ou um módulo.</span><span class="sxs-lookup"><span data-stu-id="01b15-489">Added cmdlet to generate SAS token for Iot Hub, device or module.</span></span>
* <span data-ttu-id="01b15-490">Foi adicionado um cmdlet para invocar a consulta de métricas de configuração.</span><span class="sxs-lookup"><span data-stu-id="01b15-490">Added cmdlet to invoke configuration metrics query.</span></span>
* <span data-ttu-id="01b15-491">Gerir implementações automáticas do IoT Edge em escala.</span><span class="sxs-lookup"><span data-stu-id="01b15-491">Manage IoT Edge automatic deployment at scale.</span></span> <span data-ttu-id="01b15-492">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="01b15-492">New cmdlets are:</span></span>
    - <span data-ttu-id="01b15-493">"Add-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="01b15-493">'Add-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="01b15-494">"Get-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="01b15-494">'Get-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="01b15-495">"Remove-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="01b15-495">'Remove-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="01b15-496">"Set-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="01b15-496">'Set-AzIotHubDeployment'</span></span>
* <span data-ttu-id="01b15-497">Foi adicionado um cmdlet para invocar uma consulta de métricas de implementação do IoT Edge.</span><span class="sxs-lookup"><span data-stu-id="01b15-497">Added cmdlet to invoke an IoT Edge deployment metrics query.</span></span>
* <span data-ttu-id="01b15-498">Foi adicionado um cmdlet para aplicar o conteúdo da configuração ao dispositivo edge especificado.</span><span class="sxs-lookup"><span data-stu-id="01b15-498">Added cmdlet to apply the configuration content to the specified edge device.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="01b15-499">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b15-499">Az.KeyVault</span></span>
* <span data-ttu-id="01b15-500">Foram removidos dois aliases: "New-AzKeyVaultCertificateAdministratorDetails" e "New-AzKeyVaultCertificateOrganizationDetails"</span><span class="sxs-lookup"><span data-stu-id="01b15-500">Removed two aliases: 'New-AzKeyVaultCertificateAdministratorDetails' and 'New-AzKeyVaultCertificateOrganizationDetails'</span></span>
* <span data-ttu-id="01b15-501">A eliminação recuperável foi ativada por predefinição ao criar um cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="01b15-501">Enabled soft delete by default when creating a key vault</span></span>
* <span data-ttu-id="01b15-502">Podem ser definidas regras de rede para governar a acessibilidade a partir de localizações na rede ao criar um cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="01b15-502">Network rules can be set to govern the accessibility from specific network locations when creating a key vault</span></span>
* <span data-ttu-id="01b15-503">Foi adicionado suporte para Bring Your Own Key (BYOK)</span><span class="sxs-lookup"><span data-stu-id="01b15-503">Added support to bring your own key (BYOK)</span></span>
    - <span data-ttu-id="01b15-504">"Add-AzKeyVaultKey" suporta a geração de chaves de intercâmbio de chaves</span><span class="sxs-lookup"><span data-stu-id="01b15-504">'Add-AzKeyVaultKey' supports generating a key exchange key</span></span>
    - <span data-ttu-id="01b15-505">"Get-AzKeyVaultKey" suporta a transferência de chaves públicas no formato PEM</span><span class="sxs-lookup"><span data-stu-id="01b15-505">'Get-AzKeyVaultKey' supports downloading a public key in PEM format</span></span>
* <span data-ttu-id="01b15-506">"KeyOps" foi atualizado como parte do documento de ajuda de "Add-AzKeyVaultKey"</span><span class="sxs-lookup"><span data-stu-id="01b15-506">Updated the 'KeyOps' part of the help document of 'Add-AzKeyVaultKey'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="01b15-507">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="01b15-507">Az.Monitor</span></span>
* <span data-ttu-id="01b15-508">Foi corrigido um erro em "Set-AzDiagnosticSettings"; a política de retenção não se aplicará a todas as categorias [#11589]</span><span class="sxs-lookup"><span data-stu-id="01b15-508">Fixed bug for 'Set-AzDiagnosticSettings', retention policy won't apply to all categories [#11589]</span></span>
* <span data-ttu-id="01b15-509">Suporte para critérios de disponibilidade de WebTest para alertas de métricas V2</span><span class="sxs-lookup"><span data-stu-id="01b15-509">Supported WebTest availability criteria for metric alert V2</span></span>
    - <span data-ttu-id="01b15-510">Novo "New-AzMetricAlertRuleV2Criteria": foi adicionada uma opção para criar critérios de disponibilidade WebTest</span><span class="sxs-lookup"><span data-stu-id="01b15-510">'New-AzMetricAlertRuleV2Criteria': an option to create webtest availability criteria was added</span></span>
    - <span data-ttu-id="01b15-511">"Add-AzMetricAlertRuleV2": suporta os novos critérios de disponibilidade de WebTest</span><span class="sxs-lookup"><span data-stu-id="01b15-511">'Add-AzMetricAlertRuleV2': supports the new webtest availability criteria</span></span>
* <span data-ttu-id="01b15-512">Foi removida a definição redundante de RetentionPolicy em PSLogProfile [#7608]</span><span class="sxs-lookup"><span data-stu-id="01b15-512">Removed redundant definition for RetentionPolicy in PSLogProfile [#7608]</span></span>
* <span data-ttu-id="01b15-513">Foram removidas as propriedades redundantes definidas em PSEventData [#11353]</span><span class="sxs-lookup"><span data-stu-id="01b15-513">Removed redundant properties difined in PSEventData [#11353]</span></span>
* <span data-ttu-id="01b15-514">O nome de "Get-AzLog" foi mudado para "Get-AzActivityLog"</span><span class="sxs-lookup"><span data-stu-id="01b15-514">Renamed 'Get-AzLog' to 'Get-AzActivityLog'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-515">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-515">Az.Network</span></span>
* <span data-ttu-id="01b15-516">Foi adicionado um atributo de alteração interruptiva para notificar que o comportamento predefinido da Zona vai ser alterado</span><span class="sxs-lookup"><span data-stu-id="01b15-516">Added breaking change attribute to notify that Zone default behaviour will be changed</span></span>
    - <span data-ttu-id="01b15-517">"New-AzPublicIpAddress"</span><span class="sxs-lookup"><span data-stu-id="01b15-517">'New-AzPublicIpAddress'</span></span>
    - <span data-ttu-id="01b15-518">"New-AzPublicIpPrefix"</span><span class="sxs-lookup"><span data-stu-id="01b15-518">'New-AzPublicIpPrefix'</span></span>
    - <span data-ttu-id="01b15-519">"New-AzLoadBalancerFrontendIpConfig"</span><span class="sxs-lookup"><span data-stu-id="01b15-519">'New-AzLoadBalancerFrontendIpConfig'</span></span>
* <span data-ttu-id="01b15-520">Foi adicionado suportado para um recurso de nível superior novo SecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="01b15-520">Added support for a new top level resource SecurityPartnerProvider</span></span>
    - <span data-ttu-id="01b15-521">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="01b15-521">New cmdlets added:</span></span>
        - <span data-ttu-id="01b15-522">New-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="01b15-522">New-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="01b15-523">Remove-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="01b15-523">Remove-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="01b15-524">Get-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="01b15-524">Get-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="01b15-525">Set-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="01b15-525">Set-AzSecurityPartnerProvider</span></span>
* <span data-ttu-id="01b15-526">Foi adicionado "RequiredZoneNames" em "PSPrivateLinkResource" e "GroupId" em "PSPrivateEndpointConnection”</span><span class="sxs-lookup"><span data-stu-id="01b15-526">Added 'RequiredZoneNames' on 'PSPrivateLinkResource' and 'GroupId' on 'PSPrivateEndpointConnection'</span></span>
* <span data-ttu-id="01b15-527">Foi corrigido o tipo incorreto do parâmetro SuccessThresholdRoundTripTimeMs para New-AzNetworkWatcherConnectionMonitorTestConfigurationObject</span><span class="sxs-lookup"><span data-stu-id="01b15-527">Fixed incorrect type of SuccessThresholdRoundTripTimeMs parameter for New-AzNetworkWatcherConnectionMonitorTestConfigurationObject</span></span>
* <span data-ttu-id="01b15-528">Foram atualizados os cmdlets VirtualWan para definir o valor predefinido do argumento AllowVnetToVnetTraffic como Verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="01b15-528">Updated VirtualWan cmdlets to set default value of AllowVnetToVnetTraffic argument to True.</span></span>
    - <span data-ttu-id="01b15-529">"New-AzVirtualWan"</span><span class="sxs-lookup"><span data-stu-id="01b15-529">'New-AzVirtualWan'</span></span>
    - <span data-ttu-id="01b15-530">"Update-AzVirtualWan"</span><span class="sxs-lookup"><span data-stu-id="01b15-530">'Update-AzVirtualWan'</span></span>
* <span data-ttu-id="01b15-531">Foram adicionados cmdlets para suportar o grupo de zonas DNS para pontos finais privados</span><span class="sxs-lookup"><span data-stu-id="01b15-531">Added new cmdlets to support DNS zone group for private endpoint</span></span>
    - <span data-ttu-id="01b15-532">"New-AzPrivateDnsZoneConfig"</span><span class="sxs-lookup"><span data-stu-id="01b15-532">'New-AzPrivateDnsZoneConfig'</span></span>
    - <span data-ttu-id="01b15-533">"Get-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="01b15-533">'Get-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="01b15-534">"New-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="01b15-534">'New-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="01b15-535">"Set-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="01b15-535">'Set-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="01b15-536">"Remove-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="01b15-536">'Remove-AzPrivateDnsZoneGroup'</span></span>
* <span data-ttu-id="01b15-537">Foram adicionados os parâmetros "DNSEnableProxy", "DNSRequireProxyForNetworkRules" e "DNSServers" a "AzureFirewall"</span><span class="sxs-lookup"><span data-stu-id="01b15-537">Added 'DNSEnableProxy', 'DNSRequireProxyForNetworkRules' and 'DNSServers' parameters to 'AzureFirewall'</span></span>
* <span data-ttu-id="01b15-538">Foram adicionados os parâmetros "EnableDnsProxy", "DnsProxyNotRequiredForNetworkRule" e "DnsServer" a "AzureFirewall"</span><span class="sxs-lookup"><span data-stu-id="01b15-538">Added 'EnableDnsProxy', 'DnsProxyNotRequiredForNetworkRule' and 'DnsServer' parameters to 'AzureFirewall'</span></span>
    - <span data-ttu-id="01b15-539">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="01b15-539">Updated cmdlet:</span></span>
        - <span data-ttu-id="01b15-540">New-AzFirewall</span><span class="sxs-lookup"><span data-stu-id="01b15-540">New-AzFirewall</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="01b15-541">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-541">Az.OperationalInsights</span></span>
* <span data-ttu-id="01b15-542">O código legado foi atualizado para aplicar o SDK recém-gerado</span><span class="sxs-lookup"><span data-stu-id="01b15-542">Updated legacy code to apply new generated SDK</span></span>
* <span data-ttu-id="01b15-543">Foram eliminados cmdlets devido a APIs preteridas</span><span class="sxs-lookup"><span data-stu-id="01b15-543">Deleted cmdlets due to deprecated APIs</span></span>
    - <span data-ttu-id="01b15-544">"Get-AzOperationalInsightsSavedSearchResult" (alias "Get-AzOperationalInsightsSavedSearchResults")</span><span class="sxs-lookup"><span data-stu-id="01b15-544">'Get-AzOperationalInsightsSavedSearchResult' (alias 'Get-AzOperationalInsightsSavedSearchResults')</span></span>
    - <span data-ttu-id="01b15-545">"Get-AzOperationalInsightsSearchResult" (alias "Get-AzOperationalInsightsSearchResults")</span><span class="sxs-lookup"><span data-stu-id="01b15-545">'Get-AzOperationalInsightsSearchResult' (alias 'Get-AzOperationalInsightsSearchResults')</span></span>
    - <span data-ttu-id="01b15-546">"Get-AzOperationalInsightsLinkTarget" (alias "Get-AzOperationalInsightsLinkTargets")</span><span class="sxs-lookup"><span data-stu-id="01b15-546">'Get-AzOperationalInsightsLinkTarget' (alias 'Get-AzOperationalInsightsLinkTargets')</span></span>
* <span data-ttu-id="01b15-547">Foram adicionados parâmetros para "Set-AzOperationalInsightsWorkspace" e "New-AzOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="01b15-547">Added parameters for 'Set-AzOperationalInsightsWorkspace' and 'New-AzOperationalInsightsWorkspace'</span></span>
* <span data-ttu-id="01b15-548">Foram criados cmdlets para a Conta de Armazenamento Associada</span><span class="sxs-lookup"><span data-stu-id="01b15-548">Created cmdlets for Linked Stoarge Account</span></span>
* <span data-ttu-id="01b15-549">Foram criados cmdlets para Clusters e para o Serviço Associado</span><span class="sxs-lookup"><span data-stu-id="01b15-549">Created cmdlets for Clusters and Linked Service</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-550">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-550">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-551">O Azure Site Recovery adicionou suporte para proteger máquinas virtuais de grupo de colocação por proximidade para fornecedor do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-551">Azure Site Recovery added support for protecting proximity placement group virtual machines for Azure to Azure provider.</span></span>
* <span data-ttu-id="01b15-552">O Azure Site Recovery adicionou suporte para a replicação de zona para zona.</span><span class="sxs-lookup"><span data-stu-id="01b15-552">Azure Site Recovery added support for zone to zone replication.</span></span>
* <span data-ttu-id="01b15-553">O Azure Backup adicionou suporte para a retenção de longo prazo para Pontos de Recuperação de Partilhas de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-553">Azure Backup Added Long term retention support for Azure FileShare Recovery Points.</span></span>
* <span data-ttu-id="01b15-554">O Azure Backup adicionou propriedades de exclusão de discos à saída do cmdlet "Get-AzRecoveryServicesBackupItem".</span><span class="sxs-lookup"><span data-stu-id="01b15-554">Azure Backup Added disk exclusion properties to 'Get-AzRecoveryServicesBackupItem' cmdlet output.</span></span>
* <span data-ttu-id="01b15-555">Foi adicionado o ponto final privado para o ficheiro de credenciais de Cofre para o Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="01b15-555">Added private endpoint for Vault credential file for site recovery service.</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-556">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-556">Az.Resources</span></span>
* <span data-ttu-id="01b15-557">Foi adicionado um aviso de mensagem relativo a um atraso na vista ao criar uma Definição de Função nova</span><span class="sxs-lookup"><span data-stu-id="01b15-557">Added message warning about view delay when creating a new Role Definition</span></span>
* <span data-ttu-id="01b15-558">Os cmdlets de política foram alterados para produzir objetos de tipos compatíveis</span><span class="sxs-lookup"><span data-stu-id="01b15-558">Changed policy cmdlets to output strongly-typed objects</span></span>
* <span data-ttu-id="01b15-559">Foi removido o parâmetro "-TenantLevel" utilizado no cmdlet "Get-AzResourceLock" [#11335]</span><span class="sxs-lookup"><span data-stu-id="01b15-559">Removed '-TenantLevel' parameter used for on the 'Get-AzResourceLock' cmdlet [#11335]</span></span>
* <span data-ttu-id="01b15-560">"Remove-AzResourceGroup -Id ResourceId" foi corrigido [#9882]</span><span class="sxs-lookup"><span data-stu-id="01b15-560">Fixed 'Remove-AzResourceGroup -Id ResourceId'[#9882]</span></span>
* <span data-ttu-id="01b15-561">Foi adicionado um cmdlet novo para obter resultados de What-If de modelos do ARM no âmbito de um grupo de recursos: "Get-AzDeploymentResourceGroupWhatIfResult"</span><span class="sxs-lookup"><span data-stu-id="01b15-561">Added new cmdlet for getting ARM template What-If results at resource group scope: 'Get-AzDeploymentResourceGroupWhatIfResult'</span></span>
* <span data-ttu-id="01b15-562">Foi adicionado um cmdlet novo para obter resultados de What-If de modelos do ARM no âmbito de uma subscrição: "Get-AzDeploymentWhatIfResult"</span><span class="sxs-lookup"><span data-stu-id="01b15-562">Added new cmdlet for getting ARM template What-If results at subscription scope: 'Get-AzDeploymentWhatIfResult'</span></span>
   - <span data-ttu-id="01b15-563">Alias: "Get-AzSubscriptionDeploymentWhatIf"</span><span class="sxs-lookup"><span data-stu-id="01b15-563">Alias: 'Get-AzSubscriptionDeploymentWhatIf'</span></span>
* <span data-ttu-id="01b15-564">Os parâmetros "-WhatIf" e "-Confirm" foram substituídos para "New-AzDeployment" e "New-AzResourceGroupDeployment" para utilizar resultados de What-If de modelos do ARM</span><span class="sxs-lookup"><span data-stu-id="01b15-564">Overrode '-WhatIf' and '-Confirm' parameters for 'New-AzDeployment' and 'New-AzResourceGroupDeployment' to use ARM template What-If results</span></span>
* <span data-ttu-id="01b15-565">Foi adicionada a mensagem de descontinuação para o parâmetro "ApiVersion" em cmdlets implementados</span><span class="sxs-lookup"><span data-stu-id="01b15-565">Added deprecation message for 'ApiVersion' parameter in deployment cmdlets</span></span>
* <span data-ttu-id="01b15-566">Foi adicionada a capacidade para mostrar mensagens de erro melhoradas relativas a falhas em implementações</span><span class="sxs-lookup"><span data-stu-id="01b15-566">Added capability to show improved error messages for deployment failures</span></span>
* <span data-ttu-id="01b15-567">Foi adicionado o registo de correlationId para falhas em implementações</span><span class="sxs-lookup"><span data-stu-id="01b15-567">Added correlationId logging for deployment failures</span></span>
* <span data-ttu-id="01b15-568">Foi adicionada a propriedade "error" à saída do script de implementação</span><span class="sxs-lookup"><span data-stu-id="01b15-568">Added 'error' property to the deployment script output</span></span>
* <span data-ttu-id="01b15-569">O nuget Microsoft.Azure.Management.ResourceManager foi atualizado para "3.7.1-preview"</span><span class="sxs-lookup"><span data-stu-id="01b15-569">Updated nuget Microsoft.Azure.Management.ResourceManager to '3.7.1-preview'</span></span>
* <span data-ttu-id="01b15-570">Foram removidos casos de teste específicos, uma vez que a propriedade Error em DeploymentValidateResult foi alterada para apenas de leitura a partir de 3.7.1-preview</span><span class="sxs-lookup"><span data-stu-id="01b15-570">Removed specific test cases as Error property in DeploymentValidateResult has changed to readonly from nuget 3.7.1-preview</span></span>
* <span data-ttu-id="01b15-571">GenericResourceExpanded foi importado do SDK ResourceManager 3.7.1-preview</span><span class="sxs-lookup"><span data-stu-id="01b15-571">Brought GenericResourceExpanded from SDK ResourceManager 3.7.1-preview</span></span>
* <span data-ttu-id="01b15-572">Foi adicionado suporte para etiquetas a todos os cmdlets Get para implementação, bem como</span><span class="sxs-lookup"><span data-stu-id="01b15-572">Added tag support for all Get cmdlets for deployment, as well as</span></span>
    - <span data-ttu-id="01b15-573">"New-AzDeployment"</span><span class="sxs-lookup"><span data-stu-id="01b15-573">'New-AzDeployment'</span></span>
    - <span data-ttu-id="01b15-574">"New-AzManagementGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="01b15-574">'New-AzManagementGroupDeployment'</span></span>
    - <span data-ttu-id="01b15-575">"New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="01b15-575">'New-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="01b15-576">"New-AzTenantDeployment"</span><span class="sxs-lookup"><span data-stu-id="01b15-576">'New-AzTenantDeployment'</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="01b15-577">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="01b15-577">Az.ServiceFabric</span></span>
* <span data-ttu-id="01b15-578">Foi corrigido um erro na adição de certificados mediante a utilização de --SecretIdentifier que obtinha o thumbprint de certificado incorreto</span><span class="sxs-lookup"><span data-stu-id="01b15-578">Fixed bug in add certificate using --SecretIdentifier that was getting the wrong certificate thumbprint</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-579">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-579">Az.Sql</span></span>
* <span data-ttu-id="01b15-580">Foi melhorado o desempenho de:</span><span class="sxs-lookup"><span data-stu-id="01b15-580">Enhance performance of:</span></span>
    - <span data-ttu-id="01b15-581">"Set-AzSqlDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="01b15-581">'Set-AzSqlDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="01b15-582">"Set-AzSqlInstanceDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="01b15-582">'Set-AzSqlInstanceDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="01b15-583">"Remove-AzSqlDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="01b15-583">'Remove-AzSqlDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="01b15-584">"Remove-AzSqlInstanceDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="01b15-584">'Remove-AzSqlInstanceDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="01b15-585">"Enable-AzSqlDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="01b15-585">'Enable-AzSqlDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="01b15-586">"Enable-AzSqlInstanceDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="01b15-586">'Enable-AzSqlInstanceDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="01b15-587">"Disable-AzSqlDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="01b15-587">'Disable-AzSqlDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="01b15-588">"Disable-AzSqlInstanceDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="01b15-588">'Disable-AzSqlInstanceDatabaseSensitivityRecommendation'</span></span>
* <span data-ttu-id="01b15-589">Foi removida a validação do lado do cliente do parâmetro "RetentionDays" do cmdlet "Set-AzSqlDatabaseBackupShortTermRetentionPolicy"</span><span class="sxs-lookup"><span data-stu-id="01b15-589">Removed client-side validation of 'RetentionDays' parameter from cmdlet 'Set-AzSqlDatabaseBackupShortTermRetentionPolicy'</span></span>
* <span data-ttu-id="01b15-590">Auditoria a uma conta de armazenamento na Vnet; corrigido um erro ao criar uma função de Contribuidor de Dados de Blobs de Armazenamento.</span><span class="sxs-lookup"><span data-stu-id="01b15-590">Auditing to a storage account in Vnet, fixing a bug when creating a Storage Blob Data Contributor role.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-591">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-591">Az.Storage</span></span>
* <span data-ttu-id="01b15-592">Foi adicionado "-AsJob" ao cmdlet para obter/listar contas "Get-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="01b15-592">Added '-AsJob' to get/list account cmdlet 'Get-AzStorageAccount'</span></span>
* <span data-ttu-id="01b15-593">KeyVersion foi tornado opcional ao atualizar a conta de Armazenamento com KeyvaultEncryption, para suportar a rotação automática de chaves</span><span class="sxs-lookup"><span data-stu-id="01b15-593">Make KeyVersion to optional when update Storage account with KeyvaultEncryption, to support key auto-rotation</span></span>
    - <span data-ttu-id="01b15-594">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="01b15-594">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="01b15-595">Corrigida a remoção de falha do Diretório de Ficheiros do Azure com o pipeline</span><span class="sxs-lookup"><span data-stu-id="01b15-595">Fixed remove Azure File Directory fail with pipeline</span></span>
    - <span data-ttu-id="01b15-596">"Remove-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="01b15-596">'Remove-AzStorageDirectory'</span></span>
* <span data-ttu-id="01b15-597">Corrigido [#9880]: A definição do valor DefaultAction de NetWorkRule foi alterado para estar alinhado com o swagger.</span><span class="sxs-lookup"><span data-stu-id="01b15-597">Fixed [#9880]: Change NetWorkRule DefaultAction value defination to align with swagger.</span></span>
    - <span data-ttu-id="01b15-598">"Update-AzStorageAccountNetworkRuleSet"</span><span class="sxs-lookup"><span data-stu-id="01b15-598">'Update-AzStorageAccountNetworkRuleSet'</span></span>
    - <span data-ttu-id="01b15-599">"Get-AzStorageAccountNetworkRuleSet"</span><span class="sxs-lookup"><span data-stu-id="01b15-599">'Get-AzStorageAccountNetworkRuleSet'</span></span>
* <span data-ttu-id="01b15-600">Corrigido [#11624]: Ignorar regras duplicadas ao adicionar NetworkRules, para evitar falhas de servidores</span><span class="sxs-lookup"><span data-stu-id="01b15-600">Fixed [#11624]: Skip duplicated rules when add NetworkRules, to avoid server failure</span></span>
    - <span data-ttu-id="01b15-601">"Add-AzStorageAccountNetworkRule"</span><span class="sxs-lookup"><span data-stu-id="01b15-601">'Add-AzStorageAccountNetworkRule'</span></span>
* <span data-ttu-id="01b15-602">O SDK Microsoft.Azure.Cosmos.Table foi atualizado para 1.0.7</span><span class="sxs-lookup"><span data-stu-id="01b15-602">Upgraded Microsoft.Azure.Cosmos.Table SDK to 1.0.7</span></span>
* <span data-ttu-id="01b15-603">Foi adicionada uma mensagem de aviso para relembrar o utilizador para listar novamente com ContinuationToken apenas quando são devolvidos itens de peças na lista DataLake Gen2 Items,</span><span class="sxs-lookup"><span data-stu-id="01b15-603">Added a warning message to remind user to list again with ContinuationToken when only part items are returned in list DataLake Gen2 Items,</span></span>
    - <span data-ttu-id="01b15-604">"Get-AzDataLakeGen2ChildItem"</span><span class="sxs-lookup"><span data-stu-id="01b15-604">'Get-AzDataLakeGen2ChildItem'</span></span>
* <span data-ttu-id="01b15-605">Suportado para criar ou atualizar a conta de Armazenamento com a Autenticação do Active Directory Domain Service dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="01b15-605">Supported to create or update Storage account with Azure Files Active Directory Domain Service Authentication</span></span>
    -  <span data-ttu-id="01b15-606">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="01b15-606">'New-AzStorageAccount'</span></span>
    -  <span data-ttu-id="01b15-607">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="01b15-607">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="01b15-608">Suportado para os comandos "new" ou "list" de chaves de Kerberos da conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="01b15-608">Supported to new or list Kerberos keys of Storage account</span></span>
    -  <span data-ttu-id="01b15-609">"New-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="01b15-609">'New-AzStorageAccountKey'</span></span>
    -  <span data-ttu-id="01b15-610">"Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="01b15-610">'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="01b15-611">Suportada conta de Armazenamento de ativação pós-falha</span><span class="sxs-lookup"><span data-stu-id="01b15-611">Supported failover Storage account</span></span>
    - <span data-ttu-id="01b15-612">"Invoke-AzStorageAccountFailover"</span><span class="sxs-lookup"><span data-stu-id="01b15-612">'Invoke-AzStorageAccountFailover'</span></span>
* <span data-ttu-id="01b15-613">Ajuda de "Get-AzStorageBlobCopyState" atualizada</span><span class="sxs-lookup"><span data-stu-id="01b15-613">Updated help of 'Get-AzStorageBlobCopyState'</span></span>
* <span data-ttu-id="01b15-614">Ajuda de "Get-AzStorageFileCopyState" e "Start-AzStorageBlobCopy" atualizada</span><span class="sxs-lookup"><span data-stu-id="01b15-614">Updated help of 'Get-AzStorageFileCopyState' and 'Start-AzStorageBlobCopy'</span></span>
* <span data-ttu-id="01b15-615">Integração da biblioteca de cliente do Armazenamento v12 para cmdlets de Filas e Ficheiros</span><span class="sxs-lookup"><span data-stu-id="01b15-615">Integrated Storage client library v12 to Queue and File cmdlets</span></span>
* <span data-ttu-id="01b15-616">Alteração ao tipo de saída de CloudFile para AzureStorageFile; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="01b15-616">Changed output type from CloudFile to AzureStorageFile, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="01b15-617">"Get-AzStorageFile"</span><span class="sxs-lookup"><span data-stu-id="01b15-617">'Get-AzStorageFile'</span></span>
    - <span data-ttu-id="01b15-618">"Remove-AzStorageFile"</span><span class="sxs-lookup"><span data-stu-id="01b15-618">'Remove-AzStorageFile'</span></span>
    - <span data-ttu-id="01b15-619">"Get-AzStorageFileContent"</span><span class="sxs-lookup"><span data-stu-id="01b15-619">'Get-AzStorageFileContent'</span></span>
    - <span data-ttu-id="01b15-620">"Set-AzStorageFileContent"</span><span class="sxs-lookup"><span data-stu-id="01b15-620">'Set-AzStorageFileContent'</span></span>
    - <span data-ttu-id="01b15-621">"Start-AzStorageFileCopy"</span><span class="sxs-lookup"><span data-stu-id="01b15-621">'Start-AzStorageFileCopy'</span></span>
* <span data-ttu-id="01b15-622">Alteração ao tipo de saída de CloudFileDirectory para AzureStorageFileDirectory; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="01b15-622">Changed output type from CloudFileDirectory to AzureStorageFileDirectory, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="01b15-623">"New-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="01b15-623">'New-AzStorageDirectory'</span></span>
    - <span data-ttu-id="01b15-624">"Remove-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="01b15-624">'Remove-AzStorageDirectory'</span></span>
* <span data-ttu-id="01b15-625">Alteração ao tipo de saída de CloudFileShare para AzureStorageFileShare; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="01b15-625">Changed output type from CloudFileShare to AzureStorageFileShare, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="01b15-626">"Get-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="01b15-626">'Get-AzStorageShare'</span></span>
    - <span data-ttu-id="01b15-627">"New-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="01b15-627">'New-AzStorageShare'</span></span>
    - <span data-ttu-id="01b15-628">"Remove-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="01b15-628">'Remove-AzStorageShare'</span></span>
* <span data-ttu-id="01b15-629">Alteração ao tipo de saída de FileShareProperties para AzureStorageFileShare; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="01b15-629">Changed output type from FileShareProperties to AzureStorageFileShare, the original output will become a sub child property of the new output</span></span>
    - <span data-ttu-id="01b15-630">"Set-AzStorageShareQuota"</span><span class="sxs-lookup"><span data-stu-id="01b15-630">'Set-AzStorageShareQuota'</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="01b15-631">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="01b15-631">Az.TrafficManager</span></span>
* <span data-ttu-id="01b15-632">Corrigido o nome de perfil errado na saída verbosa de "DisableAzureTrafficManagerEndpoint"</span><span class="sxs-lookup"><span data-stu-id="01b15-632">Fixed incorrect profile name in 'DisableAzureTrafficManagerEndpoint' verbose output</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="01b15-633">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-633">Az.Websites</span></span>
* <span data-ttu-id="01b15-634">Corrigido um erro ortográfico na ajuda de "Update-AzWebAppAccessRestrictionConfig".</span><span class="sxs-lookup"><span data-stu-id="01b15-634">Fixed typo on help of 'Update-AzWebAppAccessRestrictionConfig'.</span></span>

## <a name="380---april-2020"></a><span data-ttu-id="01b15-635">3.8.0 - Abril de 2020</span><span class="sxs-lookup"><span data-stu-id="01b15-635">3.8.0 - April 2020</span></span>
### <a name="highlights-since-the-last-release"></a><span data-ttu-id="01b15-636">Destaques desde a última versão</span><span class="sxs-lookup"><span data-stu-id="01b15-636">Highlights since the last release</span></span>
* <span data-ttu-id="01b15-637">Versões do Powershell suportadas pelo Az.Storage: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span><span class="sxs-lookup"><span data-stu-id="01b15-637">PowerShell versions that Az.Storage supports: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="01b15-638">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-638">Az.Accounts</span></span>
* <span data-ttu-id="01b15-639">Atualização do URL de inquérito do Azure PowerShell em "Resolve-AzError" [#11507]</span><span class="sxs-lookup"><span data-stu-id="01b15-639">Updated Azure PowerShell survey URL in 'Resolve-AzError' [#11507]</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="01b15-640">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="01b15-640">Az.ApiManagement</span></span>
* <span data-ttu-id="01b15-641">Adicionado aviso de alteração interruptiva para a alteração de resultados de cmdlets de Ficheiro do Azure numa versão futura</span><span class="sxs-lookup"><span data-stu-id="01b15-641">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="01b15-642">Documentação atualizada de "Set-AzApiManagementGroup" para especificar o parâmetro GroupId</span><span class="sxs-lookup"><span data-stu-id="01b15-642">'Set-AzApiManagementGroup' Updated documentation to specify the GroupId parameter</span></span>

#### <a name="azcdn"></a><span data-ttu-id="01b15-643">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="01b15-643">Az.Cdn</span></span>
* <span data-ttu-id="01b15-644">Correção da apresentação do SKU de preços relacionados com ChinaCDN</span><span class="sxs-lookup"><span data-stu-id="01b15-644">Fixed ChinaCDN related pricing SKU display</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="01b15-645">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="01b15-645">Az.CognitiveServices</span></span>
* <span data-ttu-id="01b15-646">Suporte para Identidade, Encriptação, UserOwnedStorage</span><span class="sxs-lookup"><span data-stu-id="01b15-646">Supported Identity, Encryption, UserOwnedStorage</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-647">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-647">Az.Compute</span></span>
* <span data-ttu-id="01b15-648">Adicionado o cmdlet "Set-AzVmssOrchestrationServiceState".</span><span class="sxs-lookup"><span data-stu-id="01b15-648">Added 'Set-AzVmssOrchestrationServiceState' cmdlet.</span></span>
* <span data-ttu-id="01b15-649">"Get-AzVmss" com -InstanceView mostra os estados de OrchestrationService.</span><span class="sxs-lookup"><span data-stu-id="01b15-649">'Get-AzVmss' with -InstanceView shows OrchestrationService states.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="01b15-650">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="01b15-650">Az.IotHub</span></span>
* <span data-ttu-id="01b15-651">Gestão da configuração do dispositivo duplo de IoT. Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="01b15-651">Manage IoT device twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="01b15-652">"Get-AzIotHubDeviceTwin"</span><span class="sxs-lookup"><span data-stu-id="01b15-652">'Get-AzIotHubDeviceTwin'</span></span>
    - <span data-ttu-id="01b15-653">"Update-AzIotHubDeviceTwin"</span><span class="sxs-lookup"><span data-stu-id="01b15-653">'Update-AzIotHubDeviceTwin'</span></span>
* <span data-ttu-id="01b15-654">Adicionado cmdlet para invocar o método direto num dispositivo num hub IoT.</span><span class="sxs-lookup"><span data-stu-id="01b15-654">Added cmdlet to invoke direct method on a device in an Iot Hub.</span></span>
* <span data-ttu-id="01b15-655">Gestão da configuração do módulo duplo do dispositivo de IoT. Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="01b15-655">Manage IoT device module twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="01b15-656">"Get-AzIotHubModuleTwin"</span><span class="sxs-lookup"><span data-stu-id="01b15-656">'Get-AzIotHubModuleTwin'</span></span>
    - <span data-ttu-id="01b15-657">"Update-AzIotHubModuleTwin"</span><span class="sxs-lookup"><span data-stu-id="01b15-657">'Update-AzIotHubModuleTwin'</span></span>
* <span data-ttu-id="01b15-658">Gestão da configuração da gestão automática de dispositivos IoT em escala.</span><span class="sxs-lookup"><span data-stu-id="01b15-658">Manage IoT automatic device management configuration at scale.</span></span> <span data-ttu-id="01b15-659">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="01b15-659">New cmdlets are:</span></span>
    - <span data-ttu-id="01b15-660">"Add-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="01b15-660">'Add-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="01b15-661">"Get-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="01b15-661">'Get-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="01b15-662">"Remove-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="01b15-662">'Remove-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="01b15-663">"Set-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="01b15-663">'Set-AzIotHubConfiguration'</span></span>
* <span data-ttu-id="01b15-664">Adicionado cmdlet para invocar um método de módulo de periferia num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="01b15-664">Added cmdlet to invoke an edge module method in an Iot Hub.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="01b15-665">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b15-665">Az.KeyVault</span></span>
* <span data-ttu-id="01b15-666">Adicionado um novo cmdlet "Update-AzKeyVault" que pode permitir a eliminação recuperável e a proteção contra remoções num cofre</span><span class="sxs-lookup"><span data-stu-id="01b15-666">Added a new cmdlet 'Update-AzKeyVault' that can enable soft delete and purge protection on a vault</span></span>
* <span data-ttu-id="01b15-667">Adicionado suporte para Microsoft.PowerShell.SecretManagement [#11178]</span><span class="sxs-lookup"><span data-stu-id="01b15-667">Added support to Microsoft.PowerShell.SecretManagement [#11178]</span></span>
* <span data-ttu-id="01b15-668">Correção do erro nos exemplos de "Remove-AzKeyVaultManagedStorageSasDefinition" [#11479]</span><span class="sxs-lookup"><span data-stu-id="01b15-668">Fixed error in the examples of 'Remove-AzKeyVaultManagedStorageSasDefinition' [#11479]</span></span>
* <span data-ttu-id="01b15-669">Adicionado suporte para o ponto final privado</span><span class="sxs-lookup"><span data-stu-id="01b15-669">Added support to private endpoint</span></span>

#### <a name="azmaintenance"></a><span data-ttu-id="01b15-670">Az.Maintenance</span><span class="sxs-lookup"><span data-stu-id="01b15-670">Az.Maintenance</span></span>
* <span data-ttu-id="01b15-671">Publicação da versão de lançamento dos cmdlets de Manutenção para Disponibilidade Geral</span><span class="sxs-lookup"><span data-stu-id="01b15-671">Publishing release version of Maintenance cmdlets for GA</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="01b15-672">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="01b15-672">Az.Monitor</span></span>
* <span data-ttu-id="01b15-673">Adicionados cmdlets para o âmbito de ligação privada</span><span class="sxs-lookup"><span data-stu-id="01b15-673">Added cmdlets for private link scope</span></span>
    - <span data-ttu-id="01b15-674">"Get-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="01b15-674">'Get-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="01b15-675">"Remove-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="01b15-675">'Remove-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="01b15-676">"New-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="01b15-676">'New-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="01b15-677">"Update-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="01b15-677">'Update-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="01b15-678">"Get-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="01b15-678">'Get-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="01b15-679">"New-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="01b15-679">'New-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="01b15-680">"Remove-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="01b15-680">'Remove-AzInsightsPrivateLinkScopedResource'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-681">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-681">Az.Network</span></span>
* <span data-ttu-id="01b15-682">Atualização dos cmdlets para permitir a ligação num IP privado para o Gateway de Rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="01b15-682">Updated cmdlets to enable connection on private IP for Virtual Network Gateway.</span></span>
    - <span data-ttu-id="01b15-683">"New-AzVirtualNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="01b15-683">'New-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="01b15-684">"Set-AzVirtualNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="01b15-684">'Set-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="01b15-685">"New-AzVirtualNetworkGatewayConnection"</span><span class="sxs-lookup"><span data-stu-id="01b15-685">'New-AzVirtualNetworkGatewayConnection'</span></span>
    - <span data-ttu-id="01b15-686">"Set-AzVirtualNetworkGatewayConnection"</span><span class="sxs-lookup"><span data-stu-id="01b15-686">'Set-AzVirtualNetworkGatewayConnection'</span></span>
* <span data-ttu-id="01b15-687">Atualização dos cmdlets para permitir LocalNetworkGateways e VpnSites com base em FQDN</span><span class="sxs-lookup"><span data-stu-id="01b15-687">Updated cmdlets to enable FQDN based LocalNetworkGateways and VpnSites</span></span>
    - <span data-ttu-id="01b15-688">"New-AzLocalNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="01b15-688">'New-AzLocalNetworkGateway'</span></span>
    - <span data-ttu-id="01b15-689">"New-AzVpnSiteLink"</span><span class="sxs-lookup"><span data-stu-id="01b15-689">'New-AzVpnSiteLink'</span></span>
* <span data-ttu-id="01b15-690">Adicionado suporte para a família de endereços IPv6 em ExpressRouteCircuitConnectionConfig (Alcance Global)</span><span class="sxs-lookup"><span data-stu-id="01b15-690">Added support for IPv6 address family in ExpressRouteCircuitConnectionConfig (Global Reach)</span></span>
    - <span data-ttu-id="01b15-691">Adicionado "Set-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="01b15-691">Added 'Set-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="01b15-692">permite a definição de todas as propriedades existentes, incluindo o IPv6CircuitConnectionProperties</span><span class="sxs-lookup"><span data-stu-id="01b15-692">allows setting of all the existing properties including the IPv6CircuitConnectionProperties</span></span>
    - <span data-ttu-id="01b15-693">Atualização de "Add-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="01b15-693">Updated 'Add-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="01b15-694">Adicionado outro parâmetro opcional AddressPrefixType para especificar a família de endereços do prefixo de endereço</span><span class="sxs-lookup"><span data-stu-id="01b15-694">Added another optional parameter AddressPrefixType to specify the address family of address prefix</span></span>
* <span data-ttu-id="01b15-695">Atualização dos cmdlets para permitir a definição do Tempo Limite de DPD nas Ligações do Gateway de Rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="01b15-695">Updated cmdlets to enable setting of DPD Timeout on Virtual Network Gateway Connections.</span></span>
    - <span data-ttu-id="01b15-696">New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-696">New-AzVirtualNetworkGatewayConnection</span></span>
    - <span data-ttu-id="01b15-697">Set-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-697">Set-AzVirtualNetworkGatewayConnection</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="01b15-698">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-698">Az.PolicyInsights</span></span>
* <span data-ttu-id="01b15-699">Adicionado o cmdlet "Start-AzPolicyComplianceScan" para acionar análises de conformidade de políticas</span><span class="sxs-lookup"><span data-stu-id="01b15-699">Added 'Start-AzPolicyComplianceScan' cmdlet for triggering policy compliance scans</span></span>
* <span data-ttu-id="01b15-700">Adição de definição de políticas, definição de conjuntos e versões de atribuição ao resultado de "Get-AzPolicyState"</span><span class="sxs-lookup"><span data-stu-id="01b15-700">Added policy definition, set definition, and assignment versions to 'Get-AzPolicyState' output</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="01b15-701">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="01b15-701">Az.ServiceFabric</span></span>
* <span data-ttu-id="01b15-702">Melhorias da formatação e usabilidade do código dos exemplos de "New-AzServiceFabricCluster"</span><span class="sxs-lookup"><span data-stu-id="01b15-702">Improved code formatting and usability of 'New-AzServiceFabricCluster' examples</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-703">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-703">Az.Sql</span></span>
* <span data-ttu-id="01b15-704">Adicionados os cmdlets "Get-AzSqlInstanceOperation" e "Stop-AzSqlInstanceOperation"</span><span class="sxs-lookup"><span data-stu-id="01b15-704">Added cmdlets 'Get-AzSqlInstanceOperation' and 'Stop-AzSqlInstanceOperation'</span></span>
* <span data-ttu-id="01b15-705">Suporte de auditorias a uma conta de armazenamento numa VNet.</span><span class="sxs-lookup"><span data-stu-id="01b15-705">Supported auditing to a storage account in VNet.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-706">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-706">Az.Storage</span></span>
* <span data-ttu-id="01b15-707">Adicionado aviso de alteração interruptiva para a alteração de resultados de cmdlets de Ficheiro do Azure numa versão futura</span><span class="sxs-lookup"><span data-stu-id="01b15-707">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="01b15-708">Suportado novo SkuName StandardGZRS, StandardRAGZRS ao criar/atualizar a Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="01b15-708">Supported new SkuName StandardGZRS, StandardRAGZRS when create/update Storage account</span></span>
    - <span data-ttu-id="01b15-709">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="01b15-709">'New-AzStorageAccount'</span></span>
    - <span data-ttu-id="01b15-710">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="01b15-710">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="01b15-711">Suportado o DataLake Gen2</span><span class="sxs-lookup"><span data-stu-id="01b15-711">Supported DataLake Gen2</span></span>
    - <span data-ttu-id="01b15-712">"New-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="01b15-712">'New-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="01b15-713">"Get-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="01b15-713">'Get-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="01b15-714">"Get-AzDataLakeGen2ChildItem"</span><span class="sxs-lookup"><span data-stu-id="01b15-714">'Get-AzDataLakeGen2ChildItem'</span></span>
    - <span data-ttu-id="01b15-715">"Move-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="01b15-715">'Move-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="01b15-716">"Set-AzDataLakeGen2ItemAclObject"</span><span class="sxs-lookup"><span data-stu-id="01b15-716">'Set-AzDataLakeGen2ItemAclObject'</span></span>
    - <span data-ttu-id="01b15-717">"Update-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="01b15-717">'Update-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="01b15-718">"Get-AzDataLakeGen2ItemContent"</span><span class="sxs-lookup"><span data-stu-id="01b15-718">'Get-AzDataLakeGen2ItemContent'</span></span>
    - <span data-ttu-id="01b15-719">"Remove-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="01b15-719">'Remove-AzDataLakeGen2Item'</span></span>

## <a name="0100-preview---april-2020"></a><span data-ttu-id="01b15-720">0.10.0-preview - Abril de 2020</span><span class="sxs-lookup"><span data-stu-id="01b15-720">0.10.0-preview - April 2020</span></span>
### <a name="general"></a><span data-ttu-id="01b15-721">Geral</span><span class="sxs-lookup"><span data-stu-id="01b15-721">General</span></span>
* <span data-ttu-id="01b15-722">Os módulos Az já estão disponíveis em pré-visualização no Azure Stack Hub.</span><span class="sxs-lookup"><span data-stu-id="01b15-722">Az modules is now available in preview on Azure Stack Hub.</span></span> <span data-ttu-id="01b15-723">Isto permite a compatibilidade entre plataformas diferentes com o Linux e macOS.</span><span class="sxs-lookup"><span data-stu-id="01b15-723">This allows for cross-platform compatibility with Linux and macOs.</span></span> <span data-ttu-id="01b15-724">Agora, o Azure Stack Hub suporta o PowerShell Core com os módulos Az. Obtenha mais informações [aqui](https://aka.ms/az4AzureStack)</span><span class="sxs-lookup"><span data-stu-id="01b15-724">Azure Stack Hub now supports PowerShell core with the Az modules, more information [here](https://aka.ms/az4AzureStack)</span></span>
* <span data-ttu-id="01b15-725">Os módulos Az suportam o perfil 2019-03-01-hybrid:</span><span class="sxs-lookup"><span data-stu-id="01b15-725">Az modules support profile 2019-03-01-hybrid:</span></span>
  - <span data-ttu-id="01b15-726">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="01b15-726">Az.Billing</span></span>
  - <span data-ttu-id="01b15-727">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-727">Az.Compute</span></span>
  - <span data-ttu-id="01b15-728">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="01b15-728">Az.DataBoxEdge</span></span>
  - <span data-ttu-id="01b15-729">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="01b15-729">Az.EventHub</span></span>
  - <span data-ttu-id="01b15-730">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="01b15-730">Az.IotHub</span></span>
  - <span data-ttu-id="01b15-731">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b15-731">Az.KeyVault</span></span>
  - <span data-ttu-id="01b15-732">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="01b15-732">Az.Monitor</span></span>
  - <span data-ttu-id="01b15-733">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-733">Az.Network</span></span>
  - <span data-ttu-id="01b15-734">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-734">Az.Resources</span></span>
  - <span data-ttu-id="01b15-735">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-735">Az.Storage</span></span>
  - <span data-ttu-id="01b15-736">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-736">Az.Websites</span></span>
* <span data-ttu-id="01b15-737">Foram introduzidos três novos módulos do PowerShell para Az que funcionam com o Azure Stack Hub. São eles o Az.Databox, Az.IotHub e Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="01b15-737">Three new PowerShell modules for az have been introduced that work with Azure Stack Hub, which are Az.Databox, Az.IotHub, and Az.EventHub</span></span>
* <span data-ttu-id="01b15-738">Os comandos permanecem sensivelmente iguais, com pequenas alterações como, por exemplo, a alteração do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="01b15-738">Commands remain relatively the same, with minor changes such as changing AzureRM to Az</span></span>
* <span data-ttu-id="01b15-739">Veja uma ligação atualizada à documentação do PowerShell para o Azure Stack Hub [aqui](https://aka.ms/InstallASHPowerShell)</span><span class="sxs-lookup"><span data-stu-id="01b15-739">Updated link to PowerShell documentation for Azure Stack Hub can be found [here](https://aka.ms/InstallASHPowerShell)</span></span>

## <a name="370---march-2020"></a><span data-ttu-id="01b15-740">3.7.0 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="01b15-740">3.7.0 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="01b15-741">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-741">Az.Accounts</span></span>
* <span data-ttu-id="01b15-742">Foram corrigidos os parâmetros "Get-AzTenant"/"Get-AzDefault"/"Set-AzDefault" que emitiam uma NullReferenceException quando a sessão não estava iniciada [#10292]</span><span class="sxs-lookup"><span data-stu-id="01b15-742">Fixed 'Get-AzTenant'/'Get-AzDefault'/'Set-AzDefault' throw NullReferenceException when not login [#10292]</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-743">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-743">Az.Compute</span></span>
* <span data-ttu-id="01b15-744">Foram adicionados os seguintes parâmetros ao cmdlet "New-AzDiskConfig":</span><span class="sxs-lookup"><span data-stu-id="01b15-744">Added the following parameters to 'New-AzDiskConfig' cmdlet:</span></span>
    - <span data-ttu-id="01b15-745">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span><span class="sxs-lookup"><span data-stu-id="01b15-745">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span></span>
* <span data-ttu-id="01b15-746">A propriedade Encryption foi permitida para o parâmetro Target do cmdlet "New-AzGalleryImageVersion".</span><span class="sxs-lookup"><span data-stu-id="01b15-746">Allowed Encryption property to Target parameter of 'New-AzGalleryImageVersion' cmdlet.</span></span>
* <span data-ttu-id="01b15-747">Foi corrigido o problema de tempDisk para os cmdlets "Set-AzVmss" -Reimage e "Invoke-AzVMReimage".</span><span class="sxs-lookup"><span data-stu-id="01b15-747">Fixed tempDisk issue for 'Set-AzVmss' -Reimage and 'Invoke-AzVMReimage' cmdlets.</span></span> <span data-ttu-id="01b15-748">[#11354]</span><span class="sxs-lookup"><span data-stu-id="01b15-748">[#11354]</span></span>
* <span data-ttu-id="01b15-749">Foi adicionado suporte aos cmdlets abaixo para a nova Extensão SAP</span><span class="sxs-lookup"><span data-stu-id="01b15-749">Added support to below cmdlets for new SAP Extension</span></span>
    - <span data-ttu-id="01b15-750">"Set-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="01b15-750">'Set-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="01b15-751">"Get-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="01b15-751">'Get-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="01b15-752">"Remove-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="01b15-752">'Remove-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="01b15-753">"Update-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="01b15-753">'Update-AzVMAEMExtension'</span></span>
* <span data-ttu-id="01b15-754">Foram corrigidos os erros em exemplos do documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="01b15-754">Fixed errors in examples of help document</span></span>
* <span data-ttu-id="01b15-755">É apresentado o valor de cadeia exato para o PowerState da VM no formato de tabela.</span><span class="sxs-lookup"><span data-stu-id="01b15-755">Showed the exact string value for VM PowerState in the table format.</span></span>
* <span data-ttu-id="01b15-756">"New-AzVmssConfig": foi corrigida a serialização da propriedade AutomaticRepairs quando a opção SinglePlacementGroup está desativada.</span><span class="sxs-lookup"><span data-stu-id="01b15-756">'New-AzVmssConfig': fixed serialization of AutomaticRepairs property when SinglePlacementGroup is disabled.</span></span> <span data-ttu-id="01b15-757">[#11257]</span><span class="sxs-lookup"><span data-stu-id="01b15-757">[#11257]</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="01b15-758">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="01b15-758">Az.DataFactory</span></span>
* <span data-ttu-id="01b15-759">Atualização da versão do SDK .Net do ADF para 4.8.0</span><span class="sxs-lookup"><span data-stu-id="01b15-759">Updated ADF .Net SDK version to 4.8.0</span></span>
* <span data-ttu-id="01b15-760">Foram adicionados parâmetros opcionais ao comando "Invoke-AzDataFactoryV2Pipeline" para suportar uma nova execução</span><span class="sxs-lookup"><span data-stu-id="01b15-760">Added optional parameters to 'Invoke-AzDataFactoryV2Pipeline' command to support rerun</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="01b15-761">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="01b15-761">Az.DataLakeStore</span></span>
* <span data-ttu-id="01b15-762">Foi adicionada a descrição da alteração interruptiva para "Export-AzDataLakeStoreItem" e "Import-AzDataLakeStoreItem"</span><span class="sxs-lookup"><span data-stu-id="01b15-762">Added breaking change description for 'Export-AzDataLakeStoreItem' and 'Import-AzDataLakeStoreItem'</span></span>
* <span data-ttu-id="01b15-763">Foi adicionada a opção de codificação de bytes para "New-AzDataLakeStoreItem", "Add-AzDAtaLakeStoreItemContent" e "Get-AzDAtaLakeStoreItemContent"</span><span class="sxs-lookup"><span data-stu-id="01b15-763">Added option of Byte encoding for 'New-AzDataLakeStoreItem', 'Add-AzDAtaLakeStoreItemContent', and 'Get-AzDAtaLakeStoreItemContent'</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="01b15-764">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="01b15-764">Az.HDInsight</span></span>
* <span data-ttu-id="01b15-765">É suportada a versão de TLS mínima suportada ao criar o cluster.</span><span class="sxs-lookup"><span data-stu-id="01b15-765">Supported specifying minimal supported TLS version when creating cluster.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="01b15-766">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="01b15-766">Az.IotHub</span></span>
* <span data-ttu-id="01b15-767">Foi adicionado suporte para gerir as definições distribuídas por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="01b15-767">Added support to manage distributed settings per-device.</span></span> <span data-ttu-id="01b15-768">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="01b15-768">New Cmdlets are:</span></span>
    - <span data-ttu-id="01b15-769">"Get-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="01b15-769">'Get-AzIotHubDistributedTracing'</span></span>
    - <span data-ttu-id="01b15-770">"Set-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="01b15-770">'Set-AzIotHubDistributedTracing'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="01b15-771">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b15-771">Az.KeyVault</span></span>
* <span data-ttu-id="01b15-772">Foram adicionados os atributos da alteração interruptiva a "New-AzKeyVault"</span><span class="sxs-lookup"><span data-stu-id="01b15-772">Added breaking change attributes to 'New-AzKeyVault'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="01b15-773">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="01b15-773">Az.Monitor</span></span>
* <span data-ttu-id="01b15-774">Foi atualizada a documentação de "New-AzScheduledQueryRuleLogMetricTrigger"</span><span class="sxs-lookup"><span data-stu-id="01b15-774">Updated documentation for 'New-AzScheduledQueryRuleLogMetricTrigger'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-775">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-775">Az.Network</span></span>
* <span data-ttu-id="01b15-776">Foram atualizados os cmdlets para permitir VirtualHubVnetConnections entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="01b15-776">Updated cmdlets to allow cross-tenant VirtualHubVnetConnections</span></span>
    - <span data-ttu-id="01b15-777">"New-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="01b15-777">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="01b15-778">"Update-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="01b15-778">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="01b15-779">"New-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="01b15-779">'New-AzVirtualHub'</span></span>
    - <span data-ttu-id="01b15-780">"Update-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="01b15-780">'Update-AzVirtualHub'</span></span>
* <span data-ttu-id="01b15-781">Foi removida a dependência do SDK do SQL Management</span><span class="sxs-lookup"><span data-stu-id="01b15-781">Removed Sql Management SDK dependency</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="01b15-782">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-782">Az.PolicyInsights</span></span>
* <span data-ttu-id="01b15-783">Mensagens de erro melhoradas</span><span class="sxs-lookup"><span data-stu-id="01b15-783">Improved error messages</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-784">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-784">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-785">O Azure Site Recovery adicionou suporte para nova proteção e atualização das propriedades de VM para Máquinas Virtuais encriptadas em disco do Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-785">Azure Site Recovery added support for doing reprotect and updated vm properties for Azure disk encrypted Virtual Machines.</span></span>
* <span data-ttu-id="01b15-786">Foi adicionada monitorização DR das propriedades VmwareToAzure ao Azure Site Recovery</span><span class="sxs-lookup"><span data-stu-id="01b15-786">Added Azure Site Recovery VmwareToAzure properties DR monitoring</span></span>
* <span data-ttu-id="01b15-787">O Azure Backup adicionou suporte para repetir a atualização de políticas para itens falhados.</span><span class="sxs-lookup"><span data-stu-id="01b15-787">Azure Backup added support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="01b15-788">O Azure Backup adicionou suporte para definições de exclusão do disco durante a cópia de segurança e o restauro.</span><span class="sxs-lookup"><span data-stu-id="01b15-788">Azure Backup Added support for disk exclusion settings during backup and restore.</span></span>
* <span data-ttu-id="01b15-789">O Azure Backup adicionou suporte para restaurar vários ficheiros/pastas no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="01b15-789">Azure Backup Added Support for Restoring Multiple files/folders in AzureFileShare</span></span>
* <span data-ttu-id="01b15-790">O Azure Backup adicionou suporte para o Resourcegroup especificado pelo utilizador durante a atualização da Política IaasVM</span><span class="sxs-lookup"><span data-stu-id="01b15-790">Azure Backup Added support for User-specified Resourcegroup support while updating IaasVM Policy</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-791">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-791">Az.Resources</span></span>
* <span data-ttu-id="01b15-792">Foi corrigido o parâmetro "Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType" para utilizar a apiVersion real dos recursos em vez da apiVersion predefinida [#11267]</span><span class="sxs-lookup"><span data-stu-id="01b15-792">Fixed 'Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType' to use actual apiVersion of resources instead of default apiVersion [#11267]</span></span>
* <span data-ttu-id="01b15-793">Foi adicionado o registo de correlationId para cenários de erro</span><span class="sxs-lookup"><span data-stu-id="01b15-793">Added correlationId logging for error scenarios</span></span>
* <span data-ttu-id="01b15-794">Pequena alteração à documentação referente a "Get-AzResourceLock".</span><span class="sxs-lookup"><span data-stu-id="01b15-794">Small documentation change to 'Get-AzResourceLock'.</span></span> <span data-ttu-id="01b15-795">Exemplo adicionado.</span><span class="sxs-lookup"><span data-stu-id="01b15-795">Added example.</span></span>
* <span data-ttu-id="01b15-796">Aspas com caráter de escape no valor de parâmetro "Get-AzADUser" [#11317]</span><span class="sxs-lookup"><span data-stu-id="01b15-796">Escaped single quote in parameter value of 'Get-AzADUser' [#11317]</span></span>
* <span data-ttu-id="01b15-797">Foram adicionados novos cmdlets aos Scripts de Implementação ("Get-AzDeploymentScript", "Get-AzDeploymentScriptLog", "Save-AzDeploymentScriptLog", "Remove-AzDeploymentScript")</span><span class="sxs-lookup"><span data-stu-id="01b15-797">Added new cmdlets for Deployment Scripts ('Get-AzDeploymentScript', 'Get-AzDeploymentScriptLog', 'Save-AzDeploymentScriptLog', 'Remove-AzDeploymentScript')</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-798">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-798">Az.Sql</span></span>
* <span data-ttu-id="01b15-799">Foi adicionado um parâmetro secundário legível a "Invoke-AzSqlDatabaseFailover"</span><span class="sxs-lookup"><span data-stu-id="01b15-799">Added readable secondary parameter to 'Invoke-AzSqlDatabaseFailover'</span></span>
* <span data-ttu-id="01b15-800">Foi adicionado o cmdlet "Disable-AzSqlServerActiveDirectoryOnlyAuthentication"</span><span class="sxs-lookup"><span data-stu-id="01b15-800">Added cmdlet 'Disable-AzSqlServerActiveDirectoryOnlyAuthentication'</span></span>
* <span data-ttu-id="01b15-801">Classificação de sensibilidade guardada ao classificar as colunas na base de dados.</span><span class="sxs-lookup"><span data-stu-id="01b15-801">Saved sensitivity rank when classifying columns in the database.</span></span>

#### <a name="azsupport"></a><span data-ttu-id="01b15-802">Az.Support</span><span class="sxs-lookup"><span data-stu-id="01b15-802">Az.Support</span></span>
* <span data-ttu-id="01b15-803">Disponibilidade geral do módulo "Az.Support"</span><span class="sxs-lookup"><span data-stu-id="01b15-803">General availability of 'Az.Support' module</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="01b15-804">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-804">Az.Websites</span></span>
* <span data-ttu-id="01b15-805">Foi adicionado suporte para utilizar Regras de Encaminhamento de Tráfego webapp através dos novos cmdlets abaixo</span><span class="sxs-lookup"><span data-stu-id="01b15-805">Added support for working with webapp Traffic Routing Rules via below new cmdlets</span></span>
    - <span data-ttu-id="01b15-806">"Get-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="01b15-806">'Get-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="01b15-807">"Update-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="01b15-807">'Update-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="01b15-808">"Add-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="01b15-808">'Add-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="01b15-809">"Remove-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="01b15-809">'Remove-AzWebAppTrafficRouting'</span></span>

## <a name="361---march-2020"></a><span data-ttu-id="01b15-810">3.6.1 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="01b15-810">3.6.1 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="01b15-811">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-811">Az.Accounts</span></span>
* <span data-ttu-id="01b15-812">Abrir a página de inquérito do Azure PowerShell em "Send-Feedback" [#11020]</span><span class="sxs-lookup"><span data-stu-id="01b15-812">Open Azure PowerShell survey page in 'Send-Feedback' [#11020]</span></span>
* <span data-ttu-id="01b15-813">Apresentar o URL de inquérito do Azure PowerShell em "Resolve-Error" [#11021]</span><span class="sxs-lookup"><span data-stu-id="01b15-813">Display Azure PowerShell survey URL in 'Resolve-Error' [#11021]</span></span>
* <span data-ttu-id="01b15-814">Adicionada versão de Az em UserAgent</span><span class="sxs-lookup"><span data-stu-id="01b15-814">Added Az version in UserAgent</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="01b15-815">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="01b15-815">Az.ApiManagement</span></span>
* <span data-ttu-id="01b15-816">Adicionado suporte para a obtenção e configuração do Domínio Personalizado no Ponto Final do DeveloperPortal [#11007]</span><span class="sxs-lookup"><span data-stu-id="01b15-816">Added support for retrieving and configuring Custom Domain on the DeveloperPortal Endpoint [#11007]</span></span>
* <span data-ttu-id="01b15-817">"Export-AzApiManagementApi" Adicionado suporte para a transferência da definição da API no formato JSON [#9987]</span><span class="sxs-lookup"><span data-stu-id="01b15-817">'Export-AzApiManagementApi' Added support for downloading Api Definition in Json format [#9987]</span></span>
* <span data-ttu-id="01b15-818">"Import-AzApiManagementApi" Adicionado suporte para a importação da definição de OpenApi 3.0 a partir de documento JSON</span><span class="sxs-lookup"><span data-stu-id="01b15-818">'Import-AzApiManagementApi' Added support for importing OpenApi 3.0 definition from Json document</span></span>
* <span data-ttu-id="01b15-819">"New-AzApiManagementIdentityProvider" e "Set-AzApiManagementIdentityProvider" Adicionado suporte para a configuração de "Inquilino de Início de Sessão" para Fornecedor de AAD B2C [#9784]</span><span class="sxs-lookup"><span data-stu-id="01b15-819">'New-AzApiManagementIdentityProvider' and 'Set-AzApiManagementIdentityProvider' Added support for configuring 'Signin Tenant' for AAD B2C Provider [#9784]</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="01b15-820">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="01b15-820">Az.DataLakeStore</span></span>
* <span data-ttu-id="01b15-821">Adicionada referência a System.Buffers explicitamente em csproj e psd1.</span><span class="sxs-lookup"><span data-stu-id="01b15-821">Added reference to System.Buffers explicitly in csproj and psd1.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="01b15-822">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="01b15-822">Az.IotHub</span></span>
* <span data-ttu-id="01b15-823">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="01b15-823">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="01b15-824">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="01b15-824">New Cmdlets are:</span></span>
    - <span data-ttu-id="01b15-825">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="01b15-825">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="01b15-826">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="01b15-826">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="01b15-827">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="01b15-827">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="01b15-828">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="01b15-828">'Set-AzIotHubDevice'</span></span>
* <span data-ttu-id="01b15-829">Adicionado suporte para a gestão de módulos num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="01b15-829">Added support to manage modules on a target Iot device in an Iot Hub.</span></span> <span data-ttu-id="01b15-830">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="01b15-830">New Cmdlets are:</span></span>
    - <span data-ttu-id="01b15-831">"Add-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="01b15-831">'Add-AzIotHubModule'</span></span>
    - <span data-ttu-id="01b15-832">"Get-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="01b15-832">'Get-AzIotHubModule'</span></span>
    - <span data-ttu-id="01b15-833">"Remove-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="01b15-833">'Remove-AzIotHubModule'</span></span>
    - <span data-ttu-id="01b15-834">"Set-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="01b15-834">'Set-AzIotHubModule'</span></span>
* <span data-ttu-id="01b15-835">Adicionado cmdlet para obter a cadeia de ligação de um dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="01b15-835">Added cmdlet to get the connection string of a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="01b15-836">Adicionado cmdlet para obter a cadeia de ligação de um módulo num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="01b15-836">Added cmdlet to get the connection string of a module on a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="01b15-837">Adicionado suporte para obter/definir dispositivo principal de um dispositivo IoT.</span><span class="sxs-lookup"><span data-stu-id="01b15-837">Added support to get/set parent device of an IoT device.</span></span> <span data-ttu-id="01b15-838">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="01b15-838">New Cmdlets are:</span></span>
    - <span data-ttu-id="01b15-839">"Get-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="01b15-839">'Get-AzIotHubDeviceParent'</span></span>
    - <span data-ttu-id="01b15-840">"Set-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="01b15-840">'Set-AzIotHubDeviceParent'</span></span>
* <span data-ttu-id="01b15-841">Adicionado suporte para gerir relações principal-subordinado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="01b15-841">Added support to manage device parent-child relationship.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="01b15-842">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="01b15-842">Az.Monitor</span></span>
* <span data-ttu-id="01b15-843">Corrigido o valor de saída de "Get-AzMetricDefinition" [#9714]</span><span class="sxs-lookup"><span data-stu-id="01b15-843">Fixed output value for 'Get-AzMetricDefinition' [#9714]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-844">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-844">Az.Network</span></span>
* <span data-ttu-id="01b15-845">Sdk Sql Management atualizado.</span><span class="sxs-lookup"><span data-stu-id="01b15-845">Updated Sql Management SDK.</span></span>
* <span data-ttu-id="01b15-846">Corrigido um problema de diferença de nomes na classe PrivateLinkServiceConnectionState.</span><span class="sxs-lookup"><span data-stu-id="01b15-846">Fixed a naming-difference issue in PrivateLinkServiceConnectionState class.</span></span>
    - <span data-ttu-id="01b15-847">Mapeamento do campo ActionsRequired para ActionRequired.</span><span class="sxs-lookup"><span data-stu-id="01b15-847">Mapping the field ActionsRequired to ActionRequired.</span></span>
* <span data-ttu-id="01b15-848">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="01b15-848">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-849">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-849">Az.Resources</span></span>
* <span data-ttu-id="01b15-850">Correção para erro de referência nula em "Get-AzRoleAssignment"</span><span class="sxs-lookup"><span data-stu-id="01b15-850">Fixed for null reference bug in 'Get-AzRoleAssignment'</span></span>
* <span data-ttu-id="01b15-851">Comutadores "-Force" e "-PassThru" marcados como opcionais em "Remove-AzADGroup" [#10849]</span><span class="sxs-lookup"><span data-stu-id="01b15-851">Marked switch '-Force' and '-PassThru' optional in 'Remove-AzADGroup' [#10849]</span></span>
* <span data-ttu-id="01b15-852">Corrigido problema em que "MailNickname" não devolve "Remove-AzADGroup" [#11167]</span><span class="sxs-lookup"><span data-stu-id="01b15-852">Fixed issue that 'MailNickname' doesn't return in 'Remove-AzADGroup' [#11167]</span></span>
* <span data-ttu-id="01b15-853">Corrigido problema em que a operação de pipe "Remove-AzADGroup" não funciona [#11171]</span><span class="sxs-lookup"><span data-stu-id="01b15-853">Fixed issue that 'Remove-AzADGroup' pipe operation doesn't work [#11171]</span></span>
* <span data-ttu-id="01b15-854">Correção para erro de referência nula em GetAzureRoleAssignmentCommand</span><span class="sxs-lookup"><span data-stu-id="01b15-854">Fixed for null reference bug in GetAzureRoleAssignmentCommand</span></span>
* <span data-ttu-id="01b15-855">Adicionados atributos de alterações interruptivas para futuras alterações a cmdlets de política</span><span class="sxs-lookup"><span data-stu-id="01b15-855">Added breaking change attributes for upcoming changes to policy cmdlets</span></span>
* <span data-ttu-id="01b15-856">"Get-AzResourceGroup" atualizado para realizar filtragem de etiqueta de grupo de recursos no lado do servidor</span><span class="sxs-lookup"><span data-stu-id="01b15-856">Updated 'Get-AzResourceGroup' to perform resource group tag filtering on server-side</span></span>
* <span data-ttu-id="01b15-857">Cmdlets Tag alargados para accept -ResourceId</span><span class="sxs-lookup"><span data-stu-id="01b15-857">Extended Tag cmdlets to accept -ResourceId</span></span>
    - <span data-ttu-id="01b15-858">Get-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="01b15-858">Get-AzTag -ResourceId</span></span>
    - <span data-ttu-id="01b15-859">New-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="01b15-859">New-AzTag -ResourceId</span></span>
    - <span data-ttu-id="01b15-860">Remove-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="01b15-860">Remove-AzTag -ResourceId</span></span>
* <span data-ttu-id="01b15-861">Adicionado cmdlet Tag novo</span><span class="sxs-lookup"><span data-stu-id="01b15-861">Added new Tag cmdlet</span></span>
    - <span data-ttu-id="01b15-862">Update-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="01b15-862">Update-AzTag -ResourceId</span></span>
* <span data-ttu-id="01b15-863">ScopedDeployment trazido de SDK 3.3.0</span><span class="sxs-lookup"><span data-stu-id="01b15-863">Brought ScopedDeployment from SDK 3.3.0</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-864">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-864">Az.Sql</span></span>
* <span data-ttu-id="01b15-865">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="01b15-865">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="01b15-866">Adicionado suporte para configuração de cópia de segurança de Retenção de Longo Prazo para Bases de Dados Geridas</span><span class="sxs-lookup"><span data-stu-id="01b15-866">Added support for Long Term Retention backup configuration for Managed Databases</span></span>
    - <span data-ttu-id="01b15-867">Política Get/Set numa base de dados gerida</span><span class="sxs-lookup"><span data-stu-id="01b15-867">Get/Set LTR policy on a managed database</span></span>
    - <span data-ttu-id="01b15-868">Obter cópia(s) de segurança LTR por base de dados gerida, por instância gerida ou por localização</span><span class="sxs-lookup"><span data-stu-id="01b15-868">Get LTR backup(s) by managed database, managed instance, or by location</span></span>
    - <span data-ttu-id="01b15-869">Remover uma cópia de segurança LTR</span><span class="sxs-lookup"><span data-stu-id="01b15-869">Remove an LTR backup</span></span>
    - <span data-ttu-id="01b15-870">Restaurar uma cópia de segurança LTR para criar uma base de dados gerida nova</span><span class="sxs-lookup"><span data-stu-id="01b15-870">Restore an LTR backup to create a new managed database</span></span>
* <span data-ttu-id="01b15-871">Adicionado MinimalTlsVersion a New-AzSqlServer e Set-AzSqlServer</span><span class="sxs-lookup"><span data-stu-id="01b15-871">Added MinimalTlsVersion to New-AzSqlServer and Set-AzSqlServer</span></span>
* <span data-ttu-id="01b15-872">Adicionado MinimalTlsVersion a New-AzSqlInstance e Set-AzSqlInstance</span><span class="sxs-lookup"><span data-stu-id="01b15-872">Added MinimalTlsVersion to New-AzSqlInstance and Set-AzSqlInstance</span></span>
* <span data-ttu-id="01b15-873">Versão de SDK SQL atualizada para Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-873">Bumped SQL SDK version for Az.Network</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-874">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-874">Az.Storage</span></span>
* <span data-ttu-id="01b15-875">AllowProtectedAppendWrite suportada em ImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="01b15-875">Supported AllowProtectedAppendWrite in ImmutabilityPolicy</span></span>
    - <span data-ttu-id="01b15-876">"Set-AzRmStorageContainerImmutabilityPolicy"</span><span class="sxs-lookup"><span data-stu-id="01b15-876">'Set-AzRmStorageContainerImmutabilityPolicy'</span></span>
* <span data-ttu-id="01b15-877">Adicionada uma mensagem de aviso de alteração interruptiva para alteração do tipo AzureStorageTable numa futura versão</span><span class="sxs-lookup"><span data-stu-id="01b15-877">Added breaking change warning message for AzureStorageTable type change in a future release</span></span>
    - <span data-ttu-id="01b15-878">"New-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="01b15-878">'New-AzStorageTable'</span></span>
    - <span data-ttu-id="01b15-879">"Get-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="01b15-879">'Get-AzStorageTable'</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="01b15-880">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-880">Az.Websites</span></span>
* <span data-ttu-id="01b15-881">Adicionado o parâmetro Tag para "New-AzAppServicePlan" e "Set-AzAppServicePlan"</span><span class="sxs-lookup"><span data-stu-id="01b15-881">Added Tag parameter for 'New-AzAppServicePlan' and 'Set-AzAppServicePlan'</span></span>
* <span data-ttu-id="01b15-882">Paragem da execução de cmdlet caso seja emitida uma exceção ao adicionar um domínio personalizado a um site</span><span class="sxs-lookup"><span data-stu-id="01b15-882">Stop cmdlet execution if an exception is thrown when adding a custom domain to a website</span></span>
* <span data-ttu-id="01b15-883">Adicionado suporte para a realização de operações para Serviços de Aplicações em grupos de recursos diferentes do Plano do Serviço de Aplicações</span><span class="sxs-lookup"><span data-stu-id="01b15-883">Added support to perform operations for App Services not in the same resource group as the App Service Plan</span></span>
* <span data-ttu-id="01b15-884">Aplicada restrição de acesso a WebApp/Função em diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="01b15-884">Applied access restriction to WebApp/Function in different resource groups</span></span>
* <span data-ttu-id="01b15-885">Corrigido problema para definir os nomes de anfitrião personalizados para WebAppSlots</span><span class="sxs-lookup"><span data-stu-id="01b15-885">Fixed issue to set custom hostnames for WebAppSlots</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="01b15-886">3.5.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="01b15-886">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="01b15-887">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="01b15-887">Highlights since the last major release</span></span>
* <span data-ttu-id="01b15-888">Telemetria do lado do cliente atualizada.</span><span class="sxs-lookup"><span data-stu-id="01b15-888">Updated client side telemetry.</span></span>
* <span data-ttu-id="01b15-889">O Az.IotHub adicionou cmdlets para suportar a gestão de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="01b15-889">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="01b15-890">O Az.SqlVirtualMachine adicionou cmdlets ao Serviço de Escuta do Grupo de Disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="01b15-890">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="01b15-891">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-891">Az.Accounts</span></span>
* <span data-ttu-id="01b15-892">SubscriptionId, TenantId e tempo de execução adicionados aos dados de telemetria do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="01b15-892">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="01b15-893">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="01b15-893">Az.Automation</span></span>
* <span data-ttu-id="01b15-894">Foi corrigido o erro no Exemplo 1 na documentação de referência de "New-AzAutomationSoftwareUpdateConfiguration"</span><span class="sxs-lookup"><span data-stu-id="01b15-894">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="01b15-895">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="01b15-895">Az.CognitiveServices</span></span>
* <span data-ttu-id="01b15-896">SDK atualizado para a versão 7.0</span><span class="sxs-lookup"><span data-stu-id="01b15-896">Updated SDK to 7.0</span></span>
* <span data-ttu-id="01b15-897">Mensagem de erro melhorada quando o servidor responde ao corpo vazio</span><span class="sxs-lookup"><span data-stu-id="01b15-897">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-898">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-898">Az.Compute</span></span>
* <span data-ttu-id="01b15-899">Valor vazio permitido para ProximityPlacementGroupId durante a atualização</span><span class="sxs-lookup"><span data-stu-id="01b15-899">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="01b15-900">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="01b15-900">Az.FrontDoor</span></span>
* <span data-ttu-id="01b15-901">Cmdlet adicionado para obter definições de regras geridas que podem ser utilizadas na WAF</span><span class="sxs-lookup"><span data-stu-id="01b15-901">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="01b15-902">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="01b15-902">Az.IotHub</span></span>
* <span data-ttu-id="01b15-903">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="01b15-903">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="01b15-904">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="01b15-904">New Cmdlets are:</span></span>
    - <span data-ttu-id="01b15-905">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="01b15-905">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="01b15-906">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="01b15-906">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="01b15-907">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="01b15-907">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="01b15-908">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="01b15-908">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="01b15-909">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b15-909">Az.KeyVault</span></span>
* <span data-ttu-id="01b15-910">Texto duplicado fixo para Add-AzKeyVaultKey.md</span><span class="sxs-lookup"><span data-stu-id="01b15-910">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="01b15-911">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="01b15-911">Az.Monitor</span></span>
* <span data-ttu-id="01b15-912">Descrição fixa do cmdlet Get-AzLog.</span><span class="sxs-lookup"><span data-stu-id="01b15-912">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="01b15-913">Foi adicionado um novo parâmetro chamado ActionGroupId ao comando "New-AzMetricAlertRuleV2".</span><span class="sxs-lookup"><span data-stu-id="01b15-913">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="01b15-914">O utilizador pode fornecer ActionGroupId(string) ou ActionGorup(ActivityLogAlertActionGroup).</span><span class="sxs-lookup"><span data-stu-id="01b15-914">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-915">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-915">Az.Network</span></span>
* <span data-ttu-id="01b15-916">Foi adicionada uma nota de parâmetro adicional para o parâmetro "-EnableProxyProtocol" para o cmdlet "New-AzPrivateLinkService".</span><span class="sxs-lookup"><span data-stu-id="01b15-916">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="01b15-917">Exemplo de FilterData fixo em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="01b15-917">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="01b15-918">Exemplo de Captura de Pacotes adicionado para capturar todos os pacotes internos e externos em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="01b15-918">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="01b15-919">Política do Azure Firewall suportada em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="01b15-919">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="01b15-920">Não foram adicionados novos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="01b15-920">No new cmdlets are added.</span></span> <span data-ttu-id="01b15-921">Simplificação da restrição da política de firewall em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="01b15-921">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-922">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-922">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-923">Suporte adicionado da funcionalidade Restaurar como ficheiros para Bases de Dados SQL.</span><span class="sxs-lookup"><span data-stu-id="01b15-923">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-924">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-924">Az.Resources</span></span>
* <span data-ttu-id="01b15-925">Cmdlets de implementação de modelos refatorizados</span><span class="sxs-lookup"><span data-stu-id="01b15-925">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="01b15-926">Foram adicionados novos cmdlets para gerir implementações no grupo de gestão: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="01b15-926">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="01b15-927">Foram adicionados novos cmdlets para gerir implementações no inquilino: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="01b15-927">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="01b15-928">Cmdlets \*-AzDeployment refatorizados para trabalhar especificamente no âmbito da subscrição</span><span class="sxs-lookup"><span data-stu-id="01b15-928">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="01b15-929">Foram criados aliases \*-AzSubscriptionDeployment para os cmdlets \*-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="01b15-929">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="01b15-930">"Update-AzADApplication" fixo quando o parâmetro "AvailableToOtherTenants" não está definido</span><span class="sxs-lookup"><span data-stu-id="01b15-930">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="01b15-931">ApplicationObjectWithoutCredentialParameterSet removido para evitar AmbiguousParameterSetException.</span><span class="sxs-lookup"><span data-stu-id="01b15-931">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="01b15-932">Ficheiros de ajuda regenerados</span><span class="sxs-lookup"><span data-stu-id="01b15-932">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-933">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-933">Az.Sql</span></span>
* <span data-ttu-id="01b15-934">Suporte adicionado para restauro para um ponto anterior no tempo entre subscrições nas Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="01b15-934">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="01b15-935">Suporte adicionado para alterar a geração de hardware das Instâncias Geridas de SQL existentes</span><span class="sxs-lookup"><span data-stu-id="01b15-935">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="01b15-936">Exemplos de ajuda "Update-AzSqlServerVulnerabilityAssessmentSetting" fixos: saída do parâmetro/propriedade - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="01b15-936">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="01b15-937">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="01b15-937">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="01b15-938">Cmdlets adicionados para o Serviço de Escuta do Grupo de Disponibilidade</span><span class="sxs-lookup"><span data-stu-id="01b15-938">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="01b15-939">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="01b15-939">Az.StorageSync</span></span>
* <span data-ttu-id="01b15-940">Conjuntos de carateres suportados atualizados em "Invoke-AzStorageSyncCompatibilityCheck".</span><span class="sxs-lookup"><span data-stu-id="01b15-940">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="01b15-941">3.4.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="01b15-941">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="01b15-942">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="01b15-942">Highlights since the last major release</span></span>
* <span data-ttu-id="01b15-943">Versão inicial Az.CosmosDB 0.1.0 lançada</span><span class="sxs-lookup"><span data-stu-id="01b15-943">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="01b15-944">Foi adicionado suporte para Az.Network ConnectionMonitor V2</span><span class="sxs-lookup"><span data-stu-id="01b15-944">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="01b15-945">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-945">Az.Accounts</span></span>
* <span data-ttu-id="01b15-946">Foi desativada a gravação automática de contexto quando AzureRmContext.json não está disponível</span><span class="sxs-lookup"><span data-stu-id="01b15-946">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="01b15-947">Atualização da referência ao Azure Powershell Common para a pré-visualização 1.3.5</span><span class="sxs-lookup"><span data-stu-id="01b15-947">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="01b15-948">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="01b15-948">Az.ApiManagement</span></span>
* <span data-ttu-id="01b15-949">**Get-AzApiManagementApiSchema** Foi corrigido ao obter Open-Api Schema associado a uma API   https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="01b15-949">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="01b15-950">**New-AzApiManagementProduct**\* e **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="01b15-950">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="01b15-951">Foi corrigida a documentação para https://github.com/Azure/azure-powershell/issues/10472</span><span class="sxs-lookup"><span data-stu-id="01b15-951">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="01b15-952">**Set-AzApiManagementApi** Exemplo adicionado para mostrar como atualizar o ServiceUrl com o cmdlet</span><span class="sxs-lookup"><span data-stu-id="01b15-952">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-953">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-953">Az.Compute</span></span>
* <span data-ttu-id="01b15-954">Foi limitado o número de estados de VM a 100 para evitar limitações quando Get-AzVM-Status é executado sem o nome da VM.</span><span class="sxs-lookup"><span data-stu-id="01b15-954">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="01b15-955">Foi adicionado o cmdlet Update-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="01b15-955">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="01b15-956">Foram adicionados os parâmetros EncryptionType e DiskEncryptionSetId aos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="01b15-956">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="01b15-957">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-957">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="01b15-958">Foi adicionado o parâmetro ColocationStatus ao cmdlet Get-AzProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="01b15-958">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="01b15-959">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="01b15-959">Az.DataFactory</span></span>
* <span data-ttu-id="01b15-960">Atualização do SDK .NET do ADF para a versão 4.7.0</span><span class="sxs-lookup"><span data-stu-id="01b15-960">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="01b15-961">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="01b15-961">Az.DeploymentManager</span></span>
* <span data-ttu-id="01b15-962">Adiciona operações LIST para os recursos</span><span class="sxs-lookup"><span data-stu-id="01b15-962">Adds LIST operations for resources</span></span>
* <span data-ttu-id="01b15-963">Adiciona a capacidade de realizar operações nos passos de Verificação de Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="01b15-963">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="01b15-964">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="01b15-964">Az.HDInsight</span></span>
* <span data-ttu-id="01b15-965">Foi corrigido o erro do documento de New-AzHDInsightCluster.</span><span class="sxs-lookup"><span data-stu-id="01b15-965">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="01b15-966">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b15-966">Az.KeyVault</span></span>
* <span data-ttu-id="01b15-967">Foi adicionado o alias do Nome ao atributo VaultName para tornar Remove-AzureKeyVault consistente com New-AzureKeyVault.</span><span class="sxs-lookup"><span data-stu-id="01b15-967">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-968">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-968">Az.Network</span></span>
* <span data-ttu-id="01b15-969">Foi adicionado um novo exemplo a Set-AzNetworkWatcherConfigFlowLog.md para demonstrar o cenário de desativação da Análise de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="01b15-969">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="01b15-970">Foi adicionado suporte para atribuir a configuração IP de gestão ao Azure Firewall, uma sub-rede dedicada e IP Público que a firewall utilizará no tráfego de gestão</span><span class="sxs-lookup"><span data-stu-id="01b15-970">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="01b15-971">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="01b15-971">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="01b15-972">Foi adicionado o parâmetro -ManagementPublicIpAddress (não obrigatório) que aceita um objeto de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="01b15-972">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="01b15-973">Foi adicionado o método SetManagementIpConfiguration no objeto de firewall. Requer uma sub-rede e um endereço IP Público como entrada. O nome da sub-rede tem de ser "AzureFirewallManagementSubnet"</span><span class="sxs-lookup"><span data-stu-id="01b15-973">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="01b15-974">Foram corrigidos os exemplos de Get-AzNetworkSecurityGroup para mostrar exemplos de NSGs em vez de interfaces de rede.</span><span class="sxs-lookup"><span data-stu-id="01b15-974">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="01b15-975">Foi corrigido um erro no comando New-AzVpnSite que estava a impedir o ID do recurso de concluir um parâmetro.</span><span class="sxs-lookup"><span data-stu-id="01b15-975">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="01b15-976">Foi adicionado suporte para a Configuração do URL em Reescrever Conjunto de Ações de Regras no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="01b15-976">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="01b15-977">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="01b15-977">New cmdlets added:</span></span>
        - <span data-ttu-id="01b15-978">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="01b15-978">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="01b15-979">Foram atualizados cmdlets com o parâmetro opcional - UrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="01b15-979">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="01b15-980">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="01b15-980">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="01b15-981">Foi adicionado suporte para os recursos do NetworkWatcher ConnectionMonitor versão 2</span><span class="sxs-lookup"><span data-stu-id="01b15-981">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="01b15-982">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-982">Az.PolicyInsights</span></span>
* <span data-ttu-id="01b15-983">Foi adicionado suporte para avaliar a conformidade antes de determinar o recurso a remediar</span><span class="sxs-lookup"><span data-stu-id="01b15-983">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="01b15-984">Foi adicionado o parâmetro "-ResourceDiscoverMode" a Start-AzPolicyRemediation</span><span class="sxs-lookup"><span data-stu-id="01b15-984">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="01b15-985">Foi adicionado o cmdlet Get-AzPolicyMetadata para obter os recursos de metadados da política</span><span class="sxs-lookup"><span data-stu-id="01b15-985">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="01b15-986">Get-AzPolicyState e Get-AzPolicyStateSummary atualizados para a versão da API 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="01b15-986">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-987">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-987">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-988">Foi adicionado suporte do Azure Site Recovery para remover um disco replicado.</span><span class="sxs-lookup"><span data-stu-id="01b15-988">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="01b15-989">O Azure Backup adicionou suporte para adicionar etiquetas ao criar um Cofre dos Serviços de Recuperação.</span><span class="sxs-lookup"><span data-stu-id="01b15-989">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-990">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-990">Az.Resources</span></span>
* <span data-ttu-id="01b15-991">-Scope foi tornado opcional nos cmdlets \*-AzPolicyAssignment com subscrição de contexto predefinida</span><span class="sxs-lookup"><span data-stu-id="01b15-991">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="01b15-992">Foram adicionados exemplos de criação de ADServicePrincipal com credenciais de palavras-passe e chaves</span><span class="sxs-lookup"><span data-stu-id="01b15-992">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-993">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-993">Az.Sql</span></span>
<span data-ttu-id="01b15-994">Foi corrigido o cmdlet New-AzSqlDatabaseSecondary para verificar a existência de PartnerDatabaseName em vez da existência de DatabaseName.</span><span class="sxs-lookup"><span data-stu-id="01b15-994">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-995">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-995">Az.Storage</span></span>
* <span data-ttu-id="01b15-996">Foi definido o suporte de Tipo de Chave de Encriptação na Tabela/Fila em Criar Conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="01b15-996">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="01b15-997">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="01b15-997">New-AzStorageAccount</span></span>
* <span data-ttu-id="01b15-998">Será apresentado RequestId quando StorageException não tiver ExtendedErrorInformation</span><span class="sxs-lookup"><span data-stu-id="01b15-998">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="01b15-999">Foi corrigido o exemplo 6 do cmdlet Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="01b15-999">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="01b15-1000">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-1000">Az.Websites</span></span>
* <span data-ttu-id="01b15-1001">Set-AzWebapp e Set-AzWebappSlot suportam as propriedades AlwaysOn, MinTls e FtpsState</span><span class="sxs-lookup"><span data-stu-id="01b15-1001">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="01b15-1002">Foi corrigido o problema em que a definição de HttpsOnly, juntamente com a alteração de AppservicePlan ao utilizar o único comando Set-AzWebApp, estava a repor HttpsOnly para o valor predefinido</span><span class="sxs-lookup"><span data-stu-id="01b15-1002">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="01b15-1003">3.3.0 – janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="01b15-1003">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="01b15-1004">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-1004">Az.Accounts</span></span>
* <span data-ttu-id="01b15-1005">Add-AzEnvironment e Set-AzEnvironment foram atualizados para aceitar os parâmetros AzureAttestationServiceEndpointResourceId e AzureAttestationServiceEndpointSuffix</span><span class="sxs-lookup"><span data-stu-id="01b15-1005">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="01b15-1006">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="01b15-1006">Az.Cdn</span></span>
* <span data-ttu-id="01b15-1007">Apresentação dos detalhes da resposta de erro no cmdlet New-AzCdnEndpoint</span><span class="sxs-lookup"><span data-stu-id="01b15-1007">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-1008">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-1008">Az.Compute</span></span>
* <span data-ttu-id="01b15-1009">Correção do cmdlet Set-AzVMCustomScriptExtension para uma VM com disco OD gerido sem perfil de SO.</span><span class="sxs-lookup"><span data-stu-id="01b15-1009">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="01b15-1010">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="01b15-1010">Az.ContainerInstance</span></span>
* <span data-ttu-id="01b15-1011">Foram corrigidos os nomes de parâmetros utilizados pelo exemplo de New-AzContainerGroup</span><span class="sxs-lookup"><span data-stu-id="01b15-1011">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="01b15-1012">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="01b15-1012">Az.DataBoxEdge</span></span>
* <span data-ttu-id="01b15-1013">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="01b15-1013">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="01b15-1014">Obter o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="01b15-1014">Get the Edge Storage Container</span></span>
* <span data-ttu-id="01b15-1015">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="01b15-1015">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="01b15-1016">Criar novo Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="01b15-1016">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="01b15-1017">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="01b15-1017">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="01b15-1018">Remover o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="01b15-1018">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="01b15-1019">Foi adicionado o cmdlet "Invoke-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="01b15-1019">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="01b15-1020">Invocar ação para atualizar os dados no Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="01b15-1020">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="01b15-1021">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="01b15-1021">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="01b15-1022">Obter a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="01b15-1022">Get the Edge Storage Account</span></span>
* <span data-ttu-id="01b15-1023">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="01b15-1023">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="01b15-1024">Criar nova Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="01b15-1024">Create new Edge Storage Account</span></span>
* <span data-ttu-id="01b15-1025">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="01b15-1025">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="01b15-1026">Remover a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="01b15-1026">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="01b15-1027">Invocar o cmdlet "Invoke-AzDataBoxEdgeShare"</span><span class="sxs-lookup"><span data-stu-id="01b15-1027">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="01b15-1028">Invocar ação para atualizar os dados na partilha</span><span class="sxs-lookup"><span data-stu-id="01b15-1028">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="01b15-1029">Foi adicionado o cmdlet "Set-AzDataBoxEdgeStorageAccountCredential"</span><span class="sxs-lookup"><span data-stu-id="01b15-1029">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="01b15-1030">Definição de AzDataBoxEdgeStorageAccountCredential</span><span class="sxs-lookup"><span data-stu-id="01b15-1030">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="01b15-1031">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="01b15-1031">Az.DataFactory</span></span>
* <span data-ttu-id="01b15-1032">Adição das propriedades AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId e VersionStatus para o cmd Get-AzDataFactoryV2IntegrationRuntime</span><span class="sxs-lookup"><span data-stu-id="01b15-1032">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="01b15-1033">Atualização do SDK .NET do ADF para a versão 4.6.0</span><span class="sxs-lookup"><span data-stu-id="01b15-1033">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="01b15-1034">Adição do parâmetro "PublicIPs" para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a criação de Azure-SSIS IR com endereços IP públicos estáticos.</span><span class="sxs-lookup"><span data-stu-id="01b15-1034">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="01b15-1035">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="01b15-1035">Az.DevTestLabs</span></span>
* <span data-ttu-id="01b15-1036">Remoção da ligação quebrada em Get-AzDtlAllowedVMSizesPolicy.md</span><span class="sxs-lookup"><span data-stu-id="01b15-1036">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="01b15-1037">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="01b15-1037">Az.EventHub</span></span>
* <span data-ttu-id="01b15-1038">Correção do problema 10634: Correção da referência de objeto nulo para remover eventhubnamespace</span><span class="sxs-lookup"><span data-stu-id="01b15-1038">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="01b15-1039">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="01b15-1039">Az.HDInsight</span></span>
* <span data-ttu-id="01b15-1040">Correção do erro Invoke-AzHDInsightHiveJob.md.</span><span class="sxs-lookup"><span data-stu-id="01b15-1040">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="01b15-1041">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="01b15-1041">Az.MachineLearning</span></span>
* <span data-ttu-id="01b15-1042">Foram removidos os cmdlets abaixo porque MachineLearningCompute já não está disponível</span><span class="sxs-lookup"><span data-stu-id="01b15-1042">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="01b15-1043">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="01b15-1043">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="01b15-1044">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="01b15-1044">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="01b15-1045">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="01b15-1045">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="01b15-1046">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="01b15-1046">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="01b15-1047">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="01b15-1047">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="01b15-1048">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="01b15-1048">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="01b15-1049">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="01b15-1049">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-1050">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-1050">Az.Network</span></span>
* <span data-ttu-id="01b15-1051">Atualização da dependência de Microsoft.Azure.Management.SQL da versão 1.36-preview para 1.37-preview</span><span class="sxs-lookup"><span data-stu-id="01b15-1051">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-1052">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-1052">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-1053">Alteração do Azure Site Recovery para suportar VMs de disco gerido com encriptação inativa com chaves geridas pelo cliente para o fornecedor do Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-1053">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="01b15-1054">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-1054">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="01b15-1055">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional ao nível do disco para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-1055">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="01b15-1056">Suporte do Azure Site Recovery para atualizar o item protegido por replicação com encriptação de discos e definir o mapa para HyperV para o Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-1056">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-1057">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-1057">Az.Resources</span></span>
* <span data-ttu-id="01b15-1058">Correção de um erro no documento de ajuda de "Remove-AzTag".</span><span class="sxs-lookup"><span data-stu-id="01b15-1058">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-1059">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-1059">Az.Sql</span></span>
* <span data-ttu-id="01b15-1060">Correção da funcionalidade dos cmdlets de linha de base do conjunto de avaliação de vulnerabilidades para funcionar na base de dados mestre da base de dados do Azure e limitá-la nas bases de dados do sistema de instância gerida</span><span class="sxs-lookup"><span data-stu-id="01b15-1060">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="01b15-1061">Correção de um erro ao criar o grupo de ativação pós-falha de instância SQL</span><span class="sxs-lookup"><span data-stu-id="01b15-1061">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="01b15-1062">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="01b15-1062">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="01b15-1063">Adição de DR como um novo tipo de Licença válido</span><span class="sxs-lookup"><span data-stu-id="01b15-1063">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-1064">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-1064">Az.Storage</span></span>
* <span data-ttu-id="01b15-1065">Adição de uma mensagem de aviso de alteração interruptiva para alteração do valor de DefaultAction numa futura versão</span><span class="sxs-lookup"><span data-stu-id="01b15-1065">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="01b15-1066">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="01b15-1066">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="01b15-1067">Suporte para obter a hora da última sincronização da conta de armazenamento ao executar get-AzureRMStorageAccount com o parâmetro -IncludeGeoReplicationStats</span><span class="sxs-lookup"><span data-stu-id="01b15-1067">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span>
    - <span data-ttu-id="01b15-1068">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="01b15-1068">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="01b15-1069">3.2.0 - Dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-1069">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="01b15-1070">Geral</span><span class="sxs-lookup"><span data-stu-id="01b15-1070">General</span></span>
* <span data-ttu-id="01b15-1071">Atualização das referências em .psd1 para utilizar o caminho relativo para todos os módulos</span><span class="sxs-lookup"><span data-stu-id="01b15-1071">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="01b15-1072">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-1072">Az.Accounts</span></span>
* <span data-ttu-id="01b15-1073">Definição do UserAgent correto para telemetria do lado do cliente para a pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="01b15-1073">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="01b15-1074">Apresentação de mensagem de erro amigável de utilizador quando o contexto é nulo na pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="01b15-1074">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="01b15-1075">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="01b15-1075">Az.Batch</span></span>
* <span data-ttu-id="01b15-1076">Correção do problema [10602](https://github.com/Azure/azure-powershell/issues/10602), em que **New-AzBatchPool** não enviava corretamente "VirtualMachineConfiguration.ContainerConfiguration" ou "VirtualMachineConfiguration.DataDisks" para o servidor.</span><span class="sxs-lookup"><span data-stu-id="01b15-1076">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="01b15-1077">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="01b15-1077">Az.DataFactory</span></span>
* <span data-ttu-id="01b15-1078">Atualização do SDK .NET do ADF para a versão 4.5.0</span><span class="sxs-lookup"><span data-stu-id="01b15-1078">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="01b15-1079">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="01b15-1079">Az.FrontDoor</span></span>
* <span data-ttu-id="01b15-1080">Adição do suporte de exclusão de regras geridas pela WAF</span><span class="sxs-lookup"><span data-stu-id="01b15-1080">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="01b15-1081">Adição de SocketAddr ao preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="01b15-1081">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="01b15-1082">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="01b15-1082">Az.HealthcareApis</span></span>
* <span data-ttu-id="01b15-1083">Processamento de Exceções</span><span class="sxs-lookup"><span data-stu-id="01b15-1083">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="01b15-1084">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b15-1084">Az.KeyVault</span></span>
* <span data-ttu-id="01b15-1085">Correção do erro em que era acedido um valor potencialmente não definido</span><span class="sxs-lookup"><span data-stu-id="01b15-1085">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="01b15-1086">Gestão de Certificados de Criptografia de Curva Elíptica</span><span class="sxs-lookup"><span data-stu-id="01b15-1086">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="01b15-1087">Adicionado suporte para especificar a Curva das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="01b15-1087">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="01b15-1088">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="01b15-1088">Az.Monitor</span></span>
* <span data-ttu-id="01b15-1089">Adição de um argumento opcional ao comando Adicionar Definições de Diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="01b15-1089">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="01b15-1090">Um argumento de opção que, se estiver presente, indica que a exportação para o Log Analytics deve ser feita para um esquema fixo (também conhecido como</span><span class="sxs-lookup"><span data-stu-id="01b15-1090">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="01b15-1091">tipo de dados dedicado)</span><span class="sxs-lookup"><span data-stu-id="01b15-1091">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-1092">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-1092">Az.Network</span></span>
* <span data-ttu-id="01b15-1093">Suporte para IpGroups na aplicação AzureFirewall, Nat e Regras de Rede.</span><span class="sxs-lookup"><span data-stu-id="01b15-1093">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-1094">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-1094">Az.Resources</span></span>
* <span data-ttu-id="01b15-1095">Correção de um problema em que a implementação do modelo não consegue ler um parâmetro se o nome estiver em conflito com um nome de parâmetro incorporado.</span><span class="sxs-lookup"><span data-stu-id="01b15-1095">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="01b15-1096">Os cmdlets da política foram atualizados para utilizar a nova versão de API 2019-09-01 que introduz suporte de agrupamento nas definições do conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="01b15-1096">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-1097">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-1097">Az.Sql</span></span>
* <span data-ttu-id="01b15-1098">Criação do armazenamento atualizada na ativação automática da Avaliação de Vulnerabilidades para StorageV2</span><span class="sxs-lookup"><span data-stu-id="01b15-1098">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-1099">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-1099">Az.Storage</span></span>
* <span data-ttu-id="01b15-1100">Suporte para gerar um token de SAS baseado na Identidade do Blob/Contentor com Contexto de Armazenamento baseado na autenticação OAuth</span><span class="sxs-lookup"><span data-stu-id="01b15-1100">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="01b15-1101">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="01b15-1101">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="01b15-1102">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="01b15-1102">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="01b15-1103">Suporte para revogar as Chaves de Delegação do Utilizador da Conta de Armazenamento, pelo que todos os tokens de SAS da identidade são revogados</span><span class="sxs-lookup"><span data-stu-id="01b15-1103">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="01b15-1104">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="01b15-1104">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="01b15-1105">Atualização de Microsoft.Azure.Management.Storage 14.2.0 para suportar a nova versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="01b15-1105">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="01b15-1106">Suporte de QuotaGiB (Quota de Partilha em Gibibye) para obter valores superiores a 5120 no plano de Gestão de cmdlets de Partilha de Ficheiros e foi adicionado o alias do parâmetro "Quota" ao parâmetro "QuotaGiB".</span><span class="sxs-lookup"><span data-stu-id="01b15-1106">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span>
    - <span data-ttu-id="01b15-1107">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="01b15-1107">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="01b15-1108">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="01b15-1108">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="01b15-1109">Adição do alias do parâmetro "QuotaGiB" ao parâmetro "Quota"</span><span class="sxs-lookup"><span data-stu-id="01b15-1109">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="01b15-1110">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="01b15-1110">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="01b15-1111">Correção do problema em que Set-AzStorageContainerAcl consegue limpar a Política de Acesso armazenada</span><span class="sxs-lookup"><span data-stu-id="01b15-1111">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="01b15-1112">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="01b15-1112">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="01b15-1113">3.1.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-1113">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="01b15-1114">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="01b15-1114">Highlights since the last major release</span></span>
* <span data-ttu-id="01b15-1115">Az.DataBoxEdge 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="01b15-1115">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="01b15-1116">Az.SqlVirtualMachine 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="01b15-1116">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-1117">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-1117">Az.Compute</span></span>
* <span data-ttu-id="01b15-1118">Funcionalidade de Reaplicação da VM</span><span class="sxs-lookup"><span data-stu-id="01b15-1118">VM Reapply feature</span></span>
    - <span data-ttu-id="01b15-1119">Adição do parâmetro Reapply ao cmdlet Set-AzVM</span><span class="sxs-lookup"><span data-stu-id="01b15-1119">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="01b15-1120">Funcionalidade AutomaticRepairs do Conjunto de Dimensionamento de VM:</span><span class="sxs-lookup"><span data-stu-id="01b15-1120">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="01b15-1121">Adição dos parâmetros EnableAutomaticRepair, AutomaticRepairGracePeriod e AutomaticRepairMaxInstanceRepairsPercent aos seguintes cmdlets:   New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="01b15-1121">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="01b15-1122">Suporte para imagens de galeria entre inquilinos para New-AzVM</span><span class="sxs-lookup"><span data-stu-id="01b15-1122">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="01b15-1123">Adição de "Spot" ao preenchedor de argumentos do parâmetro Priority nos cmdlets New-AzVM, New-AzVMConfig e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="01b15-1123">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="01b15-1124">Adição dos parâmetros DiskIOPSReadWrite e DiskMBpsReadWrite ao cmdlet Add-AzVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="01b15-1124">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="01b15-1125">Alteração do parâmetro SourceImageId do cmdlet New-AzGalleryImageVersion para opcional</span><span class="sxs-lookup"><span data-stu-id="01b15-1125">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="01b15-1126">Adição dos parâmetros OSDiskImage e DataDiskImage ao cmdlet New-AzGalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="01b15-1126">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="01b15-1127">Adição do parâmetro HyperVGeneration ao cmdlet New-AzGalleryImageDefinition</span><span class="sxs-lookup"><span data-stu-id="01b15-1127">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="01b15-1128">Adição dos parâmetros SkipExtensionsOnOverprovisionedVMs aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="01b15-1128">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="01b15-1129">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="01b15-1129">Az.DataBoxEdge</span></span>
* <span data-ttu-id="01b15-1130">Adição do cmdlet `Get-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="01b15-1130">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="01b15-1131">Obter a Encomenda</span><span class="sxs-lookup"><span data-stu-id="01b15-1131">Get the Order</span></span>
* <span data-ttu-id="01b15-1132">Adição do cmdlet `New-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="01b15-1132">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="01b15-1133">Criar nova Encomenda</span><span class="sxs-lookup"><span data-stu-id="01b15-1133">Create new Order</span></span>
* <span data-ttu-id="01b15-1134">Adição do cmdlet `Remove-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="01b15-1134">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="01b15-1135">Remover a Encomenda</span><span class="sxs-lookup"><span data-stu-id="01b15-1135">Remove the Order</span></span>
* <span data-ttu-id="01b15-1136">Alteração no cmdlet `New-AzDataBoxEdgeShare`</span><span class="sxs-lookup"><span data-stu-id="01b15-1136">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="01b15-1137">Agora cria uma Partilha Local</span><span class="sxs-lookup"><span data-stu-id="01b15-1137">Now creates Local Share</span></span>
* <span data-ttu-id="01b15-1138">Adição do cmdlet `Set-AzDataBoxEdgeRole`</span><span class="sxs-lookup"><span data-stu-id="01b15-1138">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="01b15-1139">Agora, o IotRole pode ser mapeado para a Partilha</span><span class="sxs-lookup"><span data-stu-id="01b15-1139">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="01b15-1140">Adição do cmdlet `Invoke-AzDataBoxEdgeDevice`</span><span class="sxs-lookup"><span data-stu-id="01b15-1140">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="01b15-1141">Invocar verificação da atualização, transferência da atualização, instalação das atualizações no dispositivo</span><span class="sxs-lookup"><span data-stu-id="01b15-1141">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="01b15-1142">Adição do cmdlet `Get-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="01b15-1142">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="01b15-1143">Obtém as informações sobre os Acionadores</span><span class="sxs-lookup"><span data-stu-id="01b15-1143">Gets the information about Triggers</span></span>
* <span data-ttu-id="01b15-1144">Adição do cmdlet `New-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="01b15-1144">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="01b15-1145">Criar novos Acionadores</span><span class="sxs-lookup"><span data-stu-id="01b15-1145">Create new Triggers</span></span>
* <span data-ttu-id="01b15-1146">Adição do cmdlet `Remove-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="01b15-1146">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="01b15-1147">Remover os Acionadores</span><span class="sxs-lookup"><span data-stu-id="01b15-1147">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="01b15-1148">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="01b15-1148">Az.DataFactory</span></span>
* <span data-ttu-id="01b15-1149">Atualização do SDK .NET do ADF para a versão 4.4.0</span><span class="sxs-lookup"><span data-stu-id="01b15-1149">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="01b15-1150">Adição do parâmetro "ExpressCustomSetup" para o cmdlet "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir configurações e componentes de terceiros sem scripts de configuração personalizados.</span><span class="sxs-lookup"><span data-stu-id="01b15-1150">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="01b15-1151">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="01b15-1151">Az.DataLakeStore</span></span>
* <span data-ttu-id="01b15-1152">Atualização da documentação de Get-AzDataLakeStoreDeletedItem e Restore-AzDataLakeStoreDeletedItem</span><span class="sxs-lookup"><span data-stu-id="01b15-1152">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="01b15-1153">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="01b15-1153">Az.EventHub</span></span>
* <span data-ttu-id="01b15-1154">Correção do problema 10301: Correção do formato de data do token de SAS</span><span class="sxs-lookup"><span data-stu-id="01b15-1154">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="01b15-1155">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="01b15-1155">Az.FrontDoor</span></span>
* <span data-ttu-id="01b15-1156">Adição do parâmetro MinimumTlsVersion a Enable-AzFrontDoorCustomDomainHttps e New-AzFrontDoorFrontendEndpointObject</span><span class="sxs-lookup"><span data-stu-id="01b15-1156">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="01b15-1157">Adição dos parâmetros HealthProbeMethod e EnabledState a New-AzFrontDoorHealthProbeSettingObject</span><span class="sxs-lookup"><span data-stu-id="01b15-1157">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="01b15-1158">Adição de um novo cmdlet para criar um objeto BackendPoolsSettings para passar para a criação/atualização do Front Door</span><span class="sxs-lookup"><span data-stu-id="01b15-1158">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="01b15-1159">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="01b15-1159">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-1160">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-1160">Az.Network</span></span>
* <span data-ttu-id="01b15-1161">Alteração dos exemplos de opções FilterData de "Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" e "Start-AzVirtualnetworkGatewayPacketCapture.md".</span><span class="sxs-lookup"><span data-stu-id="01b15-1161">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="01b15-1162">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="01b15-1162">Az.PrivateDns</span></span>
* <span data-ttu-id="01b15-1163">Atualização do SDK .NET do PrivateDns para a versão 1.0.0</span><span class="sxs-lookup"><span data-stu-id="01b15-1163">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-1164">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-1164">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-1165">Suporte do Azure Site Recovery para selecionar o tipo de disco ao ativar a proteção.</span><span class="sxs-lookup"><span data-stu-id="01b15-1165">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="01b15-1166">Correção do Azure Site Recovery para a edição de ações do plano de recuperação.</span><span class="sxs-lookup"><span data-stu-id="01b15-1166">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="01b15-1167">Suporte de Restauro de SQL do Azure Backup para aceitar BDs de filestream.</span><span class="sxs-lookup"><span data-stu-id="01b15-1167">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="01b15-1168">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="01b15-1168">Az.RedisCache</span></span>
* <span data-ttu-id="01b15-1169">Adição do parâmetro "MinimumTlsVersion" nos cmdlets "New-AzRedisCache" e "Set-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="01b15-1169">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="01b15-1170">Adição, também, de "MinimumTlsVersion" na saída do cmdlet "Get-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="01b15-1170">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="01b15-1171">Adição da validação no parâmetro "-Size" para os cmdlets "Set-AzRedisCache" e "New-AzRedisCache"</span><span class="sxs-lookup"><span data-stu-id="01b15-1171">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-1172">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-1172">Az.Resources</span></span>
- <span data-ttu-id="01b15-1173">Atualização dos cmdlets de política no sentido de utilizar a nova versão de api 2019-06-01, a qual tem a nova propriedade EnforcementMode na atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="01b15-1173">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="01b15-1174">Atualização do exemplo de ajuda da definição da política de criação</span><span class="sxs-lookup"><span data-stu-id="01b15-1174">Updated create policy definition help example</span></span>
- <span data-ttu-id="01b15-1175">Correção do erro Remove-AZADServicePrincipal -ServicePrincipalName. Apresentação de uma referência nula quando o nome do principal do serviço não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="01b15-1175">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="01b15-1176">Correção do erro New-AZADServicePrincipal. Apresentação de uma referência nula quando o inquilino não tem uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="01b15-1176">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="01b15-1177">Alteração de New-AzAdServicePrincipal para adicionar credenciais apenas a aplicações associadas.</span><span class="sxs-lookup"><span data-stu-id="01b15-1177">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-1178">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-1178">Az.Sql</span></span>
* <span data-ttu-id="01b15-1179">Adição de suporte para a base de dados ReadReplicaCount.</span><span class="sxs-lookup"><span data-stu-id="01b15-1179">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="01b15-1180">Correção de Set-AzSqlDatabase quando a redundância de zona não está definida</span><span class="sxs-lookup"><span data-stu-id="01b15-1180">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="01b15-1181">3.0.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-1181">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="01b15-1182">Geral</span><span class="sxs-lookup"><span data-stu-id="01b15-1182">General</span></span>
* <span data-ttu-id="01b15-1183">Disponibilização do Az.PrivateDns 1.0.0</span><span class="sxs-lookup"><span data-stu-id="01b15-1183">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="01b15-1184">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-1184">Az.Accounts</span></span>
* <span data-ttu-id="01b15-1185">Adição de uma mensagem de descontinuação para o alias "Resolve-Error".</span><span class="sxs-lookup"><span data-stu-id="01b15-1185">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="01b15-1186">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="01b15-1186">Az.Advisor</span></span>
* <span data-ttu-id="01b15-1187">Adição da nova categoria "Excelência Operacional" ao cmdlet Get-AzAdvisorRecommendation.</span><span class="sxs-lookup"><span data-stu-id="01b15-1187">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="01b15-1188">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="01b15-1188">Az.Batch</span></span>
* <span data-ttu-id="01b15-1189">Mudança de nome de `CoreQuota` em `BatchAccountContext` para `DedicatedCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="01b15-1189">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="01b15-1190">Existe também um novo `LowPriorityCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="01b15-1190">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="01b15-1191">Isto afeta **Get-AzBatchAccount**.</span><span class="sxs-lookup"><span data-stu-id="01b15-1191">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="01b15-1192">O parâmetro **New-AzBatchTask** `-ResourceFile` assume agora uma coleção de objetos `PSResourceFile`, os quais podem ser construídos com o novo cmdlet **New-AzBatchResourceFile**.</span><span class="sxs-lookup"><span data-stu-id="01b15-1192">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="01b15-1193">Novo cmdlet **New-AzBatchResourceFile** para ajudar a criar objetos `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="01b15-1193">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="01b15-1194">Estes podem ser fornecidos a **New-AzBatchTask** no parâmetro `-ResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="01b15-1194">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="01b15-1195">Isto suporta dois novos tipos de ficheiro de recursos para além do caminho `HttpUrl` existente:</span><span class="sxs-lookup"><span data-stu-id="01b15-1195">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="01b15-1196">Os ficheiros de recursos baseados em `AutoStorageContainerName` transferem um contentor integral de armazenamento automático para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="01b15-1196">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="01b15-1197">Os ficheiros de recursos baseados em `StorageContainerUrl` transferem o contentor especificado no URL para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="01b15-1197">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="01b15-1198">Remoção da propriedade `ApplicationPackages` de `PSApplication` devolvida por **Get-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="01b15-1198">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="01b15-1199">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com **Get-AzBatchApplicationPackage**.</span><span class="sxs-lookup"><span data-stu-id="01b15-1199">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="01b15-1200">Por exemplo: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span><span class="sxs-lookup"><span data-stu-id="01b15-1200">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="01b15-1201">Mudança de nome de `ApplicationId` para `ApplicationName` em **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication** e **Set-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="01b15-1201">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="01b15-1202">`ApplicationId` é agora um alias de `ApplicationName`.</span><span class="sxs-lookup"><span data-stu-id="01b15-1202">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="01b15-1203">Adição da nova propriedade `PSWindowsUserConfiguration` a `PSUserAccount`.</span><span class="sxs-lookup"><span data-stu-id="01b15-1203">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="01b15-1204">Mudança de nome de `Version` para `Name` em `PSApplicationPackage`.</span><span class="sxs-lookup"><span data-stu-id="01b15-1204">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="01b15-1205">Mudança de nome de `BlobSource` para `HttpUrl` em `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="01b15-1205">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="01b15-1206">Remoção da propriedade `OSDisk` de `PSVirtualMachineConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="01b15-1206">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="01b15-1207">Remoção de **Set-AzBatchPoolOSVersion**.</span><span class="sxs-lookup"><span data-stu-id="01b15-1207">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="01b15-1208">Esta operação deixou de ser suportada.</span><span class="sxs-lookup"><span data-stu-id="01b15-1208">This operation is no longer supported.</span></span>
* <span data-ttu-id="01b15-1209">Remoção de `TargetOSVersion` de `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="01b15-1209">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="01b15-1210">Mudança de nome de `CurrentOSVersion` para `OSVersion` em `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="01b15-1210">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="01b15-1211">Remoção de `DataEgressGiB` e `DataIngressGiB` de `PSPoolUsageMetrics`.</span><span class="sxs-lookup"><span data-stu-id="01b15-1211">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="01b15-1212">Remoção de **Get-AzBatchNodeAgentSku** e substituição deste por **Get-AzBatchSupportedImage**.</span><span class="sxs-lookup"><span data-stu-id="01b15-1212">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span>
  - <span data-ttu-id="01b15-1213">**Get-AzBatchSupportedImage** devolve os mesmos dados de **Get-AzBatchNodeAgentSku**, mas num formato mais acessível.</span><span class="sxs-lookup"><span data-stu-id="01b15-1213">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="01b15-1214">As novas imagens não verificadas agora também são devolvidas.</span><span class="sxs-lookup"><span data-stu-id="01b15-1214">New non-verified images are also now returned.</span></span> <span data-ttu-id="01b15-1215">Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.</span><span class="sxs-lookup"><span data-stu-id="01b15-1215">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="01b15-1216">Adição da capacidade de montagem de sistemas de ficheiros remotos em cada nó de um conjunto através do novo parâmetro `MountConfiguration` de **New-AzBatchPool**.</span><span class="sxs-lookup"><span data-stu-id="01b15-1216">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="01b15-1217">Adição do suporte a regras de segurança de rede que bloqueiam o acesso de rede a um conjunto com base na porta de origem do tráfego.</span><span class="sxs-lookup"><span data-stu-id="01b15-1217">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="01b15-1218">Isto ocorre através da propriedade `SourcePortRanges` em `PSNetworkSecurityGroupRule`.</span><span class="sxs-lookup"><span data-stu-id="01b15-1218">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="01b15-1219">Ao executar um contentor, o Batch agora suporta a execução da tarefa no diretório de trabalho do contentor ou no diretório de trabalho da tarefa do Batch.</span><span class="sxs-lookup"><span data-stu-id="01b15-1219">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="01b15-1220">Isto é controlado pela propriedade `WorkingDirectory` em `PSTaskContainerSettings`.</span><span class="sxs-lookup"><span data-stu-id="01b15-1220">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="01b15-1221">Adição da capacidade de especificar uma coleção de IPs públicos em `PSNetworkConfiguration` através da nova propriedade `PublicIPs`.</span><span class="sxs-lookup"><span data-stu-id="01b15-1221">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="01b15-1222">Isto garante que os nós no Conjunto terão um IP da lista de IPs fornecidos pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="01b15-1222">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="01b15-1223">Quando não for especificado, o valor predefinido de `WaitForSuccess` em `PSSTartTask` é agora `$True` (era `$False`).</span><span class="sxs-lookup"><span data-stu-id="01b15-1223">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="01b15-1224">Quando não for especificado, o valor predefinido de `Scope` em `PSAutoUserSpecification` é agora `Pool` (era `Task` no Windows e `Pool` no Linux).</span><span class="sxs-lookup"><span data-stu-id="01b15-1224">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="01b15-1225">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="01b15-1225">Az.Cdn</span></span>
* <span data-ttu-id="01b15-1226">Introdução de UrlRewriteAction e CacheKeyQueryStringAction em RulesEngine.</span><span class="sxs-lookup"><span data-stu-id="01b15-1226">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="01b15-1227">Correção de vários erros como a falta da Entrada "Seletor" no cmdlet New-AzDeliveryRuleCondition.</span><span class="sxs-lookup"><span data-stu-id="01b15-1227">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-1228">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-1228">Az.Compute</span></span>
* <span data-ttu-id="01b15-1229">Funcionalidade Conjunto de Encriptação de Discos</span><span class="sxs-lookup"><span data-stu-id="01b15-1229">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="01b15-1230">Novos cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="01b15-1230">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="01b15-1231">Adição do parâmetro DiskEncryptionSetId aos seguintes cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="01b15-1231">DiskEncryptionSetId parameter is added to the following cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="01b15-1232">Adição dos parâmetros DiskEncryptionSetId e EncryptionType aos seguintes cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-1232">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="01b15-1233">Adição do parâmetro PublicIPAddressVersion a New-AzVmssIPConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-1233">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="01b15-1234">Movimentação de FileUris da extensão de script personalizado da definição pública para a definição protegida</span><span class="sxs-lookup"><span data-stu-id="01b15-1234">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="01b15-1235">Adição de ScaleInPolicy aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="01b15-1235">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="01b15-1236">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="01b15-1236">Breaking changes</span></span>
    - <span data-ttu-id="01b15-1237">Utilização do parâmetro UploadSizeInBytes em vez de DiskSizeGB para New-AzDiskConfig quando CreateOption é Carregar</span><span class="sxs-lookup"><span data-stu-id="01b15-1237">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="01b15-1238">Substituição de PublishingProfile.Source.ManagedImage.Id por StorageProfile.Source.Id no objeto GalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="01b15-1238">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="01b15-1239">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="01b15-1239">Az.DataFactory</span></span>
* <span data-ttu-id="01b15-1240">Atualização da versão do SDK .Net do ADF para 4.3.0</span><span class="sxs-lookup"><span data-stu-id="01b15-1240">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="01b15-1241">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="01b15-1241">Az.DataLakeStore</span></span>
* <span data-ttu-id="01b15-1242">Atualização da versão do SDK ADLS (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) ) com as seguintes correções</span><span class="sxs-lookup"><span data-stu-id="01b15-1242">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="01b15-1243">Evita a apresentação de uma exceção ao mesmo tempo que não consegue anular a serialização do creationtime do lixo ou da entrada de diretório.</span><span class="sxs-lookup"><span data-stu-id="01b15-1243">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="01b15-1244">Expõe a definição por tempo limite do pedido em adlsclient</span><span class="sxs-lookup"><span data-stu-id="01b15-1244">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="01b15-1245">Correção da passagem do syncflag original para a recuperação de badoffset</span><span class="sxs-lookup"><span data-stu-id="01b15-1245">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="01b15-1246">Correção de EnumerateDirectory para obter o token de continuação após a verificação da resposta</span><span class="sxs-lookup"><span data-stu-id="01b15-1246">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="01b15-1247">Correção do Erro de Concatenação</span><span class="sxs-lookup"><span data-stu-id="01b15-1247">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="01b15-1248">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="01b15-1248">Az.FrontDoor</span></span>
* <span data-ttu-id="01b15-1249">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="01b15-1249">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="01b15-1250">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="01b15-1250">Az.HDInsight</span></span>
* <span data-ttu-id="01b15-1251">Correção do erro em que o cliente recebe o erro "Não é uma cadeia Base 64 válida" quando utiliza Get-AzHDInsightCluster para obter o cluster com o armazenamento ADLSGen1.</span><span class="sxs-lookup"><span data-stu-id="01b15-1251">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="01b15-1252">Adição de um parâmetro com o nome "ApplicationId" a três cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig e New-AzHDInsightCluster para que o cliente consiga fornecer o ID da aplicação do principal de serviço que permite aceder ao Azure Data Lake.</span><span class="sxs-lookup"><span data-stu-id="01b15-1252">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="01b15-1253">Alteração de Microsoft.Azure.Management.HDInsight da versão 2.1.0 para a 5.1.0</span><span class="sxs-lookup"><span data-stu-id="01b15-1253">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="01b15-1254">Remoção de cinco cmdlets:</span><span class="sxs-lookup"><span data-stu-id="01b15-1254">Removed five cmdlets:</span></span>
    - <span data-ttu-id="01b15-1255">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="01b15-1255">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="01b15-1256">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="01b15-1256">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="01b15-1257">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="01b15-1257">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="01b15-1258">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="01b15-1258">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="01b15-1259">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="01b15-1259">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="01b15-1260">Adição de três cmdlets:</span><span class="sxs-lookup"><span data-stu-id="01b15-1260">Added three cmdlets:</span></span>
    - <span data-ttu-id="01b15-1261">Get-AzHDInsightMonitoring para substituir Get-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="01b15-1261">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="01b15-1262">Enable-AzHDInsightMonitoring para substituir Enable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="01b15-1262">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="01b15-1263">Disable-AzHDInsightMonitoring para substituir Disable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="01b15-1263">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="01b15-1264">Correção do cmdlet Get-AzHDInsightProperties para suportar a obtenção de informações sobre capacidades de uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="01b15-1264">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="01b15-1265">Remoção de conjuntos de parâmetros("Spark1", "Spark2") de Add-AzHDInsightConfigValue.</span><span class="sxs-lookup"><span data-stu-id="01b15-1265">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="01b15-1266">Adição de exemplos aos documentos de ajuda do cmdlet Add-AzHDInsightSecurityProfile.</span><span class="sxs-lookup"><span data-stu-id="01b15-1266">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="01b15-1267">Alteração do tipo de saída dos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="01b15-1267">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="01b15-1268">Alteração do tipo de saída de Get-AzHDInsightProperties de CapabilitiesResponse para AzureHDInsightCapabilities.</span><span class="sxs-lookup"><span data-stu-id="01b15-1268">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="01b15-1269">Alteração do tipo de saída de Remove-AzHDInsightCluster de ClusterGetResponse para booleano.</span><span class="sxs-lookup"><span data-stu-id="01b15-1269">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="01b15-1270">Alteração do tipo de saída de Set-AzHDInsightGatewaySettings de HttpConnectivitySettings para GatewaySettings.</span><span class="sxs-lookup"><span data-stu-id="01b15-1270">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="01b15-1271">Adição de alguns casos de teste de cenários.</span><span class="sxs-lookup"><span data-stu-id="01b15-1271">Added some scenario test cases.</span></span>
* <span data-ttu-id="01b15-1272">Remoção de alguns alias: "Add-AzHDInsightConfigValues", "Get-AzHDInsightProperties".</span><span class="sxs-lookup"><span data-stu-id="01b15-1272">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="01b15-1273">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="01b15-1273">Az.IotHub</span></span>
* <span data-ttu-id="01b15-1274">Alterações interruptivas:</span><span class="sxs-lookup"><span data-stu-id="01b15-1274">Breaking changes:</span></span>
    - <span data-ttu-id="01b15-1275">O cmdlet "Add-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="01b15-1275">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="01b15-1276">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Add-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="01b15-1276">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="01b15-1277">O cmdlet "Get-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="01b15-1277">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="01b15-1278">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Get-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="01b15-1278">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="01b15-1279">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="01b15-1279">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="01b15-1280">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="01b15-1280">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="01b15-1281">O cmdlet "New-AzIotHubExportDevice" deixou de suportar o alias "New-AzIotHubExportDevices".</span><span class="sxs-lookup"><span data-stu-id="01b15-1281">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="01b15-1282">O cmdlet "New-AzIotHubImportDevice" deixou de suportar o alias "New-AzIotHubImportDevices".</span><span class="sxs-lookup"><span data-stu-id="01b15-1282">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="01b15-1283">O cmdlet "Remove-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="01b15-1283">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="01b15-1284">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Remove-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="01b15-1284">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="01b15-1285">O cmdlet "Set-AzIotHub" deixou de suportar o parâmetro "OperationsMonitoringProperties" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="01b15-1285">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="01b15-1286">O conjunto de parâmetros "UpdateOperationsMonitoringProperties" do cmdlet "Set-AzIotHub" foi removido.</span><span class="sxs-lookup"><span data-stu-id="01b15-1286">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-1287">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-1287">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-1288">Suporte do Azure Site Recovery para configurar recursos de rede como NSG, IP público e balanceadores de carga internos do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-1288">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="01b15-1289">Suporte do Azure Site Recovery para escrever para um disco gerido do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-1289">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="01b15-1290">Suporte do Azure Site Recovery para redução de NIC do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-1290">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="01b15-1291">Suporte do Azure Site Recovery para aceleração de rede do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-1291">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="01b15-1292">Suporte do Azure Site Recovery para a atualização automática do agente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-1292">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="01b15-1293">Suporte do Azure Site Recovery para SSD Standard do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-1293">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="01b15-1294">Suporte do Azure Site Recovery para a codificação em dois passos do Azure Disk Encryption do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-1294">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="01b15-1295">Suporte do Azure Site Recovery para a proteção de um disco adicionado recentemente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-1295">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="01b15-1296">Adição da funcionalidade SoftDelete para VM e de testes para softdelete</span><span class="sxs-lookup"><span data-stu-id="01b15-1296">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-1297">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-1297">Az.Resources</span></span>
* <span data-ttu-id="01b15-1298">Atualização da assemblagem de dependências Microsoft.Extensions.Caching.Memory da versão 1.1.1 para a 2.2</span><span class="sxs-lookup"><span data-stu-id="01b15-1298">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-1299">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-1299">Az.Network</span></span>
* <span data-ttu-id="01b15-1300">Alteração de todos os cmdlets para PrivateEndpointConnection para suportar o fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="01b15-1300">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="01b15-1301">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="01b15-1301">Updated cmdlet:</span></span>
        - <span data-ttu-id="01b15-1302">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-1302">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="01b15-1303">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-1303">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="01b15-1304">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-1304">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="01b15-1305">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-1305">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="01b15-1306">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-1306">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="01b15-1307">Adição de novo cmdlet para PrivateLinkResource também com suporte de fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="01b15-1307">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="01b15-1308">Novo cmdlet:</span><span class="sxs-lookup"><span data-stu-id="01b15-1308">New cmdlet:</span></span>
        - <span data-ttu-id="01b15-1309">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="01b15-1309">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="01b15-1310">Adição de novos campos e parâmetro para a funcionalidade Protocolo de Proxy V2.</span><span class="sxs-lookup"><span data-stu-id="01b15-1310">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="01b15-1311">Adição da propriedade EnableProxyProtocol em PrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="01b15-1311">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="01b15-1312">Adição da propriedade LinkIdentifier em PrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-1312">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="01b15-1313">Atualização de New-AzPrivateLinkService para adicionar um novo parâmetro adicional EnableProxyProtocol.</span><span class="sxs-lookup"><span data-stu-id="01b15-1313">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="01b15-1314">Correção da descrição incorreta do parâmetro na documentação de referência "New-AzApplicationGatewaySku"</span><span class="sxs-lookup"><span data-stu-id="01b15-1314">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="01b15-1315">Novos cmdlets para suportar a política de firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="01b15-1315">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="01b15-1316">Adição de suporte para o recurso subordinado RouteTables de VirtualHub</span><span class="sxs-lookup"><span data-stu-id="01b15-1316">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="01b15-1317">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="01b15-1317">New cmdlets added:</span></span>
        - <span data-ttu-id="01b15-1318">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="01b15-1318">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="01b15-1319">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="01b15-1319">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="01b15-1320">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="01b15-1320">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="01b15-1321">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="01b15-1321">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="01b15-1322">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="01b15-1322">Set-AzVirtualHub</span></span>
* <span data-ttu-id="01b15-1323">Adição de suporte para o SKU de novas propriedades de VirtualHub e VirtualWANType de VirtualWan</span><span class="sxs-lookup"><span data-stu-id="01b15-1323">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="01b15-1324">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="01b15-1324">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="01b15-1325">New-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="01b15-1325">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="01b15-1326">Update-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="01b15-1326">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="01b15-1327">New-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="01b15-1327">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="01b15-1328">Update-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="01b15-1328">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="01b15-1329">Adição de suporte para a propriedade EnableInternetSecurity para HubVnetConnection, VpnConnection e ExpressRouteConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-1329">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="01b15-1330">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="01b15-1330">New cmdlets added:</span></span>
        - <span data-ttu-id="01b15-1331">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-1331">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="01b15-1332">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="01b15-1332">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="01b15-1333">New-AzureRmVirtualHubVnetConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="01b15-1333">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="01b15-1334">New-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="01b15-1334">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="01b15-1335">Update-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="01b15-1335">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="01b15-1336">New-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="01b15-1336">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="01b15-1337">Set-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="01b15-1337">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="01b15-1338">Adição de suporte para Configurar a Política WebApplicationFirewall de Nível Superior</span><span class="sxs-lookup"><span data-stu-id="01b15-1338">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="01b15-1339">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="01b15-1339">New cmdlets added:</span></span>
        - <span data-ttu-id="01b15-1340">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="01b15-1340">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="01b15-1341">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="01b15-1341">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="01b15-1342">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="01b15-1342">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="01b15-1343">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="01b15-1343">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="01b15-1344">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="01b15-1344">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="01b15-1345">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="01b15-1345">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="01b15-1346">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="01b15-1346">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="01b15-1347">New-AzApplicationGatewayFirewallPolicy : adição do parâmetro PolicySetting, ManagedRule</span><span class="sxs-lookup"><span data-stu-id="01b15-1347">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="01b15-1348">Adição de suporte para o operador GeoMatch em CustomRule</span><span class="sxs-lookup"><span data-stu-id="01b15-1348">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="01b15-1349">Adição de GeoMatch ao operador em FirewallCondition</span><span class="sxs-lookup"><span data-stu-id="01b15-1349">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="01b15-1350">Adição de suporte para a Política de firewall perListener e perSite</span><span class="sxs-lookup"><span data-stu-id="01b15-1350">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="01b15-1351">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="01b15-1351">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="01b15-1352">New-AzApplicationGatewayHttpListener : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="01b15-1352">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="01b15-1353">New-AzApplicationGatewayPathRuleConfig : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="01b15-1353">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="01b15-1354">Correção da sub-rede necessária com o nome AzureBastionSubnet em "PSBastion" pode não ser sensível às maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="01b15-1354">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="01b15-1355">Suporte para FQDNs de Destino nas Regras de Rede e para FQDN Traduzido em Regras NAT para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="01b15-1355">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="01b15-1356">Adição de suporte para o recurso de nível superior RouteTables de IpGroup</span><span class="sxs-lookup"><span data-stu-id="01b15-1356">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="01b15-1357">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="01b15-1357">New cmdlets added:</span></span>
        - <span data-ttu-id="01b15-1358">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="01b15-1358">New-AzIpGroup</span></span>
        - <span data-ttu-id="01b15-1359">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="01b15-1359">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="01b15-1360">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="01b15-1360">Get-AzIpGroup</span></span>
        - <span data-ttu-id="01b15-1361">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="01b15-1361">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="01b15-1362">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="01b15-1362">Az.ServiceFabric</span></span>
* <span data-ttu-id="01b15-1363">Remoção do cmdlet Add-AzServiceFabricApplicationCertificate uma vez que este cenário é abrangido por Add-AzVmssSecret.</span><span class="sxs-lookup"><span data-stu-id="01b15-1363">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-1364">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-1364">Az.Sql</span></span>
* <span data-ttu-id="01b15-1365">Adição de suporte para o restauro de bases de dados removidas em Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="01b15-1365">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="01b15-1366">Descontinuação dos cmdlets de auditoria antigos do código.</span><span class="sxs-lookup"><span data-stu-id="01b15-1366">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="01b15-1367">Remoção de aliases descontinuados:</span><span class="sxs-lookup"><span data-stu-id="01b15-1367">Removed deprecated aliases:</span></span>
* <span data-ttu-id="01b15-1368">Get-AzSqlDatabaseIndexRecommendations (utilize antes Get-AzSqlDatabaseIndexRecommendation)</span><span class="sxs-lookup"><span data-stu-id="01b15-1368">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="01b15-1369">Get-AzSqlDatabaseRestorePoints (utilize antes Get-AzSqlDatabaseRestorePoint)</span><span class="sxs-lookup"><span data-stu-id="01b15-1369">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="01b15-1370">Remoção do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="01b15-1370">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="01b15-1371">Remoção dos aliases dos cmdlets descontinuados das Definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="01b15-1371">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="01b15-1372">Descontinuação dos cmdlets das Definições de Deteção Avançada de Ameaças</span><span class="sxs-lookup"><span data-stu-id="01b15-1372">Deprecate Advanced Threat Detection Settings cmdlets</span></span>
* <span data-ttu-id="01b15-1373">Adição de cmdlets para Desativar e Ativar as recomendações de sensibilidade nas colunas de uma base de dados.</span><span class="sxs-lookup"><span data-stu-id="01b15-1373">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-1374">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-1374">Az.Storage</span></span>
* <span data-ttu-id="01b15-1375">Suporte à ativação da partilha de Ficheiros de Grandes Dimensões ao criar ou atualizar uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="01b15-1375">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="01b15-1376">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="01b15-1376">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="01b15-1377">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="01b15-1377">Set-AzStorageAccount</span></span>
* <span data-ttu-id="01b15-1378">Ao fechar/obter o Identificador de ficheiro, ignorar a verificação do caminho de entrada corresponde a Diretório de ficheiros ou Ficheiro, de forma a evitar a falha com o objeto no estado DeletePending</span><span class="sxs-lookup"><span data-stu-id="01b15-1378">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="01b15-1379">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="01b15-1379">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="01b15-1380">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="01b15-1380">Close-AzStorageFileHandle</span></span>

## <a name="280---october-2019"></a><span data-ttu-id="01b15-1381">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-1381">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="01b15-1382">Geral</span><span class="sxs-lookup"><span data-stu-id="01b15-1382">General</span></span>
* <span data-ttu-id="01b15-1383">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="01b15-1383">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="01b15-1384">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-1384">Az.Accounts</span></span>
* <span data-ttu-id="01b15-1385">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="01b15-1385">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="01b15-1386">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="01b15-1386">Az.ApiManagement</span></span>
* <span data-ttu-id="01b15-1387">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="01b15-1387">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="01b15-1388">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="01b15-1388">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="01b15-1389">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="01b15-1389">Az.Automation</span></span>
* <span data-ttu-id="01b15-1390">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="01b15-1390">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="01b15-1391">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="01b15-1391">Az.Batch</span></span>
* <span data-ttu-id="01b15-1392">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="01b15-1392">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-1393">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-1393">Az.Compute</span></span>
* <span data-ttu-id="01b15-1394">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="01b15-1394">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="01b15-1395">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="01b15-1395">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="01b15-1396">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="01b15-1396">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span>
* <span data-ttu-id="01b15-1397">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="01b15-1397">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="01b15-1398">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="01b15-1398">Az.DataFactory</span></span>
* <span data-ttu-id="01b15-1399">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="01b15-1399">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="01b15-1400">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="01b15-1400">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="01b15-1401">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="01b15-1401">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="01b15-1402">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="01b15-1402">Az.DataLakeStore</span></span>
* <span data-ttu-id="01b15-1403">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="01b15-1403">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="01b15-1404">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="01b15-1404">Az.HealthcareApis</span></span>
* <span data-ttu-id="01b15-1405">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="01b15-1405">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="01b15-1406">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="01b15-1406">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="01b15-1407">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="01b15-1407">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="01b15-1408">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="01b15-1408">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="01b15-1409">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="01b15-1409">Az.IotHub</span></span>
* <span data-ttu-id="01b15-1410">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="01b15-1410">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="01b15-1411">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="01b15-1411">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="01b15-1412">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="01b15-1412">Az.Monitor</span></span>
* <span data-ttu-id="01b15-1413">Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="01b15-1413">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="01b15-1414">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="01b15-1414">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="01b15-1415">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="01b15-1415">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="01b15-1416">Os Webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="01b15-1416">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-1417">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-1417">Az.Network</span></span>
* <span data-ttu-id="01b15-1418">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="01b15-1418">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="01b15-1419">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="01b15-1419">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="01b15-1420">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="01b15-1420">New cmdlets added:</span></span>
        - <span data-ttu-id="01b15-1421">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="01b15-1421">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="01b15-1422">Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-1422">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="01b15-1423">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="01b15-1423">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="01b15-1424">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="01b15-1424">Updated cmdlets:</span></span>
        - <span data-ttu-id="01b15-1425">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-1425">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="01b15-1426">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-1426">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="01b15-1427">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-1427">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="01b15-1428">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="01b15-1428">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="01b15-1429">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="01b15-1429">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="01b15-1430">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="01b15-1430">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="01b15-1431">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="01b15-1431">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="01b15-1432">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="01b15-1432">Az.RedisCache</span></span>
* <span data-ttu-id="01b15-1433">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="01b15-1433">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-1434">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-1434">Az.Sql</span></span>
* <span data-ttu-id="01b15-1435">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="01b15-1435">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-1436">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-1436">Az.Storage</span></span>
* <span data-ttu-id="01b15-1437">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="01b15-1437">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="01b15-1438">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="01b15-1438">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="01b15-1439">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="01b15-1439">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="01b15-1440">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="01b15-1440">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="01b15-1441">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="01b15-1441">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="01b15-1442">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="01b15-1442">Az.StorageSync</span></span>
* <span data-ttu-id="01b15-1443">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="01b15-1443">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="01b15-1444">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-1444">Az.Websites</span></span>
* <span data-ttu-id="01b15-1445">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="01b15-1445">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="01b15-1446">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-1446">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="01b15-1447">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="01b15-1447">Az.ApiManagement</span></span>
* <span data-ttu-id="01b15-1448">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="01b15-1448">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="01b15-1449">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="01b15-1449">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="01b15-1450">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="01b15-1450">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="01b15-1451">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="01b15-1451">Az.Automation</span></span>
* <span data-ttu-id="01b15-1452">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="01b15-1452">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="01b15-1453">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="01b15-1453">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="01b15-1454">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="01b15-1454">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-1455">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-1455">Az.Compute</span></span>
* <span data-ttu-id="01b15-1456">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-1456">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="01b15-1457">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-1457">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="01b15-1458">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="01b15-1458">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="01b15-1459">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="01b15-1459">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="01b15-1460">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="01b15-1460">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="01b15-1461">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="01b15-1461">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="01b15-1462">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="01b15-1462">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="01b15-1463">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="01b15-1463">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="01b15-1464">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="01b15-1464">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="01b15-1465">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="01b15-1465">Az.DataFactory</span></span>
* <span data-ttu-id="01b15-1466">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="01b15-1466">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="01b15-1467">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="01b15-1467">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="01b15-1468">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="01b15-1468">Az.HDInsight</span></span>
* <span data-ttu-id="01b15-1469">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="01b15-1469">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="01b15-1470">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="01b15-1470">Az.IotHub</span></span>
* <span data-ttu-id="01b15-1471">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="01b15-1471">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="01b15-1472">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="01b15-1472">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="01b15-1473">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="01b15-1473">New cmdlets are:</span></span>
    - <span data-ttu-id="01b15-1474">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="01b15-1474">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="01b15-1475">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="01b15-1475">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="01b15-1476">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="01b15-1476">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="01b15-1477">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="01b15-1477">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="01b15-1478">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="01b15-1478">Az.Monitor</span></span>
* <span data-ttu-id="01b15-1479">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="01b15-1479">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="01b15-1480">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="01b15-1480">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="01b15-1481">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="01b15-1481">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="01b15-1482">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="01b15-1482">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="01b15-1483">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="01b15-1483">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="01b15-1484">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="01b15-1484">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="01b15-1485">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="01b15-1485">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="01b15-1486">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="01b15-1486">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="01b15-1487">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="01b15-1487">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="01b15-1488">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="01b15-1488">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="01b15-1489">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="01b15-1489">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="01b15-1490">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="01b15-1490">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="01b15-1491">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="01b15-1491">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="01b15-1492">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="01b15-1492">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="01b15-1493">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="01b15-1493">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="01b15-1494">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="01b15-1494">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="01b15-1495">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="01b15-1495">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="01b15-1496">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="01b15-1496">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="01b15-1497">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="01b15-1497">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="01b15-1498">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="01b15-1498">Overall improved help files</span></span>
* <span data-ttu-id="01b15-1499">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="01b15-1499">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-1500">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-1500">Az.Network</span></span>
* <span data-ttu-id="01b15-1501">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="01b15-1501">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span>
* <span data-ttu-id="01b15-1502">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="01b15-1502">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="01b15-1503">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="01b15-1503">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="01b15-1504">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="01b15-1504">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="01b15-1505">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="01b15-1505">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="01b15-1506">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="01b15-1506">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="01b15-1507">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="01b15-1507">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="01b15-1508">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="01b15-1508">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="01b15-1509">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="01b15-1509">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="01b15-1510">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="01b15-1510">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="01b15-1511">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="01b15-1511">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="01b15-1512">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="01b15-1512">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="01b15-1513">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="01b15-1513">New cmdlets</span></span>
        - <span data-ttu-id="01b15-1514">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="01b15-1514">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="01b15-1515">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-1515">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="01b15-1516">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="01b15-1516">Updated cmdlet:</span></span>
        - <span data-ttu-id="01b15-1517">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="01b15-1517">New-VpnSite</span></span>
        - <span data-ttu-id="01b15-1518">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="01b15-1518">Update-VpnSite</span></span>
        - <span data-ttu-id="01b15-1519">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-1519">New-VpnConnection</span></span>
        - <span data-ttu-id="01b15-1520">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-1520">Update-VpnConnection</span></span>
* <span data-ttu-id="01b15-1521">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="01b15-1521">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-1522">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-1522">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-1523">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="01b15-1523">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="01b15-1524">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="01b15-1524">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-1525">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-1525">Az.Resources</span></span>
* <span data-ttu-id="01b15-1526">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="01b15-1526">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="01b15-1527">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="01b15-1527">Az.ServiceFabric</span></span>
* <span data-ttu-id="01b15-1528">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="01b15-1528">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="01b15-1529">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="01b15-1529">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="01b15-1530">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="01b15-1530">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="01b15-1531">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="01b15-1531">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="01b15-1532">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="01b15-1532">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="01b15-1533">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="01b15-1533">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="01b15-1534">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="01b15-1534">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="01b15-1535">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="01b15-1535">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="01b15-1536">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="01b15-1536">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="01b15-1537">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="01b15-1537">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="01b15-1538">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="01b15-1538">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="01b15-1539">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="01b15-1539">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="01b15-1540">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="01b15-1540">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="01b15-1541">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="01b15-1541">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="01b15-1542">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="01b15-1542">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="01b15-1543">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="01b15-1543">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="01b15-1544">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="01b15-1544">Az.SignalR</span></span>
* <span data-ttu-id="01b15-1545">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="01b15-1545">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-1546">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-1546">Az.Sql</span></span>
* <span data-ttu-id="01b15-1547">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="01b15-1547">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="01b15-1548">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="01b15-1548">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="01b15-1549">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="01b15-1549">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="01b15-1550">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="01b15-1550">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="01b15-1551">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="01b15-1551">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-1552">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-1552">Az.Storage</span></span>
* <span data-ttu-id="01b15-1553">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="01b15-1553">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="01b15-1554">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="01b15-1554">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="01b15-1555">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="01b15-1555">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="01b15-1556">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="01b15-1556">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="01b15-1557">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="01b15-1557">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="01b15-1558">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="01b15-1558">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="01b15-1559">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="01b15-1559">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="01b15-1560">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="01b15-1560">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="01b15-1561">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="01b15-1561">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="01b15-1562">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="01b15-1562">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="01b15-1563">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="01b15-1563">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="01b15-1564">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-1564">Az.Websites</span></span>
* <span data-ttu-id="01b15-1565">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="01b15-1565">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="01b15-1566">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="01b15-1566">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="01b15-1567">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="01b15-1567">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="01b15-1568">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-1568">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="01b15-1569">Geral</span><span class="sxs-lookup"><span data-stu-id="01b15-1569">General</span></span>
* <span data-ttu-id="01b15-1570">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="01b15-1570">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="01b15-1571">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-1571">Az.Accounts</span></span>
* <span data-ttu-id="01b15-1572">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="01b15-1572">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="01b15-1573">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="01b15-1573">Az.Aks</span></span>
* <span data-ttu-id="01b15-1574">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="01b15-1574">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="01b15-1575">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="01b15-1575">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="01b15-1576">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="01b15-1576">Az.ApiManagement</span></span>
* <span data-ttu-id="01b15-1577">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="01b15-1577">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="01b15-1578">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="01b15-1578">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="01b15-1579">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="01b15-1579">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="01b15-1580">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="01b15-1580">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="01b15-1581">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="01b15-1581">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="01b15-1582">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="01b15-1582">Az.Batch</span></span>
* <span data-ttu-id="01b15-1583">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="01b15-1583">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="01b15-1584">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="01b15-1584">Az.Cdn</span></span>
* <span data-ttu-id="01b15-1585">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="01b15-1585">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-1586">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-1586">Az.Compute</span></span>
* <span data-ttu-id="01b15-1587">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-1587">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="01b15-1588">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="01b15-1588">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="01b15-1589">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="01b15-1589">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="01b15-1590">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="01b15-1590">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="01b15-1591">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="01b15-1591">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="01b15-1592">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="01b15-1592">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="01b15-1593">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="01b15-1593">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="01b15-1594">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="01b15-1594">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="01b15-1595">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="01b15-1595">Az.DataFactory</span></span>
* <span data-ttu-id="01b15-1596">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="01b15-1596">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="01b15-1597">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="01b15-1597">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="01b15-1598">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="01b15-1598">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="01b15-1599">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="01b15-1599">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="01b15-1600">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="01b15-1600">Az.DataLakeStore</span></span>
* <span data-ttu-id="01b15-1601">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="01b15-1601">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="01b15-1602">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="01b15-1602">Az.EventHub</span></span>
* <span data-ttu-id="01b15-1603">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="01b15-1603">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="01b15-1604">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="01b15-1604">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="01b15-1605">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="01b15-1605">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="01b15-1606">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="01b15-1606">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="01b15-1607">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="01b15-1607">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="01b15-1608">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="01b15-1608">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="01b15-1609">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="01b15-1609">Az.Monitor</span></span>
* <span data-ttu-id="01b15-1610">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="01b15-1610">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-1611">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-1611">Az.Network</span></span>
* <span data-ttu-id="01b15-1612">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="01b15-1612">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="01b15-1613">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="01b15-1613">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="01b15-1614">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="01b15-1614">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="01b15-1615">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="01b15-1615">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="01b15-1616">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="01b15-1616">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span>
* <span data-ttu-id="01b15-1617">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="01b15-1617">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="01b15-1618">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="01b15-1618">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="01b15-1619">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-1619">Az.OperationalInsights</span></span>
* <span data-ttu-id="01b15-1620">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="01b15-1620">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="01b15-1621">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="01b15-1621">Added example</span></span>
    - <span data-ttu-id="01b15-1622">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="01b15-1622">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="01b15-1623">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="01b15-1623">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="01b15-1624">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="01b15-1624">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-1625">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-1625">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-1626">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="01b15-1626">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-1627">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-1627">Az.Resources</span></span>
* <span data-ttu-id="01b15-1628">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="01b15-1628">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="01b15-1629">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="01b15-1629">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="01b15-1630">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="01b15-1630">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="01b15-1631">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="01b15-1631">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="01b15-1632">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="01b15-1632">Az.ServiceBus</span></span>
* <span data-ttu-id="01b15-1633">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="01b15-1633">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="01b15-1634">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="01b15-1634">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="01b15-1635">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="01b15-1635">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="01b15-1636">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="01b15-1636">Az.ServiceFabric</span></span>
* <span data-ttu-id="01b15-1637">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="01b15-1637">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="01b15-1638">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="01b15-1638">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="01b15-1639">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="01b15-1639">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="01b15-1640">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="01b15-1640">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="01b15-1641">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="01b15-1641">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="01b15-1642">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="01b15-1642">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-1643">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-1643">Az.Sql</span></span>
* <span data-ttu-id="01b15-1644">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="01b15-1644">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-1645">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-1645">Az.Storage</span></span>
* <span data-ttu-id="01b15-1646">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="01b15-1646">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="01b15-1647">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="01b15-1647">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="01b15-1648">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="01b15-1648">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="01b15-1649">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="01b15-1649">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="01b15-1650">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="01b15-1650">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="01b15-1651">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="01b15-1651">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="01b15-1652">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-1652">Az.Websites</span></span>
* <span data-ttu-id="01b15-1653">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="01b15-1653">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="01b15-1654">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-1654">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="01b15-1655">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-1655">Az.Accounts</span></span>
* <span data-ttu-id="01b15-1656">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="01b15-1656">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="01b15-1657">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-1657">Az.ApplicationInsights</span></span>
* <span data-ttu-id="01b15-1658">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="01b15-1658">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span>

#### <a name="azautomation"></a><span data-ttu-id="01b15-1659">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="01b15-1659">Az.Automation</span></span>
* <span data-ttu-id="01b15-1660">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="01b15-1660">Fix typo in resource string</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="01b15-1661">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="01b15-1661">Az.CognitiveServices</span></span>
* <span data-ttu-id="01b15-1662">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="01b15-1662">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-1663">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-1663">Az.Compute</span></span>
* <span data-ttu-id="01b15-1664">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="01b15-1664">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="01b15-1665">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="01b15-1665">Az.ContainerRegistry</span></span>
* <span data-ttu-id="01b15-1666">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="01b15-1666">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="01b15-1667">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="01b15-1667">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="01b15-1668">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="01b15-1668">Az.DataFactory</span></span>
* <span data-ttu-id="01b15-1669">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="01b15-1669">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="01b15-1670">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="01b15-1670">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="01b15-1671">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="01b15-1671">Az.EventHub</span></span>
* <span data-ttu-id="01b15-1672">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="01b15-1672">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="01b15-1673">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="01b15-1673">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="01b15-1674">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b15-1674">Az.KeyVault</span></span>
* <span data-ttu-id="01b15-1675">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="01b15-1675">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="01b15-1676">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="01b15-1676">Az.LogicApp</span></span>
* <span data-ttu-id="01b15-1677">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="01b15-1677">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="01b15-1678">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="01b15-1678">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="01b15-1679">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="01b15-1679">Az.ManagedServices</span></span>
* <span data-ttu-id="01b15-1680">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="01b15-1680">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-1681">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-1681">Az.Network</span></span>
* <span data-ttu-id="01b15-1682">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="01b15-1682">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="01b15-1683">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="01b15-1683">New cmdlets</span></span>
        - <span data-ttu-id="01b15-1684">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="01b15-1684">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="01b15-1685">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="01b15-1685">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="01b15-1686">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-1686">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="01b15-1687">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-1687">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="01b15-1688">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-1688">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="01b15-1689">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-1689">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="01b15-1690">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="01b15-1690">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="01b15-1691">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="01b15-1691">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="01b15-1692">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="01b15-1692">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="01b15-1693">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-1693">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="01b15-1694">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="01b15-1694">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="01b15-1695">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="01b15-1695">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="01b15-1696">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="01b15-1696">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="01b15-1697">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="01b15-1697">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="01b15-1698">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="01b15-1698">Updated cmdlets</span></span>
        - <span data-ttu-id="01b15-1699">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-1699">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="01b15-1700">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-1700">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="01b15-1701">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-1701">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="01b15-1702">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-1702">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="01b15-1703">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="01b15-1703">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="01b15-1704">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="01b15-1704">Updated cmdlet:</span></span>
        - <span data-ttu-id="01b15-1705">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-1705">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="01b15-1706">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-1706">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="01b15-1707">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-1707">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="01b15-1708">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="01b15-1708">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="01b15-1709">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="01b15-1709">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="01b15-1710">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="01b15-1710">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="01b15-1711">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-1711">Az.OperationalInsights</span></span>
* <span data-ttu-id="01b15-1712">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="01b15-1712">Updated default version for saved searches to be 1.</span></span>
* <span data-ttu-id="01b15-1713">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="01b15-1713">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-1714">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-1714">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-1715">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="01b15-1715">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="01b15-1716">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="01b15-1716">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="01b15-1717">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="01b15-1717">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="01b15-1718">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="01b15-1718">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="01b15-1719">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="01b15-1719">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="01b15-1720">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="01b15-1720">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="01b15-1721">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="01b15-1721">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="01b15-1722">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="01b15-1722">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="01b15-1723">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="01b15-1723">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="01b15-1724">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="01b15-1724">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-1725">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-1725">Az.Resources</span></span>
- <span data-ttu-id="01b15-1726">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="01b15-1726">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="01b15-1727">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="01b15-1727">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="01b15-1728">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="01b15-1728">Az.ServiceBus</span></span>
* <span data-ttu-id="01b15-1729">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="01b15-1729">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="01b15-1730">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="01b15-1730">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-1731">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-1731">Az.Sql</span></span>
* <span data-ttu-id="01b15-1732">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="01b15-1732">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="01b15-1733">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="01b15-1733">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="01b15-1734">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="01b15-1734">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-1735">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-1735">Az.Storage</span></span>
* <span data-ttu-id="01b15-1736">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="01b15-1736">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="01b15-1737">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="01b15-1737">Az.StorageSync</span></span>
* <span data-ttu-id="01b15-1738">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="01b15-1738">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="01b15-1739">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="01b15-1739">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="01b15-1740">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-1740">Az.Websites</span></span>
* <span data-ttu-id="01b15-1741">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="01b15-1741">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="01b15-1742">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="01b15-1742">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="01b15-1743">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="01b15-1743">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="01b15-1744">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-1744">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="01b15-1745">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-1745">Az.Accounts</span></span>
* <span data-ttu-id="01b15-1746">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="01b15-1746">Add support for profile cmdlets</span></span>
* <span data-ttu-id="01b15-1747">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="01b15-1747">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="01b15-1748">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="01b15-1748">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="01b15-1749">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="01b15-1749">Az.Advisor</span></span>
* <span data-ttu-id="01b15-1750">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="01b15-1750">GA release of Az.Advisor</span></span>
* <span data-ttu-id="01b15-1751">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="01b15-1751">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="01b15-1752">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="01b15-1752">Az.ApiManagement</span></span>
* <span data-ttu-id="01b15-1753">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="01b15-1753">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="01b15-1754">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="01b15-1754">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="01b15-1755">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="01b15-1755">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="01b15-1756">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="01b15-1756">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="01b15-1757">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="01b15-1757">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="01b15-1758">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="01b15-1758">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="01b15-1759">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="01b15-1759">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="01b15-1760">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="01b15-1760">Az.Automation</span></span>
* <span data-ttu-id="01b15-1761">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="01b15-1761">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-1762">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-1762">Az.Compute</span></span>
* <span data-ttu-id="01b15-1763">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-1763">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="01b15-1764">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="01b15-1764">Az.DataFactory</span></span>
* <span data-ttu-id="01b15-1765">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="01b15-1765">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="01b15-1766">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="01b15-1766">Az.EventGrid</span></span>
* <span data-ttu-id="01b15-1767">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="01b15-1767">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="01b15-1768">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="01b15-1768">Az.IotHub</span></span>
* <span data-ttu-id="01b15-1769">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="01b15-1769">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-1770">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-1770">Az.Network</span></span>
* <span data-ttu-id="01b15-1771">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="01b15-1771">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="01b15-1772">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="01b15-1772">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="01b15-1773">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-1773">Az.PolicyInsights</span></span>
* <span data-ttu-id="01b15-1774">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="01b15-1774">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="01b15-1775">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="01b15-1775">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="01b15-1776">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-1776">Az.OperationalInsights</span></span>
* <span data-ttu-id="01b15-1777">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="01b15-1777">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-1778">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-1778">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-1779">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="01b15-1779">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-1780">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-1780">Az.Resources</span></span>
    - <span data-ttu-id="01b15-1781">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="01b15-1781">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="01b15-1782">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="01b15-1782">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="01b15-1783">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="01b15-1783">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="01b15-1784">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="01b15-1784">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="01b15-1785">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="01b15-1785">Az.ServiceBus</span></span>
* <span data-ttu-id="01b15-1786">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="01b15-1786">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-1787">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-1787">Az.Sql</span></span>
* <span data-ttu-id="01b15-1788">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="01b15-1788">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="01b15-1789">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="01b15-1789">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="01b15-1790">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="01b15-1790">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="01b15-1791">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="01b15-1791">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="01b15-1792">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="01b15-1792">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="01b15-1793">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="01b15-1793">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="01b15-1794">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="01b15-1794">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="01b15-1795">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="01b15-1795">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="01b15-1796">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="01b15-1796">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-1797">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-1797">Az.Storage</span></span>
* <span data-ttu-id="01b15-1798">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="01b15-1798">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="01b15-1799">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="01b15-1799">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="01b15-1800">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="01b15-1800">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="01b15-1801">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="01b15-1801">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="01b15-1802">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="01b15-1802">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="01b15-1803">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="01b15-1803">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="01b15-1804">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="01b15-1804">Set-AzStorageAccount</span></span>
* <span data-ttu-id="01b15-1805">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="01b15-1805">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="01b15-1806">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="01b15-1806">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="01b15-1807">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="01b15-1807">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="01b15-1808">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="01b15-1808">Az.StorageSync</span></span>
* <span data-ttu-id="01b15-1809">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="01b15-1809">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="01b15-1810">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-1810">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="01b15-1811">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-1811">Az.Accounts</span></span>
* <span data-ttu-id="01b15-1812">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="01b15-1812">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="01b15-1813">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="01b15-1813">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="01b15-1814">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="01b15-1814">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="01b15-1815">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="01b15-1815">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="01b15-1816">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="01b15-1816">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-1817">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-1817">Az.Compute</span></span>
* <span data-ttu-id="01b15-1818">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="01b15-1818">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="01b15-1819">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="01b15-1819">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="01b15-1820">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="01b15-1820">Az.Dns</span></span>
* <span data-ttu-id="01b15-1821">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="01b15-1821">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="01b15-1822">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="01b15-1822">Az.EventGrid</span></span>
* <span data-ttu-id="01b15-1823">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="01b15-1823">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="01b15-1824">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="01b15-1824">New cmdlets:</span></span>
    - <span data-ttu-id="01b15-1825">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="01b15-1825">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="01b15-1826">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="01b15-1826">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="01b15-1827">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="01b15-1827">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="01b15-1828">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-1828">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="01b15-1829">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="01b15-1829">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="01b15-1830">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="01b15-1830">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="01b15-1831">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="01b15-1831">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="01b15-1832">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="01b15-1832">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="01b15-1833">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="01b15-1833">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="01b15-1834">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="01b15-1834">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="01b15-1835">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="01b15-1835">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="01b15-1836">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="01b15-1836">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="01b15-1837">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="01b15-1837">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="01b15-1838">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="01b15-1838">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span>
    - <span data-ttu-id="01b15-1839">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="01b15-1839">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="01b15-1840">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="01b15-1840">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="01b15-1841">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="01b15-1841">Updated cmdlets:</span></span>
    - <span data-ttu-id="01b15-1842">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="01b15-1842">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="01b15-1843">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="01b15-1843">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="01b15-1844">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="01b15-1844">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="01b15-1845">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="01b15-1845">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="01b15-1846">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="01b15-1846">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="01b15-1847">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="01b15-1847">Event subscription expiration date,</span></span>
            - <span data-ttu-id="01b15-1848">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="01b15-1848">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="01b15-1849">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="01b15-1849">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="01b15-1850">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="01b15-1850">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span>
    - <span data-ttu-id="01b15-1851">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="01b15-1851">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="01b15-1852">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="01b15-1852">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="01b15-1853">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="01b15-1853">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="01b15-1854">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="01b15-1854">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="01b15-1855">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="01b15-1855">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="01b15-1856">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="01b15-1856">Az.FrontDoor</span></span>
* <span data-ttu-id="01b15-1857">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="01b15-1857">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="01b15-1858">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="01b15-1858">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="01b15-1859">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="01b15-1859">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="01b15-1860">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="01b15-1860">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-1861">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-1861">Az.Network</span></span>
* <span data-ttu-id="01b15-1862">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="01b15-1862">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="01b15-1863">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="01b15-1863">New cmdlets</span></span>
        - <span data-ttu-id="01b15-1864">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="01b15-1864">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="01b15-1865">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="01b15-1865">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="01b15-1866">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="01b15-1866">New cmdlets</span></span>
        - <span data-ttu-id="01b15-1867">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="01b15-1867">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="01b15-1868">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="01b15-1868">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="01b15-1869">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="01b15-1869">New cmdlets</span></span>
        - <span data-ttu-id="01b15-1870">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="01b15-1870">Get-AzPrivateLinkService</span></span>
        - <span data-ttu-id="01b15-1871">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="01b15-1871">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="01b15-1872">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="01b15-1872">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="01b15-1873">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-1873">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="01b15-1874">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-1874">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="01b15-1875">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="01b15-1875">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="01b15-1876">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="01b15-1876">New cmdlets</span></span>
        - <span data-ttu-id="01b15-1877">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="01b15-1877">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="01b15-1878">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="01b15-1878">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="01b15-1879">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="01b15-1879">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="01b15-1880">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-1880">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="01b15-1881">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="01b15-1881">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="01b15-1882">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="01b15-1882">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="01b15-1883">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="01b15-1883">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="01b15-1884">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="01b15-1884">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="01b15-1885">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="01b15-1885">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="01b15-1886">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="01b15-1886">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="01b15-1887">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="01b15-1887">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="01b15-1888">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="01b15-1888">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="01b15-1889">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="01b15-1889">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="01b15-1890">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="01b15-1890">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="01b15-1891">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="01b15-1891">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="01b15-1892">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="01b15-1892">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="01b15-1893">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="01b15-1893">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="01b15-1894">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="01b15-1894">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="01b15-1895">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="01b15-1895">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="01b15-1896">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="01b15-1896">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="01b15-1897">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="01b15-1897">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="01b15-1898">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="01b15-1898">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="01b15-1899">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="01b15-1899">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span>
* <span data-ttu-id="01b15-1900">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="01b15-1900">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span>
    - <span data-ttu-id="01b15-1901">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="01b15-1901">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="01b15-1902">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="01b15-1902">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="01b15-1903">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="01b15-1903">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="01b15-1904">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-1904">Az.OperationalInsights</span></span>
* <span data-ttu-id="01b15-1905">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="01b15-1905">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-1906">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-1906">Az.Resources</span></span>
* <span data-ttu-id="01b15-1907">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="01b15-1907">Support for additional Template Export options</span></span>
    - <span data-ttu-id="01b15-1908">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="01b15-1908">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="01b15-1909">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="01b15-1909">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="01b15-1910">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="01b15-1910">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="01b15-1911">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="01b15-1911">Az.ServiceFabric</span></span>
* <span data-ttu-id="01b15-1912">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="01b15-1912">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-1913">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-1913">Az.Sql</span></span>
* <span data-ttu-id="01b15-1914">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="01b15-1914">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="01b15-1915">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="01b15-1915">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="01b15-1916">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="01b15-1916">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="01b15-1917">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="01b15-1917">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="01b15-1918">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="01b15-1918">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="01b15-1919">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="01b15-1919">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="01b15-1920">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="01b15-1920">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="01b15-1921">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="01b15-1921">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-1922">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-1922">Az.Storage</span></span>
* <span data-ttu-id="01b15-1923">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="01b15-1923">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="01b15-1924">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="01b15-1924">New-AzStorageAccount</span></span>
* <span data-ttu-id="01b15-1925">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="01b15-1925">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="01b15-1926">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="01b15-1926">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="01b15-1927">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-1927">Az.Websites</span></span>
* <span data-ttu-id="01b15-1928">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="01b15-1928">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="01b15-1929">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="01b15-1929">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="01b15-1930">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-1930">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="01b15-1931">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="01b15-1931">Az.Cdn</span></span>
* <span data-ttu-id="01b15-1932">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="01b15-1932">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-1933">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-1933">Az.Compute</span></span>
* <span data-ttu-id="01b15-1934">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="01b15-1934">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="01b15-1935">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="01b15-1935">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="01b15-1936">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="01b15-1936">Az.EventHub</span></span>
* <span data-ttu-id="01b15-1937">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="01b15-1937">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="01b15-1938">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="01b15-1938">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-1939">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-1939">Az.Network</span></span>
* <span data-ttu-id="01b15-1940">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="01b15-1940">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="01b15-1941">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="01b15-1941">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="01b15-1942">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-1942">Az.PolicyInsights</span></span>
* <span data-ttu-id="01b15-1943">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="01b15-1943">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-1944">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-1944">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-1945">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="01b15-1945">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="01b15-1946">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="01b15-1946">Az.ServiceBus</span></span>
* <span data-ttu-id="01b15-1947">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="01b15-1947">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="01b15-1948">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="01b15-1948">Az.ServiceFabric</span></span>
* <span data-ttu-id="01b15-1949">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="01b15-1949">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="01b15-1950">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="01b15-1950">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-1951">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-1951">Az.Sql</span></span>
* <span data-ttu-id="01b15-1952">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="01b15-1952">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="01b15-1953">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="01b15-1953">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="01b15-1954">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="01b15-1954">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="01b15-1955">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="01b15-1955">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="01b15-1956">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-1956">Az.Websites</span></span>
* <span data-ttu-id="01b15-1957">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="01b15-1957">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="01b15-1958">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-1958">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="01b15-1959">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="01b15-1959">Az.ApiManagement</span></span>
* <span data-ttu-id="01b15-1960">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="01b15-1960">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="01b15-1961">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="01b15-1961">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="01b15-1962">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="01b15-1962">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="01b15-1963">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="01b15-1963">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="01b15-1964">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="01b15-1964">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="01b15-1965">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="01b15-1965">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="01b15-1966">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="01b15-1966">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="01b15-1967">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="01b15-1967">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="01b15-1968">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="01b15-1968">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="01b15-1969">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="01b15-1969">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="01b15-1970">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="01b15-1970">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="01b15-1971">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="01b15-1971">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="01b15-1972">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="01b15-1972">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="01b15-1973">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="01b15-1973">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="01b15-1974">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="01b15-1974">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="01b15-1975">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="01b15-1975">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="01b15-1976">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="01b15-1976">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="01b15-1977">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="01b15-1977">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="01b15-1978">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="01b15-1978">Created new Cmdlet for generating a User Token.</span></span>
    - <span data-ttu-id="01b15-1979">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="01b15-1979">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="01b15-1980">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="01b15-1980">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="01b15-1981">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="01b15-1981">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="01b15-1982">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="01b15-1982">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="01b15-1983">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="01b15-1983">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span>
    - <span data-ttu-id="01b15-1984">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="01b15-1984">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="01b15-1985">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="01b15-1985">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="01b15-1986">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="01b15-1986">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="01b15-1987">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="01b15-1987">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="01b15-1988">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="01b15-1988">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="01b15-1989">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="01b15-1989">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="01b15-1990">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="01b15-1990">Updated the cmdlet to display Error Messages inline</span></span>
     > <span data-ttu-id="01b15-1991">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="01b15-1991">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="01b15-1992">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="01b15-1992">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="01b15-1993">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="01b15-1993">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="01b15-1994">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="01b15-1994">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="01b15-1995">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="01b15-1995">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="01b15-1996">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="01b15-1996">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="01b15-1997">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="01b15-1997">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="01b15-1998">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="01b15-1998">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="01b15-1999">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="01b15-1999">Updated cmdlet **New-AzApiManagementApi**</span></span>
    - <span data-ttu-id="01b15-2000">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="01b15-2000">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="01b15-2001">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="01b15-2001">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="01b15-2002">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="01b15-2002">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="01b15-2003">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="01b15-2003">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="01b15-2004">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="01b15-2004">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="01b15-2005">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="01b15-2005">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="01b15-2006">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="01b15-2006">To updated an API into an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="01b15-2007">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="01b15-2007">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="01b15-2008">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="01b15-2008">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="01b15-2009">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="01b15-2009">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="01b15-2010">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="01b15-2010">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="01b15-2011">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="01b15-2011">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="01b15-2012">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="01b15-2012">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="01b15-2013">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="01b15-2013">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="01b15-2014">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="01b15-2014">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="01b15-2015">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="01b15-2015">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="01b15-2016">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="01b15-2016">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="01b15-2017">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="01b15-2017">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="01b15-2018">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="01b15-2018">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="01b15-2019">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="01b15-2019">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="01b15-2020">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="01b15-2020">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="01b15-2021">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="01b15-2021">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="01b15-2022">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="01b15-2022">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="01b15-2023">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="01b15-2023">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="01b15-2024">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="01b15-2024">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="01b15-2025">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="01b15-2025">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="01b15-2026">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="01b15-2026">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="01b15-2027">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="01b15-2027">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="01b15-2028">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="01b15-2028">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="01b15-2029">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="01b15-2029">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="01b15-2030">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="01b15-2030">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="01b15-2031">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="01b15-2031">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="01b15-2032">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="01b15-2032">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="01b15-2033">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="01b15-2033">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="01b15-2034">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="01b15-2034">'Get-AzApiManagementCertificate'</span></span>
    - <span data-ttu-id="01b15-2035">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="01b15-2035">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="01b15-2036">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="01b15-2036">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="01b15-2037">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="01b15-2037">Az.Automation</span></span>
* <span data-ttu-id="01b15-2038">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="01b15-2038">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="01b15-2039">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="01b15-2039">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="01b15-2040">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="01b15-2040">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="01b15-2041">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="01b15-2041">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="01b15-2042">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="01b15-2042">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="01b15-2043">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="01b15-2043">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="01b15-2044">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="01b15-2044">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-2045">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-2045">Az.Compute</span></span>
* <span data-ttu-id="01b15-2046">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="01b15-2046">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="01b15-2047">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="01b15-2047">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="01b15-2048">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="01b15-2048">Az.DataLakeStore</span></span>
* <span data-ttu-id="01b15-2049">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="01b15-2049">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="01b15-2050">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="01b15-2050">Az.Monitor</span></span>
* <span data-ttu-id="01b15-2051">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="01b15-2051">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-2052">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-2052">Az.Network</span></span>
* <span data-ttu-id="01b15-2053">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="01b15-2053">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="01b15-2054">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="01b15-2054">Updated cmdlet:</span></span>
        - <span data-ttu-id="01b15-2055">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="01b15-2055">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="01b15-2056">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="01b15-2056">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-2057">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-2057">Az.Resources</span></span>
* <span data-ttu-id="01b15-2058">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="01b15-2058">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-2059">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-2059">Az.Sql</span></span>
* <span data-ttu-id="01b15-2060">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="01b15-2060">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="01b15-2061">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-2061">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="01b15-2062">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-2062">Az.Accounts</span></span>
* <span data-ttu-id="01b15-2063">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="01b15-2063">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="01b15-2064">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="01b15-2064">Az.CognitiveServices</span></span>
* <span data-ttu-id="01b15-2065">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="01b15-2065">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="01b15-2066">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="01b15-2066">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-2067">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-2067">Az.Compute</span></span>
* <span data-ttu-id="01b15-2068">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="01b15-2068">Proximity placement group feature.</span></span>
    - <span data-ttu-id="01b15-2069">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="01b15-2069">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="01b15-2070">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-2070">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="01b15-2071">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="01b15-2071">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="01b15-2072">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="01b15-2072">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="01b15-2073">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="01b15-2073">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>
* <span data-ttu-id="01b15-2074">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="01b15-2074">Breaking changes</span></span>
    - <span data-ttu-id="01b15-2075">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="01b15-2075">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="01b15-2076">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="01b15-2076">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="01b15-2077">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="01b15-2077">Az.DeploymentManager</span></span>
* <span data-ttu-id="01b15-2078">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="01b15-2078">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="01b15-2079">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="01b15-2079">Az.Dns</span></span>
* <span data-ttu-id="01b15-2080">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="01b15-2080">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="01b15-2081">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="01b15-2081">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="01b15-2082">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="01b15-2082">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="01b15-2083">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="01b15-2083">Az.FrontDoor</span></span>
* <span data-ttu-id="01b15-2084">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="01b15-2084">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="01b15-2085">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="01b15-2085">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="01b15-2086">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="01b15-2086">Az.HDInsight</span></span>
* <span data-ttu-id="01b15-2087">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="01b15-2087">Removed two cmdlets:</span></span>
    - <span data-ttu-id="01b15-2088">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="01b15-2088">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="01b15-2089">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="01b15-2089">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="01b15-2090">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="01b15-2090">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="01b15-2091">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="01b15-2091">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="01b15-2092">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="01b15-2092">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="01b15-2093">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="01b15-2093">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="01b15-2094">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="01b15-2094">Az.Monitor</span></span>
* <span data-ttu-id="01b15-2095">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="01b15-2095">New cmdlets for SQR API (Scheduled Query Rule)</span></span>
    - <span data-ttu-id="01b15-2096">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="01b15-2096">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="01b15-2097">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="01b15-2097">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="01b15-2098">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="01b15-2098">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="01b15-2099">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="01b15-2099">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="01b15-2100">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="01b15-2100">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="01b15-2101">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="01b15-2101">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="01b15-2102">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="01b15-2102">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="01b15-2103">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="01b15-2103">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="01b15-2104">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="01b15-2104">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="01b15-2105">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="01b15-2105">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="01b15-2106">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="01b15-2106">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="01b15-2107">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="01b15-2107">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="01b15-2108">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="01b15-2108">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-2109">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-2109">Az.Network</span></span>
* <span data-ttu-id="01b15-2110">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="01b15-2110">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="01b15-2111">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="01b15-2111">New cmdlets</span></span>
        - <span data-ttu-id="01b15-2112">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="01b15-2112">New-AzNatGateway</span></span>
        - <span data-ttu-id="01b15-2113">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="01b15-2113">Get-AzNatGateway</span></span>
        - <span data-ttu-id="01b15-2114">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="01b15-2114">Set-AzNatGateway</span></span>
        - <span data-ttu-id="01b15-2115">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="01b15-2115">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="01b15-2116">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="01b15-2116">Updated cmdlets</span></span>
        - <span data-ttu-id="01b15-2117">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="01b15-2117">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="01b15-2118">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="01b15-2118">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="01b15-2119">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="01b15-2119">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="01b15-2120">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="01b15-2120">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="01b15-2121">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="01b15-2121">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="01b15-2122">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-2122">Az.PolicyInsights</span></span>
* <span data-ttu-id="01b15-2123">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="01b15-2123">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="01b15-2124">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="01b15-2124">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="01b15-2125">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="01b15-2125">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-2126">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-2126">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-2127">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="01b15-2127">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="01b15-2128">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="01b15-2128">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="01b15-2129">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="01b15-2129">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="01b15-2130">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-2130">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="01b15-2131">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="01b15-2131">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="01b15-2132">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="01b15-2132">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="01b15-2133">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="01b15-2133">Az.Relay</span></span>
* <span data-ttu-id="01b15-2134">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="01b15-2134">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="01b15-2135">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="01b15-2135">Az.ServiceBus</span></span>
* <span data-ttu-id="01b15-2136">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="01b15-2136">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-2137">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-2137">Az.Storage</span></span>
* <span data-ttu-id="01b15-2138">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="01b15-2138">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="01b15-2139">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="01b15-2139">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="01b15-2140">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="01b15-2140">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="01b15-2141">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="01b15-2141">New-AzStorageAccount</span></span>
* <span data-ttu-id="01b15-2142">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="01b15-2142">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="01b15-2143">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="01b15-2143">New-AzStorageAccount</span></span>
    - <span data-ttu-id="01b15-2144">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="01b15-2144">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="01b15-2145">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="01b15-2145">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="01b15-2146">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-2146">Az.Websites</span></span>
* <span data-ttu-id="01b15-2147">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="01b15-2147">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="01b15-2148">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="01b15-2148">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="01b15-2149">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-2149">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="01b15-2150">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="01b15-2150">Highlights since the last major release</span></span>
* <span data-ttu-id="01b15-2151">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="01b15-2151">General availability of `Az` module</span></span>
* <span data-ttu-id="01b15-2152">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="01b15-2152">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="01b15-2153">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="01b15-2153">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="01b15-2154">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-2154">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="01b15-2155">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="01b15-2155">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="01b15-2156">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="01b15-2156">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="01b15-2157">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="01b15-2157">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="01b15-2158">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-2158">Az.Accounts</span></span>
* <span data-ttu-id="01b15-2159">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="01b15-2159">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="01b15-2160">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="01b15-2160">Az.Batch</span></span>
* <span data-ttu-id="01b15-2161">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="01b15-2161">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="01b15-2162">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="01b15-2162">Az.Cdn</span></span>
* <span data-ttu-id="01b15-2163">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="01b15-2163">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="01b15-2164">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="01b15-2164">Az.CognitiveServices</span></span>
* <span data-ttu-id="01b15-2165">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="01b15-2165">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-2166">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-2166">Az.Compute</span></span>
* <span data-ttu-id="01b15-2167">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="01b15-2167">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="01b15-2168">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="01b15-2168">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="01b15-2169">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="01b15-2169">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="01b15-2170">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="01b15-2170">Az.DataFactory</span></span>
* <span data-ttu-id="01b15-2171">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="01b15-2171">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="01b15-2172">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="01b15-2172">Az.DataLakeStore</span></span>
* <span data-ttu-id="01b15-2173">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="01b15-2173">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="01b15-2174">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="01b15-2174">Az.EventGrid</span></span>
* <span data-ttu-id="01b15-2175">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="01b15-2175">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="01b15-2176">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="01b15-2176">Az.EventHub</span></span>
* <span data-ttu-id="01b15-2177">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="01b15-2177">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="01b15-2178">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="01b15-2178">Az.HDInsight</span></span>
* <span data-ttu-id="01b15-2179">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="01b15-2179">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="01b15-2180">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="01b15-2180">Az.IotHub</span></span>
* <span data-ttu-id="01b15-2181">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="01b15-2181">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="01b15-2182">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b15-2182">Az.KeyVault</span></span>
* <span data-ttu-id="01b15-2183">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="01b15-2183">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="01b15-2184">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="01b15-2184">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="01b15-2185">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="01b15-2185">Az.MachineLearning</span></span>
* <span data-ttu-id="01b15-2186">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="01b15-2186">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="01b15-2187">Az.Media</span><span class="sxs-lookup"><span data-stu-id="01b15-2187">Az.Media</span></span>
* <span data-ttu-id="01b15-2188">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="01b15-2188">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="01b15-2189">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="01b15-2189">Az.Monitor</span></span>
  * <span data-ttu-id="01b15-2190">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="01b15-2190">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="01b15-2191">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="01b15-2191">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="01b15-2192">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="01b15-2192">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="01b15-2193">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="01b15-2193">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="01b15-2194">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="01b15-2194">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="01b15-2195">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="01b15-2195">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="01b15-2196">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="01b15-2196">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-2197">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-2197">Az.Network</span></span>
* <span data-ttu-id="01b15-2198">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="01b15-2198">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="01b15-2199">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="01b15-2199">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="01b15-2200">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="01b15-2200">Az.NotificationHubs</span></span>
* <span data-ttu-id="01b15-2201">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="01b15-2201">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="01b15-2202">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-2202">Az.OperationalInsights</span></span>
* <span data-ttu-id="01b15-2203">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="01b15-2203">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="01b15-2204">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="01b15-2204">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="01b15-2205">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="01b15-2205">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-2206">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-2206">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-2207">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="01b15-2207">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="01b15-2208">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="01b15-2208">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="01b15-2209">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="01b15-2209">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="01b15-2210">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="01b15-2210">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="01b15-2211">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="01b15-2211">Az.RedisCache</span></span>
* <span data-ttu-id="01b15-2212">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="01b15-2212">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-2213">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-2213">Az.Resources</span></span>
* <span data-ttu-id="01b15-2214">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="01b15-2214">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-2215">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-2215">Az.Sql</span></span>
* <span data-ttu-id="01b15-2216">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="01b15-2216">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="01b15-2217">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="01b15-2217">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="01b15-2218">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="01b15-2218">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="01b15-2219">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="01b15-2219">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="01b15-2220">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="01b15-2220">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="01b15-2221">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="01b15-2221">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="01b15-2222">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="01b15-2222">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="01b15-2223">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-2223">Az.Websites</span></span>
* <span data-ttu-id="01b15-2224">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="01b15-2224">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="01b15-2225">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="01b15-2225">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="01b15-2226">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="01b15-2226">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="01b15-2227">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="01b15-2227">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="01b15-2228">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-2228">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="01b15-2229">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="01b15-2229">Highlights since the last major release</span></span>
* <span data-ttu-id="01b15-2230">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="01b15-2230">General availability of `Az` module</span></span>
* <span data-ttu-id="01b15-2231">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="01b15-2231">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="01b15-2232">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="01b15-2232">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="01b15-2233">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-2233">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="01b15-2234">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="01b15-2234">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="01b15-2235">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="01b15-2235">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="01b15-2236">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="01b15-2236">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="01b15-2237">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-2237">Az.Accounts</span></span>
* <span data-ttu-id="01b15-2238">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="01b15-2238">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="01b15-2239">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="01b15-2239">Az.AnalysisServices</span></span>
* <span data-ttu-id="01b15-2240">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="01b15-2240">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="01b15-2241">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="01b15-2241">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="01b15-2242">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="01b15-2242">Az.Automation</span></span>
* <span data-ttu-id="01b15-2243">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="01b15-2243">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="01b15-2244">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="01b15-2244">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="01b15-2245">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="01b15-2245">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-2246">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-2246">Az.Compute</span></span>
* <span data-ttu-id="01b15-2247">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-2247">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="01b15-2248">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="01b15-2248">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="01b15-2249">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="01b15-2249">Az.ContainerInstance</span></span>
* <span data-ttu-id="01b15-2250">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="01b15-2250">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="01b15-2251">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="01b15-2251">Az.DataFactory</span></span>
* <span data-ttu-id="01b15-2252">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="01b15-2252">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="01b15-2253">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="01b15-2253">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-2254">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-2254">Az.Resources</span></span>
* <span data-ttu-id="01b15-2255">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="01b15-2255">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="01b15-2256">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="01b15-2256">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="01b15-2257">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="01b15-2257">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="01b15-2258">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="01b15-2258">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="01b15-2259">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="01b15-2259">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="01b15-2260">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="01b15-2260">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-2261">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-2261">Az.Sql</span></span>
* <span data-ttu-id="01b15-2262">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="01b15-2262">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-2263">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-2263">Az.Storage</span></span>
* <span data-ttu-id="01b15-2264">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="01b15-2264">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="01b15-2265">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="01b15-2265">New-AzStorageContext</span></span>
* <span data-ttu-id="01b15-2266">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="01b15-2266">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="01b15-2267">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="01b15-2267">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="01b15-2268">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="01b15-2268">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="01b15-2269">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="01b15-2269">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="01b15-2270">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="01b15-2270">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="01b15-2271">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="01b15-2271">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="01b15-2272">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="01b15-2272">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="01b15-2273">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="01b15-2273">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="01b15-2274">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="01b15-2274">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="01b15-2275">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="01b15-2275">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="01b15-2276">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-2276">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="01b15-2277">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="01b15-2277">Highlights since the last major release</span></span>
* <span data-ttu-id="01b15-2278">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="01b15-2278">General availability of `Az` module</span></span>
* <span data-ttu-id="01b15-2279">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="01b15-2279">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="01b15-2280">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="01b15-2280">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="01b15-2281">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-2281">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="01b15-2282">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="01b15-2282">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="01b15-2283">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="01b15-2283">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="01b15-2284">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="01b15-2284">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="01b15-2285">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="01b15-2285">Az.Automation</span></span>
* <span data-ttu-id="01b15-2286">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="01b15-2286">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="01b15-2287">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="01b15-2287">Dynamic grouping</span></span>
    * <span data-ttu-id="01b15-2288">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="01b15-2288">Pre-Post script</span></span>
    * <span data-ttu-id="01b15-2289">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="01b15-2289">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-2290">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-2290">Az.Compute</span></span>
* <span data-ttu-id="01b15-2291">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="01b15-2291">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="01b15-2292">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="01b15-2292">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="01b15-2293">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b15-2293">Az.KeyVault</span></span>
* <span data-ttu-id="01b15-2294">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b15-2294">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-2295">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-2295">Az.Network</span></span>
* <span data-ttu-id="01b15-2296">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="01b15-2296">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="01b15-2297">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="01b15-2297">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-2298">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-2298">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-2299">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="01b15-2299">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="01b15-2300">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="01b15-2300">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-2301">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-2301">Az.Resources</span></span>
* <span data-ttu-id="01b15-2302">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="01b15-2302">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="01b15-2303">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="01b15-2303">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-2304">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-2304">Az.Sql</span></span>
* <span data-ttu-id="01b15-2305">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="01b15-2305">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-2306">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-2306">Az.Storage</span></span>
* <span data-ttu-id="01b15-2307">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="01b15-2307">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="01b15-2308">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="01b15-2308">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="01b15-2309">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="01b15-2309">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="01b15-2310">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="01b15-2310">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="01b15-2311">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="01b15-2311">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="01b15-2312">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="01b15-2312">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="01b15-2313">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="01b15-2313">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="01b15-2314">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-2314">Az.Websites</span></span>
* <span data-ttu-id="01b15-2315">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="01b15-2315">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="01b15-2316">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-2316">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="01b15-2317">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-2317">Az.Accounts</span></span>
* <span data-ttu-id="01b15-2318">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="01b15-2318">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="01b15-2319">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="01b15-2319">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="01b15-2320">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="01b15-2320">Az.Automation</span></span>
* <span data-ttu-id="01b15-2321">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="01b15-2321">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="01b15-2322">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="01b15-2322">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="01b15-2323">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="01b15-2323">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="01b15-2324">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="01b15-2324">Az.Cdn</span></span>
* <span data-ttu-id="01b15-2325">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="01b15-2325">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-2326">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-2326">Az.Compute</span></span>
* <span data-ttu-id="01b15-2327">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="01b15-2327">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="01b15-2328">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="01b15-2328">Az.DataFactory</span></span>
* <span data-ttu-id="01b15-2329">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="01b15-2329">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="01b15-2330">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="01b15-2330">Az.LogicApp</span></span>
* <span data-ttu-id="01b15-2331">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="01b15-2331">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-2332">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-2332">Az.Network</span></span>
* <span data-ttu-id="01b15-2333">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="01b15-2333">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-2334">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-2334">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-2335">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="01b15-2335">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="01b15-2336">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="01b15-2336">SDK Update</span></span>
* <span data-ttu-id="01b15-2337">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="01b15-2337">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="01b15-2338">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="01b15-2338">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-2339">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-2339">Az.Resources</span></span>
* <span data-ttu-id="01b15-2340">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="01b15-2340">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="01b15-2341">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="01b15-2341">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="01b15-2342">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="01b15-2342">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="01b15-2343">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="01b15-2343">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="01b15-2344">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="01b15-2344">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="01b15-2345">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="01b15-2345">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-2346">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-2346">Az.Sql</span></span>
* <span data-ttu-id="01b15-2347">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="01b15-2347">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="01b15-2348">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="01b15-2348">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-2349">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-2349">Az.Storage</span></span>
* <span data-ttu-id="01b15-2350">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="01b15-2350">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="01b15-2351">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-2351">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="01b15-2352">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="01b15-2352">Az.AnalysisServices</span></span>
* <span data-ttu-id="01b15-2353">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="01b15-2353">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="01b15-2354">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="01b15-2354">Az.Automation</span></span>
* <span data-ttu-id="01b15-2355">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="01b15-2355">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="01b15-2356">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="01b15-2356">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="01b15-2357">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="01b15-2357">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="01b15-2358">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="01b15-2358">Az.CognitiveServices</span></span>
* <span data-ttu-id="01b15-2359">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="01b15-2359">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-2360">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-2360">Az.Compute</span></span>
* <span data-ttu-id="01b15-2361">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="01b15-2361">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="01b15-2362">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="01b15-2362">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="01b15-2363">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="01b15-2363">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="01b15-2364">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="01b15-2364">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="01b15-2365">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="01b15-2365">Az.DataLakeStore</span></span>
* <span data-ttu-id="01b15-2366">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="01b15-2366">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="01b15-2367">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="01b15-2367">Az.EventHub</span></span>
* <span data-ttu-id="01b15-2368">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="01b15-2368">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="01b15-2369">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b15-2369">Az.KeyVault</span></span>
* <span data-ttu-id="01b15-2370">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="01b15-2370">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="01b15-2371">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="01b15-2371">Az.LogicApp</span></span>
* <span data-ttu-id="01b15-2372">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="01b15-2372">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="01b15-2373">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="01b15-2373">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="01b15-2374">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="01b15-2374">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="01b15-2375">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="01b15-2375">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="01b15-2376">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="01b15-2376">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="01b15-2377">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="01b15-2377">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="01b15-2378">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="01b15-2378">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="01b15-2379">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="01b15-2379">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="01b15-2380">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="01b15-2380">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="01b15-2381">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="01b15-2381">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="01b15-2382">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="01b15-2382">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="01b15-2383">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="01b15-2383">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="01b15-2384">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="01b15-2384">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="01b15-2385">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="01b15-2385">Az.Monitor</span></span>
* <span data-ttu-id="01b15-2386">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="01b15-2386">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-2387">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-2387">Az.Network</span></span>
* <span data-ttu-id="01b15-2388">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="01b15-2388">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="01b15-2389">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-2389">Az.OperationalInsights</span></span>
* <span data-ttu-id="01b15-2390">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="01b15-2390">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="01b15-2391">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="01b15-2391">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="01b15-2392">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="01b15-2392">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-2393">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-2393">Az.Resources</span></span>
* <span data-ttu-id="01b15-2394">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="01b15-2394">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="01b15-2395">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="01b15-2395">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="01b15-2396">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="01b15-2396">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="01b15-2397">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="01b15-2397">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-2398">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-2398">Az.Sql</span></span>
* <span data-ttu-id="01b15-2399">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="01b15-2399">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="01b15-2400">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="01b15-2400">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="01b15-2401">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-2401">Az.Websites</span></span>
* <span data-ttu-id="01b15-2402">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="01b15-2402">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="01b15-2403">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-2403">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="01b15-2404">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-2404">Az.Accounts</span></span>
* <span data-ttu-id="01b15-2405">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="01b15-2405">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="01b15-2406">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="01b15-2406">Az.AnalysisServices</span></span>
<span data-ttu-id="01b15-2407">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="01b15-2407">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-2408">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-2408">Az.Compute</span></span>
* <span data-ttu-id="01b15-2409">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="01b15-2409">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="01b15-2410">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="01b15-2410">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="01b15-2411">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="01b15-2411">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-2412">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-2412">Az.RecoveryServices</span></span>
<span data-ttu-id="01b15-2413">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="01b15-2413">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-2414">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-2414">Az.Resources</span></span>
* <span data-ttu-id="01b15-2415">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="01b15-2415">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="01b15-2416">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="01b15-2416">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="01b15-2417">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="01b15-2417">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="01b15-2418">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="01b15-2418">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-2419">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-2419">Az.Sql</span></span>
* <span data-ttu-id="01b15-2420">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="01b15-2420">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="01b15-2421">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="01b15-2421">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="01b15-2422">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="01b15-2422">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="01b15-2423">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-2423">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="01b15-2424">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-2424">Az.Accounts</span></span>
* <span data-ttu-id="01b15-2425">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="01b15-2425">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="01b15-2426">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="01b15-2426">Az.AnalysisServices</span></span>
* <span data-ttu-id="01b15-2427">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="01b15-2427">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-2428">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-2428">Az.RecoveryServices</span></span>
* <span data-ttu-id="01b15-2429">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="01b15-2429">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="01b15-2430">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-2430">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="01b15-2431">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-2431">Az.Accounts</span></span>
* <span data-ttu-id="01b15-2432">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="01b15-2432">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="01b15-2433">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="01b15-2433">Update incorrect online help URLs</span></span>
* <span data-ttu-id="01b15-2434">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="01b15-2434">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="01b15-2435">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="01b15-2435">Az.Aks</span></span>
* <span data-ttu-id="01b15-2436">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="01b15-2436">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="01b15-2437">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="01b15-2437">Az.Automation</span></span>
* <span data-ttu-id="01b15-2438">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="01b15-2438">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="01b15-2439">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="01b15-2439">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="01b15-2440">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="01b15-2440">Az.Cdn</span></span>
* <span data-ttu-id="01b15-2441">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="01b15-2441">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-2442">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-2442">Az.Compute</span></span>
* <span data-ttu-id="01b15-2443">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="01b15-2443">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="01b15-2444">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="01b15-2444">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="01b15-2445">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="01b15-2445">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="01b15-2446">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="01b15-2446">Az.ContainerRegistry</span></span>
* <span data-ttu-id="01b15-2447">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="01b15-2447">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="01b15-2448">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="01b15-2448">Az.DataFactory</span></span>
* <span data-ttu-id="01b15-2449">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="01b15-2449">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="01b15-2450">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="01b15-2450">Az.DataLakeStore</span></span>
* <span data-ttu-id="01b15-2451">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="01b15-2451">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="01b15-2452">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="01b15-2452">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="01b15-2453">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="01b15-2453">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="01b15-2454">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="01b15-2454">Az.IotHub</span></span>
* <span data-ttu-id="01b15-2455">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="01b15-2455">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="01b15-2456">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b15-2456">Az.KeyVault</span></span>
* <span data-ttu-id="01b15-2457">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="01b15-2457">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-2458">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-2458">Az.Network</span></span>
* <span data-ttu-id="01b15-2459">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="01b15-2459">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-2460">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-2460">Az.Resources</span></span>
* <span data-ttu-id="01b15-2461">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="01b15-2461">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="01b15-2462">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="01b15-2462">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="01b15-2463">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="01b15-2463">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="01b15-2464">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="01b15-2464">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="01b15-2465">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="01b15-2465">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="01b15-2466">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="01b15-2466">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="01b15-2467">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="01b15-2467">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="01b15-2468">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="01b15-2468">Az.ServiceFabric</span></span>
* <span data-ttu-id="01b15-2469">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="01b15-2469">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="01b15-2470">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="01b15-2470">Fix some error messages.</span></span>
* <span data-ttu-id="01b15-2471">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="01b15-2471">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="01b15-2472">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="01b15-2472">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="01b15-2473">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="01b15-2473">Az.SignalR</span></span>
* <span data-ttu-id="01b15-2474">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="01b15-2474">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-2475">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-2475">Az.Sql</span></span>
* <span data-ttu-id="01b15-2476">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="01b15-2476">Update incorrect online help URLs</span></span>
* <span data-ttu-id="01b15-2477">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="01b15-2477">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="01b15-2478">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="01b15-2478">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="01b15-2479">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="01b15-2479">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-2480">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-2480">Az.Storage</span></span>
* <span data-ttu-id="01b15-2481">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="01b15-2481">Update incorrect online help URLs</span></span>
* <span data-ttu-id="01b15-2482">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="01b15-2482">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="01b15-2483">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="01b15-2483">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="01b15-2484">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="01b15-2484">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="01b15-2485">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="01b15-2485">Az.TrafficManager</span></span>
* <span data-ttu-id="01b15-2486">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="01b15-2486">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="01b15-2487">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-2487">Az.Websites</span></span>
* <span data-ttu-id="01b15-2488">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="01b15-2488">Update incorrect online help URLs</span></span>
* <span data-ttu-id="01b15-2489">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="01b15-2489">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="01b15-2490">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="01b15-2490">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="01b15-2491">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="01b15-2491">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="01b15-2492">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-2492">Az.Accounts</span></span>
* <span data-ttu-id="01b15-2493">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="01b15-2493">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-2494">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-2494">Az.Compute</span></span>
* <span data-ttu-id="01b15-2495">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="01b15-2495">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="01b15-2496">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="01b15-2496">Updated the description of ID in help files</span></span>
* <span data-ttu-id="01b15-2497">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-2497">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="01b15-2498">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="01b15-2498">Az.DataLakeStore</span></span>
* <span data-ttu-id="01b15-2499">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="01b15-2499">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="01b15-2500">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="01b15-2500">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="01b15-2501">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="01b15-2501">Az.EventGrid</span></span>
* <span data-ttu-id="01b15-2502">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="01b15-2502">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="01b15-2503">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="01b15-2503">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="01b15-2504">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="01b15-2504">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="01b15-2505">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="01b15-2505">Event Time-To-Live,</span></span>
        - <span data-ttu-id="01b15-2506">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="01b15-2506">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="01b15-2507">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="01b15-2507">Dead letter endpoint.</span></span>
    - <span data-ttu-id="01b15-2508">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="01b15-2508">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="01b15-2509">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="01b15-2509">Event Time-To-Live,</span></span>
        - <span data-ttu-id="01b15-2510">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="01b15-2510">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="01b15-2511">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="01b15-2511">Dead letter endpoint.</span></span>
* <span data-ttu-id="01b15-2512">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="01b15-2512">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="01b15-2513">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="01b15-2513">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="01b15-2514">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="01b15-2514">Az.IotHub</span></span>
* <span data-ttu-id="01b15-2515">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="01b15-2515">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="01b15-2516">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="01b15-2516">Az.LogicApp</span></span>
* <span data-ttu-id="01b15-2517">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="01b15-2517">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-2518">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-2518">Az.Resources</span></span>
* <span data-ttu-id="01b15-2519">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="01b15-2519">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="01b15-2520">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="01b15-2520">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="01b15-2521">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="01b15-2521">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="01b15-2522">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="01b15-2522">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="01b15-2523">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="01b15-2523">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="01b15-2524">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="01b15-2524">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="01b15-2525">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="01b15-2525">Az.SignalR</span></span>
* <span data-ttu-id="01b15-2526">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-2526">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-2527">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-2527">Az.Sql</span></span>
* <span data-ttu-id="01b15-2528">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="01b15-2528">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="01b15-2529">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-2529">Az.Storage</span></span>
* <span data-ttu-id="01b15-2530">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="01b15-2530">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="01b15-2531">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="01b15-2531">New-AzStorageContext</span></span>
* <span data-ttu-id="01b15-2532">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="01b15-2532">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="01b15-2533">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="01b15-2533">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="01b15-2534">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-2534">Az.Websites</span></span>
* <span data-ttu-id="01b15-2535">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="01b15-2535">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="01b15-2536">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-2536">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="01b15-2537">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="01b15-2537">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="01b15-2538">Geral</span><span class="sxs-lookup"><span data-stu-id="01b15-2538">General</span></span>

- <span data-ttu-id="01b15-2539">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="01b15-2539">General Availability of Az Module</span></span>
- <span data-ttu-id="01b15-2540">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="01b15-2540">Online help for each module</span></span>
- <span data-ttu-id="01b15-2541">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="01b15-2541">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="01b15-2542">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="01b15-2542">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="01b15-2543">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-2543">Az.Accounts</span></span>
- <span data-ttu-id="01b15-2544">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="01b15-2544">Changed from Az.Profile</span></span>
- <span data-ttu-id="01b15-2545">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="01b15-2545">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="01b15-2546">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="01b15-2546">Az.ApiManagement</span></span>
- <span data-ttu-id="01b15-2547">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="01b15-2547">Fixes for #7002</span></span>
- <span data-ttu-id="01b15-2548">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="01b15-2548">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="01b15-2549">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="01b15-2549">Az.Batch</span></span>
- <span data-ttu-id="01b15-2550">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="01b15-2550">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="01b15-2551">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="01b15-2551">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="01b15-2552">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="01b15-2552">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="01b15-2553">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="01b15-2553">Az.Billing</span></span>
- <span data-ttu-id="01b15-2554">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="01b15-2554">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="01b15-2555">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="01b15-2555">Az.CognitivServices</span></span>
- <span data-ttu-id="01b15-2556">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="01b15-2556">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="01b15-2557">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="01b15-2557">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="01b15-2558">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="01b15-2558">Az.ContainerInstance</span></span>
- <span data-ttu-id="01b15-2559">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="01b15-2559">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="01b15-2560">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="01b15-2560">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="01b15-2561">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="01b15-2561">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="01b15-2562">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="01b15-2562">Az.DataLakeStore</span></span>
- <span data-ttu-id="01b15-2563">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="01b15-2563">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="01b15-2564">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="01b15-2564">Az.Monitor</span></span>
- <span data-ttu-id="01b15-2565">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="01b15-2565">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="01b15-2566">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="01b15-2566">Az.KeyVault</span></span>
- <span data-ttu-id="01b15-2567">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="01b15-2567">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="01b15-2568">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="01b15-2568">Az.MachineLearning</span></span>
- <span data-ttu-id="01b15-2569">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="01b15-2569">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="01b15-2570">Az.Media</span><span class="sxs-lookup"><span data-stu-id="01b15-2570">Az.Media</span></span>
- <span data-ttu-id="01b15-2571">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="01b15-2571">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="01b15-2572">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-2572">Az.Network</span></span>
<span data-ttu-id="01b15-2573">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="01b15-2573">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="01b15-2574">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="01b15-2574">New cmdlets added:</span></span>
        - <span data-ttu-id="01b15-2575">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="01b15-2575">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="01b15-2576">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="01b15-2576">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="01b15-2577">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="01b15-2577">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="01b15-2578">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="01b15-2578">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="01b15-2579">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="01b15-2579">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="01b15-2580">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="01b15-2580">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="01b15-2581">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="01b15-2581">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="01b15-2582">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="01b15-2582">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="01b15-2583">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="01b15-2583">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="01b15-2584">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="01b15-2584">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="01b15-2585">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="01b15-2585">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="01b15-2586">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="01b15-2586">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="01b15-2587">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-2587">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="01b15-2588">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-2588">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="01b15-2589">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="01b15-2589">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="01b15-2590">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="01b15-2590">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="01b15-2591">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="01b15-2591">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="01b15-2592">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="01b15-2592">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="01b15-2593">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="01b15-2593">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="01b15-2594">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="01b15-2594">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="01b15-2595">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="01b15-2595">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="01b15-2596">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-2596">Az.OperationalInsights</span></span>
- <span data-ttu-id="01b15-2597">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="01b15-2597">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="01b15-2598">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="01b15-2598">Az.Profile</span></span>
- <span data-ttu-id="01b15-2599">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="01b15-2599">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-2600">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-2600">Az.RecoveryServices</span></span>
- <span data-ttu-id="01b15-2601">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="01b15-2601">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="01b15-2602">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-2602">Az.Resources</span></span>
- <span data-ttu-id="01b15-2603">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="01b15-2603">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="01b15-2604">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="01b15-2604">Az.ServiceFabric</span></span>
- <span data-ttu-id="01b15-2605">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="01b15-2605">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="01b15-2606">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="01b15-2606">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="01b15-2607">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="01b15-2607">Az.SIgnalR</span></span>
- <span data-ttu-id="01b15-2608">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="01b15-2608">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="01b15-2609">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-2609">Az.Sql</span></span>
- <span data-ttu-id="01b15-2610">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="01b15-2610">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="01b15-2611">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="01b15-2611">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="01b15-2612">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="01b15-2612">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="01b15-2613">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-2613">Az.Storage</span></span>
- <span data-ttu-id="01b15-2614">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="01b15-2614">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="01b15-2615">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-2615">Az.Websites</span></span>
- <span data-ttu-id="01b15-2616">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="01b15-2616">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="01b15-2617">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="01b15-2617">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="01b15-2618">Geral</span><span class="sxs-lookup"><span data-stu-id="01b15-2618">General</span></span>

* <span data-ttu-id="01b15-2619">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="01b15-2619">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="01b15-2620">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-2620">Az.Compute</span></span>

* <span data-ttu-id="01b15-2621">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="01b15-2621">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="01b15-2622">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="01b15-2622">Az.DataLakeStore</span></span>

* <span data-ttu-id="01b15-2623">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="01b15-2623">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="01b15-2624">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="01b15-2624">Az.FrontDoor</span></span>

* <span data-ttu-id="01b15-2625">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="01b15-2625">Fixed some broken links</span></span>
    - <span data-ttu-id="01b15-2626">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="01b15-2626">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="01b15-2627">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="01b15-2627">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="01b15-2628">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="01b15-2628">Az.RecoveryServices</span></span>

* <span data-ttu-id="01b15-2629">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-2629">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="01b15-2630">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="01b15-2630">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="01b15-2631">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-2631">Az.Resources</span></span>

* <span data-ttu-id="01b15-2632">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="01b15-2632">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="01b15-2633">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="01b15-2633">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="01b15-2634">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-2634">Az.Sql</span></span>

* <span data-ttu-id="01b15-2635">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="01b15-2635">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="01b15-2636">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="01b15-2636">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="01b15-2637">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="01b15-2637">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="01b15-2638">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-2638">Az.Storage</span></span>

* <span data-ttu-id="01b15-2639">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="01b15-2639">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="01b15-2640">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="01b15-2640">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="01b15-2641">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="01b15-2641">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="01b15-2642">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="01b15-2642">Support Static Website configuration</span></span>
    - <span data-ttu-id="01b15-2643">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="01b15-2643">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="01b15-2644">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="01b15-2644">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="01b15-2645">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-2645">Az.Websites</span></span>

* <span data-ttu-id="01b15-2646">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="01b15-2646">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="01b15-2647">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="01b15-2647">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="01b15-2648">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-2648">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="01b15-2649">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="01b15-2649">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="01b15-2650">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="01b15-2650">Az.ApiManagement</span></span>
* <span data-ttu-id="01b15-2651">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="01b15-2651">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="01b15-2652">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="01b15-2652">Az.Automation</span></span>
* <span data-ttu-id="01b15-2653">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="01b15-2653">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="01b15-2654">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="01b15-2654">Added Update Management cmdlets</span></span>
* <span data-ttu-id="01b15-2655">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="01b15-2655">Added Source Control cmdlets</span></span>
* <span data-ttu-id="01b15-2656">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="01b15-2656">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="01b15-2657">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="01b15-2657">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="01b15-2658">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-2658">Az.Compute</span></span>
* <span data-ttu-id="01b15-2659">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="01b15-2659">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="01b15-2660">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="01b15-2660">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="01b15-2661">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="01b15-2661">Az.ContainerInstance</span></span>
* <span data-ttu-id="01b15-2662">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="01b15-2662">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="01b15-2663">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="01b15-2663">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="01b15-2664">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="01b15-2664">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="01b15-2665">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-2665">Az.Network</span></span>
* <span data-ttu-id="01b15-2666">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="01b15-2666">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="01b15-2667">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="01b15-2667">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="01b15-2668">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="01b15-2668">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="01b15-2669">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="01b15-2669">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="01b15-2670">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="01b15-2670">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="01b15-2671">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="01b15-2671">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="01b15-2672">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="01b15-2672">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="01b15-2673">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="01b15-2673">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="01b15-2674">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="01b15-2674">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="01b15-2675">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="01b15-2675">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="01b15-2676">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="01b15-2676">Az.Relay</span></span>
* <span data-ttu-id="01b15-2677">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="01b15-2677">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="01b15-2678">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-2678">Az.Resources</span></span>
* <span data-ttu-id="01b15-2679">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="01b15-2679">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="01b15-2680">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="01b15-2680">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="01b15-2681">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="01b15-2681">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="01b15-2682">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="01b15-2682">Az.ServiceFabric</span></span>
* <span data-ttu-id="01b15-2683">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="01b15-2683">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="01b15-2684">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-2684">Az.Sql</span></span>
* <span data-ttu-id="01b15-2685">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="01b15-2685">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="01b15-2686">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="01b15-2686">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="01b15-2687">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="01b15-2687">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="01b15-2688">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="01b15-2688">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="01b15-2689">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="01b15-2689">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="01b15-2690">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="01b15-2690">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="01b15-2691">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="01b15-2691">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="01b15-2692">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="01b15-2692">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="01b15-2693">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="01b15-2693">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="01b15-2694">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="01b15-2694">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="01b15-2695">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="01b15-2695">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="01b15-2696">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="01b15-2696">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="01b15-2697">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="01b15-2697">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="01b15-2698">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="01b15-2698">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="01b15-2699">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="01b15-2699">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="01b15-2700">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="01b15-2700">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="01b15-2701">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="01b15-2701">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="01b15-2702">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="01b15-2702">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="01b15-2703">Geral</span><span class="sxs-lookup"><span data-stu-id="01b15-2703">General</span></span>
* <span data-ttu-id="01b15-2704">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="01b15-2704">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="01b15-2705">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="01b15-2705">Az.Profile</span></span>
* <span data-ttu-id="01b15-2706">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="01b15-2706">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="01b15-2707">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="01b15-2707">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="01b15-2708">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="01b15-2708">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="01b15-2709">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="01b15-2709">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="01b15-2710">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="01b15-2710">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="01b15-2711">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="01b15-2711">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="01b15-2712">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="01b15-2712">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="01b15-2713">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="01b15-2713">Az.CognitiveServices</span></span>
* <span data-ttu-id="01b15-2714">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="01b15-2714">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-2715">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-2715">Az.Compute</span></span>
* <span data-ttu-id="01b15-2716">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="01b15-2716">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="01b15-2717">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="01b15-2717">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="01b15-2718">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="01b15-2718">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="01b15-2719">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="01b15-2719">Az.DataLakeStore</span></span>
* <span data-ttu-id="01b15-2720">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="01b15-2720">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="01b15-2721">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="01b15-2721">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="01b15-2722">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="01b15-2722">Az.Insights</span></span>
* <span data-ttu-id="01b15-2723">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="01b15-2723">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="01b15-2724">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="01b15-2724">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="01b15-2725">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="01b15-2725">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="01b15-2726">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="01b15-2726">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-2727">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-2727">Az.Network</span></span>
* <span data-ttu-id="01b15-2728">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="01b15-2728">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="01b15-2729">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="01b15-2729">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="01b15-2730">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="01b15-2730">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="01b15-2731">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="01b15-2731">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="01b15-2732">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="01b15-2732">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="01b15-2733">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="01b15-2733">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="01b15-2734">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="01b15-2734">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="01b15-2735">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="01b15-2735">Az.PolicyInsights</span></span>
* <span data-ttu-id="01b15-2736">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="01b15-2736">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-2737">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-2737">Az.Resources</span></span>
* <span data-ttu-id="01b15-2738">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="01b15-2738">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="01b15-2739">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="01b15-2739">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="01b15-2740">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="01b15-2740">Az.ServiceBus</span></span>
* <span data-ttu-id="01b15-2741">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="01b15-2741">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="01b15-2742">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="01b15-2742">Az.ServiceFabric</span></span>
* <span data-ttu-id="01b15-2743">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="01b15-2743">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="01b15-2744">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="01b15-2744">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="01b15-2745">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="01b15-2745">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="01b15-2746">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="01b15-2746">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="01b15-2747">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="01b15-2747">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="01b15-2748">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="01b15-2748">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="01b15-2749">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="01b15-2749">Az.Profile</span></span>
* <span data-ttu-id="01b15-2750">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="01b15-2750">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="01b15-2751">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="01b15-2751">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-2752">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-2752">Az.Compute</span></span>
* <span data-ttu-id="01b15-2753">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="01b15-2753">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="01b15-2754">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="01b15-2754">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="01b15-2755">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="01b15-2755">Az.DataLakeStore</span></span>
* <span data-ttu-id="01b15-2756">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="01b15-2756">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="01b15-2757">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-2757">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="01b15-2758">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="01b15-2758">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="01b15-2759">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="01b15-2759">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="01b15-2760">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="01b15-2760">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-2761">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-2761">Az.Network</span></span>
* <span data-ttu-id="01b15-2762">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="01b15-2762">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="01b15-2763">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="01b15-2763">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-2764">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-2764">Az.Resources</span></span>
* <span data-ttu-id="01b15-2765">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="01b15-2765">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="01b15-2766">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="01b15-2766">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="01b15-2767">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="01b15-2767">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="01b15-2768">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="01b15-2768">Azure.Storage</span></span>
* <span data-ttu-id="01b15-2769">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="01b15-2769">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="01b15-2770">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="01b15-2770">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="01b15-2771">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="01b15-2771">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="01b15-2772">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="01b15-2772">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="01b15-2773">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="01b15-2773">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="01b15-2774">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="01b15-2774">Az.CognitiveServices</span></span>
* <span data-ttu-id="01b15-2775">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="01b15-2775">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="01b15-2776">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="01b15-2776">Az.Compute</span></span>
* <span data-ttu-id="01b15-2777">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="01b15-2777">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="01b15-2778">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="01b15-2778">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="01b15-2779">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="01b15-2779">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="01b15-2780">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="01b15-2780">Az.DataFactoryV2</span></span>
* <span data-ttu-id="01b15-2781">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="01b15-2781">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="01b15-2782">Az.Network</span><span class="sxs-lookup"><span data-stu-id="01b15-2782">Az.Network</span></span>
* <span data-ttu-id="01b15-2783">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="01b15-2783">Added NetworkProfile functionality.</span></span> <span data-ttu-id="01b15-2784">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="01b15-2784">new cmdlets added</span></span>
    - <span data-ttu-id="01b15-2785">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="01b15-2785">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="01b15-2786">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="01b15-2786">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="01b15-2787">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="01b15-2787">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="01b15-2788">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="01b15-2788">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="01b15-2789">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-2789">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="01b15-2790">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-2790">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="01b15-2791">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="01b15-2791">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="01b15-2792">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="01b15-2792">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="01b15-2793">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="01b15-2793">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="01b15-2794">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="01b15-2794">Az.RedisCache</span></span>
* <span data-ttu-id="01b15-2795">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="01b15-2795">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="01b15-2796">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="01b15-2796">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="01b15-2797">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="01b15-2797">Az.Resources</span></span>
* <span data-ttu-id="01b15-2798">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="01b15-2798">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="01b15-2799">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="01b15-2799">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="01b15-2800">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="01b15-2800">Az.Sql</span></span>
* <span data-ttu-id="01b15-2801">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="01b15-2801">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="01b15-2802">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="01b15-2802">Az.Websites</span></span>
* <span data-ttu-id="01b15-2803">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="01b15-2803">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="01b15-2804">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="01b15-2804">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="01b15-2805">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="01b15-2805">0.2.0 - September 2018</span></span>
 <span data-ttu-id="01b15-2806">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="01b15-2806">Initial Release</span></span>
