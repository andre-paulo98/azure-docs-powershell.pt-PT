---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: 04e85c32b1af0bbdfb622973e0900724b8e3c8e3
ms.sourcegitcommit: 8b3126b5c79f453464d90669f0046ba86b7a3424
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/01/2020
ms.locfileid: "89244233"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="89801-103">Notas de versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="89801-103">Azure PowerShell release notes</span></span>

## <a name="461---august-2020"></a><span data-ttu-id="89801-104">4.6.1 - Agosto de 2020</span><span class="sxs-lookup"><span data-stu-id="89801-104">4.6.1 - August 2020</span></span>
#### <a name="azcompute"></a><span data-ttu-id="89801-105">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-105">Az.Compute</span></span>
* <span data-ttu-id="89801-106">Correção do parâmetro "-EncryptionAtHost" em "New-AzVm" para remover o valor predefinido de falso [#12776]</span><span class="sxs-lookup"><span data-stu-id="89801-106">Patched '-EncryptionAtHost' parameter in 'New-AzVm' to remove default value of false [#12776]</span></span>

## <a name="460---august-2020"></a><span data-ttu-id="89801-107">4.6.0 - Agosto de 2020</span><span class="sxs-lookup"><span data-stu-id="89801-107">4.6.0 - August 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="89801-108">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-108">Az.Accounts</span></span>
* <span data-ttu-id="89801-109">São carregados todos os ambientes de cloud pública quando o ponto final de deteção não devolve o AzureCloud predefinido ou outros ambientes públicos [#12633]</span><span class="sxs-lookup"><span data-stu-id="89801-109">Loaded all public cloud environments when discovery endpoint doesn't return default AzureCloud or other public environments [#12633]</span></span>
* <span data-ttu-id="89801-110">Exposição de SubscriptionPolicies em "Get-AzSubscription" [#12551]</span><span class="sxs-lookup"><span data-stu-id="89801-110">Exposed SubscriptionPolicies in 'Get-AzSubscription' [#12551]</span></span>

#### <a name="azautomation"></a><span data-ttu-id="89801-111">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="89801-111">Az.Automation</span></span>
* <span data-ttu-id="89801-112">Adição de parâmetros "-RunOn" a "Set-AzAutomationWebhook" para especificar um Grupo de Função de Trabalho Híbrida</span><span class="sxs-lookup"><span data-stu-id="89801-112">Added '-RunOn' parameters to 'Set-AzAutomationWebhook' to specify a Hybrid Worker Group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-113">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-113">Az.Compute</span></span>
* <span data-ttu-id="89801-114">Adição do parâmetro "-EncryptionAtHost" a "New-AzVm", "New-AzVmss", "New-AzVMConfig", "New-AzVmssConfig", "Update-AzVM" e "Update-AzVmss"</span><span class="sxs-lookup"><span data-stu-id="89801-114">Added '-EncryptionAtHost' parameter to 'New-AzVm', 'New-AzVmss', 'New-AzVMConfig', 'New-AzVmssConfig', 'Update-AzVM', and 'Update-AzVmss'</span></span>
* <span data-ttu-id="89801-115">Adição de "SecurityProfile" ao objeto de retorno "Get-AzVM" e "Get-AzVmss"</span><span class="sxs-lookup"><span data-stu-id="89801-115">Added 'SecurityProfile' to 'Get-AzVM' and 'Get-AzVmss' return object</span></span>
* <span data-ttu-id="89801-116">Adição do comutador "-InstanceView" como parâmetro opcional a "Get-AzHostGroup"</span><span class="sxs-lookup"><span data-stu-id="89801-116">Added '-InstanceView' switch as optional parameter to 'Get-AzHostGroup'</span></span>
* <span data-ttu-id="89801-117">Adição do novo cmdlet "Invoke-AzVmPatchAssessment"</span><span class="sxs-lookup"><span data-stu-id="89801-117">Added new cmdlet 'Invoke-AzVmPatchAssessment'</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="89801-118">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="89801-118">Az.DataFactory</span></span>
* <span data-ttu-id="89801-119">Adição das propriedades em falta à classe PSPipelineRun.</span><span class="sxs-lookup"><span data-stu-id="89801-119">Added missing properties to PSPipelineRun class.</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="89801-120">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="89801-120">Az.HDInsight</span></span>
* <span data-ttu-id="89801-121">É suportada a criação de clusters com encriptação na funcionalidade de anfitrião.</span><span class="sxs-lookup"><span data-stu-id="89801-121">Supported creating cluster with encryption at host feature.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="89801-122">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="89801-122">Az.KeyVault</span></span>
* <span data-ttu-id="89801-123">Adição de mensagens de aviso para planear a desativação da eliminação recuperável</span><span class="sxs-lookup"><span data-stu-id="89801-123">Added warning messages for planning to disable soft delete</span></span>
* <span data-ttu-id="89801-124">Adição de mensagens de aviso para planear a remoção do atributo SecretValueText</span><span class="sxs-lookup"><span data-stu-id="89801-124">Added warning messages for planning to remove attribute SecretValueText</span></span>

#### <a name="azmaintenance"></a><span data-ttu-id="89801-125">Az.Maintenance</span><span class="sxs-lookup"><span data-stu-id="89801-125">Az.Maintenance</span></span>
* <span data-ttu-id="89801-126">Adição de campos relacionados com agendamento opcionais a "New-AzMaintenanceConfiguration"</span><span class="sxs-lookup"><span data-stu-id="89801-126">Added optional schedule related fields to 'New-AzMaintenanceConfiguration'</span></span>
* <span data-ttu-id="89801-127">Adição do novo cmdlet para "Get-AzMaintenancePublicConfiguration"</span><span class="sxs-lookup"><span data-stu-id="89801-127">Added new cmdlet for 'Get-AzMaintenancePublicConfiguration'</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="89801-128">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="89801-128">Az.ManagedServices</span></span>
* <span data-ttu-id="89801-129">Adição de avisos de alteração interruptiva nos cmdlets de atribuição e definição de serviços geridos</span><span class="sxs-lookup"><span data-stu-id="89801-129">Added breaking change warnings on cmdlets of managed services assignment and definition</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="89801-130">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="89801-130">Az.Monitor</span></span>
* <span data-ttu-id="89801-131">Expansão do parâmetro definido em "Set-AzDiagnosticSetting" para a separação da ativação de Registos e Métricas [#12482]</span><span class="sxs-lookup"><span data-stu-id="89801-131">Extended the parameter set in 'Set-AzDiagnosticSetting' for separation of Logs and Metrics enablement [#12482]</span></span>
* <span data-ttu-id="89801-132">Correção do erro de "Add-AzMetricAlertRuleV2" ao obter o alerta de métrica do pipeline</span><span class="sxs-lookup"><span data-stu-id="89801-132">Fixed bug for 'Add-AzMetricAlertRuleV2' when getting metric alert from pipeline</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-133">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-133">Az.Resources</span></span>
* <span data-ttu-id="89801-134">Atualização da resposta "Get-AzPolicyAlias" no sentido de incluir informações que indicam se o alias pode ser modificado pelo Azure Policy.</span><span class="sxs-lookup"><span data-stu-id="89801-134">Updated 'Get-AzPolicyAlias' response to include information indicating whether the alias is modifiable by Azure Policy.</span></span>
* <span data-ttu-id="89801-135">Criação do novo cmdlet "Set-AzRoleAssignment"</span><span class="sxs-lookup"><span data-stu-id="89801-135">Created new cmdlet 'Set-AzRoleAssignment'</span></span>
* <span data-ttu-id="89801-136">Adição de "Get-AzDeploymentManagementGroupWhatIfResult" para obter os resultados de Hipóteses do modelo do ARM no âmbito do Grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="89801-136">Added 'Get-AzDeploymentManagementGroupWhatIfResult' for getting ARM template What-If results at management Group scope</span></span>
* <span data-ttu-id="89801-137">Adição do novo cmdlet "Get-AzTenantWhatIfResult" para obter os resultados de Hipóteses do modelo do ARM no âmbito do inquilino</span><span class="sxs-lookup"><span data-stu-id="89801-137">Added 'Get-AzTenantWhatIfResult' new cmdlet for getting ARM template What-If results at tenant scope</span></span>
* <span data-ttu-id="89801-138">Substituição de "-WhatIf" e "-Confirm" por "New-AzManagementGroupDeployment" e "New-AzTenantDeployment" no sentido de utilizar os resultados de Hipóteses do modelo do ARM</span><span class="sxs-lookup"><span data-stu-id="89801-138">Overrode '-WhatIf' and '-Confirm' for 'New-AzManagementGroupDeployment' and 'New-AzTenantDeployment' to use ARM template What-If results</span></span>
* <span data-ttu-id="89801-139">Correção dos comportamentos de "-WhatIf" e "-Confirm" para os novos cmdlets de implementação para que estejam em conformidade com Falso e</span><span class="sxs-lookup"><span data-stu-id="89801-139">Fixed the behaviors of '-WhatIf' and '-Confirm' for new deployment cmdlets so they comply with False and</span></span> 
* <span data-ttu-id="89801-140">Correção do erro de serialização de "-TemplateObject" e "TemplateParameterObject" [#1528] [#6292]</span><span class="sxs-lookup"><span data-stu-id="89801-140">Fixed serialization error for '-TemplateObject' and 'TemplateParameterObject' [#1528] [#6292]</span></span>
* <span data-ttu-id="89801-141">Adição do atributo de alteração interruptiva a "Get-AzResourceGroupDeploymentOperation" para a próxima alteração do tipo de saída</span><span class="sxs-lookup"><span data-stu-id="89801-141">Added breaking change attribute to 'Get-AzResourceGroupDeploymentOperation' for the upcoming output type change</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="89801-142">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="89801-142">Az.SignalR</span></span>
* <span data-ttu-id="89801-143">Correção dos erros dos ficheiros de ajuda "Restart-AzSignalR" e "Update-AzSignalR"</span><span class="sxs-lookup"><span data-stu-id="89801-143">Fixed 'Restart-AzSignalR' and 'Update-AzSignalR' help files errors</span></span>
* <span data-ttu-id="89801-144">Adição dos cmdlets "Update-AzSignalRNetworkAcl" e "Set-AzSignalRUpstream"</span><span class="sxs-lookup"><span data-stu-id="89801-144">Added cmdlets 'Update-AzSignalRNetworkAcl', 'Set-AzSignalRUpstream'</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-145">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-145">Az.Storage</span></span>
* <span data-ttu-id="89801-146">É suportada a aceleração da consulta de blobs</span><span class="sxs-lookup"><span data-stu-id="89801-146">Supported blob query acceleration</span></span>
    -  <span data-ttu-id="89801-147">"Get-AzStorageBlobQueryResult"</span><span class="sxs-lookup"><span data-stu-id="89801-147">'Get-AzStorageBlobQueryResult'</span></span>
    -  <span data-ttu-id="89801-148">"New-AzStorageBlobQueryConfig"</span><span class="sxs-lookup"><span data-stu-id="89801-148">'New-AzStorageBlobQueryConfig'</span></span>
* <span data-ttu-id="89801-149">Atualização do ficheiro de ajuda, com a adição de mais descrições e a correção de erros de digitação</span><span class="sxs-lookup"><span data-stu-id="89801-149">Updated help file, added more description, and fixed typo</span></span>
    -  <span data-ttu-id="89801-150">"Start-AzStorageBlobCopy"</span><span class="sxs-lookup"><span data-stu-id="89801-150">'Start-AzStorageBlobCopy'</span></span>
    -  <span data-ttu-id="89801-151">"Get-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="89801-151">'Get-AzDataLakeGen2Item'</span></span>
* <span data-ttu-id="89801-152">Correção da falha de transferência de blobs quando o subdiretório relacionado não existe [#12592]</span><span class="sxs-lookup"><span data-stu-id="89801-152">Fixed download blob fail when related sub directory not exist [#12592]</span></span>
    -  <span data-ttu-id="89801-153">"Get-AzStorageBlobContent"</span><span class="sxs-lookup"><span data-stu-id="89801-153">'Get-AzStorageBlobContent'</span></span>
* <span data-ttu-id="89801-154">É suportada a Política de Replicação Definir/Obter/Remover Objeto nas Contas de armazenamento</span><span class="sxs-lookup"><span data-stu-id="89801-154">Supported Set/Get/Remove Object Replication Policy on Storage accounts</span></span>
    - <span data-ttu-id="89801-155">"New-AzStorageObjectReplicationPolicyRule"</span><span class="sxs-lookup"><span data-stu-id="89801-155">'New-AzStorageObjectReplicationPolicyRule'</span></span>
    - <span data-ttu-id="89801-156">"Set-AzStorageObjectReplicationPolicy"</span><span class="sxs-lookup"><span data-stu-id="89801-156">'Set-AzStorageObjectReplicationPolicy'</span></span>
    - <span data-ttu-id="89801-157">"Get-AzStorageObjectReplicationPolicy"</span><span class="sxs-lookup"><span data-stu-id="89801-157">'Get-AzStorageObjectReplicationPolicy'</span></span>
    - <span data-ttu-id="89801-158">"Remove-AzStorageObjectReplicationPolicy"</span><span class="sxs-lookup"><span data-stu-id="89801-158">'Remove-AzStorageObjectReplicationPolicy'</span></span>
* <span data-ttu-id="89801-159">Suporte para ativar/desativar o ChangeFeed no Serviço Blob de uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="89801-159">Supported enable/disable ChangeFeed on Blob Service of a Storage account</span></span>
    - <span data-ttu-id="89801-160">"Update-AzStorageBlobServiceProperty"</span><span class="sxs-lookup"><span data-stu-id="89801-160">'Update-AzStorageBlobServiceProperty'</span></span>

## <a name="450---august-2020"></a><span data-ttu-id="89801-161">4.5.0 - Agosto de 2020</span><span class="sxs-lookup"><span data-stu-id="89801-161">4.5.0 - August 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="89801-162">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-162">Az.Accounts</span></span>
* <span data-ttu-id="89801-163">"Connect-AzAccount" atualizado para aceitar o parâmetro "MaxContextPopulation" [#9865]</span><span class="sxs-lookup"><span data-stu-id="89801-163">Updated 'Connect-AzAccount' to accept parameter 'MaxContextPopulation' [#9865]</span></span>
* <span data-ttu-id="89801-164">Versão de SubscriptionClient atualizada para a de 2019-06-01 e apresentação de domínios de inquilino [#9838]</span><span class="sxs-lookup"><span data-stu-id="89801-164">Updated SubscriptionClient version to 2019-06-01 and display tenant domains [#9838]</span></span>
* <span data-ttu-id="89801-165">Inquilino principal suportado e informações do inquilino managedBy da subscrição</span><span class="sxs-lookup"><span data-stu-id="89801-165">Supported home tenant and managedBy tenant information of subscription</span></span>
* <span data-ttu-id="89801-166">Nome do módulo corrigido, informações da versão nos dados telemétricos</span><span class="sxs-lookup"><span data-stu-id="89801-166">Corrected module name, version info in telemetry data</span></span>
* <span data-ttu-id="89801-167">SqlDatabaseDnsSuffix e ServiceManagementUrl ajustados se o ponto final dos metadados do ambiente devolverem valores incompatíveis</span><span class="sxs-lookup"><span data-stu-id="89801-167">Adjusted SqlDatabaseDnsSuffix and ServiceManagementUrl if environment metadata endpoint returns incompatible value</span></span>

#### <a name="azaks"></a><span data-ttu-id="89801-168">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="89801-168">Az.Aks</span></span>
* <span data-ttu-id="89801-169">"ClientIdAndSecret" removido para "ServicePrincipalIdAndSecret" e "ClientIdAndSecret" definido como um alias [#12381].</span><span class="sxs-lookup"><span data-stu-id="89801-169">Removed 'ClientIdAndSecret' to 'ServicePrincipalIdAndSecret' and set 'ClientIdAndSecret' as an alias [#12381].</span></span>
* <span data-ttu-id="89801-170">"Get-AzAks"/"New-AzAks"/"Remove-AzAks"/"Set-AzAks" removidos para "Get-AzAksCluster"/"New-AzAksCluster"/"Remove-AzAksCluster"/"Set-AzAksCluster" e definição dos valores originais como alias [#12373].</span><span class="sxs-lookup"><span data-stu-id="89801-170">Removed 'Get-AzAks'/'New-AzAks'/'Remove-AzAks'/'Set-AzAks' to 'Get-AzAksCluster'/'New-AzAksCluster'/'Remove-AzAksCluster'/'Set-AzAksCluster' and set the original ones as alias [#12373].</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="89801-171">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="89801-171">Az.ApiManagement</span></span>
* <span data-ttu-id="89801-172">Novo cmdlet "Add-AzApiManagementApiToGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="89801-172">Added new 'Add-AzApiManagementApiToGateway' cmdlet.</span></span>
* <span data-ttu-id="89801-173">Novo cmdlet "Get-AzApiManagementGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="89801-173">Added new 'Get-AzApiManagementGateway' cmdlet.</span></span>
* <span data-ttu-id="89801-174">Novo cmdlet "Get-AzApiManagementGatewayHostnameConfiguration" adicionado.</span><span class="sxs-lookup"><span data-stu-id="89801-174">Added new 'Get-AzApiManagementGatewayHostnameConfiguration' cmdlet.</span></span>
* <span data-ttu-id="89801-175">Novo cmdlet "Get-AzApiManagementGatewayKey" adicionado.</span><span class="sxs-lookup"><span data-stu-id="89801-175">Added new 'Get-AzApiManagementGatewayKey' cmdlet.</span></span>
* <span data-ttu-id="89801-176">Novo cmdlet "New-AzApiManagementGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="89801-176">Added new 'New-AzApiManagementGateway' cmdlet.</span></span>
* <span data-ttu-id="89801-177">Novo cmdlet "New-AzApiManagementGatewayHostnameConfiguration" adicionado.</span><span class="sxs-lookup"><span data-stu-id="89801-177">Added new 'New-AzApiManagementGatewayHostnameConfiguration' cmdlet.</span></span>
* <span data-ttu-id="89801-178">Novo cmdlet "New-AzApiManagementResourceLocationObject" adicionado.</span><span class="sxs-lookup"><span data-stu-id="89801-178">Added new 'New-AzApiManagementResourceLocationObject' cmdlet.</span></span>
* <span data-ttu-id="89801-179">Novo cmdlet "Remove-AzApiManagementApiFromGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="89801-179">Added new 'Remove-AzApiManagementApiFromGateway' cmdlet.</span></span>
* <span data-ttu-id="89801-180">Novo cmdlet "Remove-AzApiManagementGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="89801-180">Added new 'Remove-AzApiManagementGateway' cmdlet.</span></span>
* <span data-ttu-id="89801-181">Novo cmdlet "Remove-AzApiManagementGatewayHostnameConfiguration" adicionado.</span><span class="sxs-lookup"><span data-stu-id="89801-181">Added new 'Remove-AzApiManagementGatewayHostnameConfiguration' cmdlet.</span></span>
* <span data-ttu-id="89801-182">Novo cmdlet "Update-AzApiManagementGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="89801-182">Added new 'Update-AzApiManagementGateway' cmdlet.</span></span>
* <span data-ttu-id="89801-183">Foi adicionado um novo parâmetro [-GatewayId] opcional ao cmdlet "Get-AzApiManagementApi".</span><span class="sxs-lookup"><span data-stu-id="89801-183">Added new optional [-GatewayId] parameter to the 'Get-AzApiManagementApi' cmdlet.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="89801-184">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="89801-184">Az.CognitiveServices</span></span>
* <span data-ttu-id="89801-185">Utilizado "Deny" especificamente como ação NetworkRules predefinida.</span><span class="sxs-lookup"><span data-stu-id="89801-185">Used 'Deny' specifically as NetworkRules default action.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="89801-186">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="89801-186">Az.FrontDoor</span></span>
* <span data-ttu-id="89801-187">Foi resolvido um problema em que é gerada uma exceção quando Enum.Parse tenta limitar um valor nulo a um valor de enumeração Enabled ou Disabled [#12344]</span><span class="sxs-lookup"><span data-stu-id="89801-187">Fixed an issue where an exception is being thrown when Enum.Parse tries to coerce a null value to an Enabled or Disabled enum values [#12344]</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="89801-188">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="89801-188">Az.HDInsight</span></span>
* <span data-ttu-id="89801-189">É suportada a criação de clusters com encriptação na funcionalidade de trânsito.</span><span class="sxs-lookup"><span data-stu-id="89801-189">Supported creating cluster with encryption in transit feature.</span></span>
    - <span data-ttu-id="89801-190">Foi adicionado o novo parâmetro "EncryptionInTransit" ao cmdlet "New-AzHDInsightCluster"</span><span class="sxs-lookup"><span data-stu-id="89801-190">Add new parameter 'EncryptionInTransit' to the cmdlet 'New-AzHDInsightCluster'</span></span>
    - <span data-ttu-id="89801-191">Foi adicionado o novo parâmetro "EncryptionInTransit" ao cmdlet "New-AzHDInsightClusterConfig"</span><span class="sxs-lookup"><span data-stu-id="89801-191">Add new parameter 'EncryptionInTransit' to the cmdlet 'New-AzHDInsightClusterConfig'</span></span>
* <span data-ttu-id="89801-192">É suportada a criação de clusters com a funcionalidade de ligação privada:</span><span class="sxs-lookup"><span data-stu-id="89801-192">Supported creating cluster with private link feature:</span></span>
    - <span data-ttu-id="89801-193">Novos parâmetros "PublicNetworkAccessType" e "OutboundPublicNetworkAccessType" adicionados ao cmdlet "New-AzHDInsightCluster"</span><span class="sxs-lookup"><span data-stu-id="89801-193">Add new parameter 'PublicNetworkAccessType' and 'OutboundPublicNetworkAccessType' to the cmdlet 'New-AzHDInsightCluster'</span></span>
    - <span data-ttu-id="89801-194">Novos parâmetros "PublicNetworkAccessType" e "OutboundPublicNetworkAccessType" adicionados ao cmdlet "New-AzHDInsightClusterConfig"</span><span class="sxs-lookup"><span data-stu-id="89801-194">Add new parameter 'PublicNetworkAccessType' and 'OutboundPublicNetworkAccessType' to the cmdlet 'New-AzHDInsightClusterConfig'</span></span>
* <span data-ttu-id="89801-195">Informações de rede virtual devolvidas ao chamar "New-AzHDInsightCluster" ou "Get-AzHDInsightCluster"</span><span class="sxs-lookup"><span data-stu-id="89801-195">Returned virtual network information when calling 'New-AzHDInsightCluster' or 'Get-AzHDInsightCluster'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-196">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-196">Az.Network</span></span>
* <span data-ttu-id="89801-197">Adição de suporte para o parâmetro AddressPrefixType a "Remove-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="89801-197">Added support for AddressPrefixType parameter to 'Remove-AzExpressRouteCircuitConnectionConfig'</span></span>
* <span data-ttu-id="89801-198">Alterações não interruptivas adicionadas: Funcionalidade PeerAddressType para Peering Privado em "Remove-AzExpressRouteCircutPeeringConfig".</span><span class="sxs-lookup"><span data-stu-id="89801-198">Added non-breaking changes: PeerAddressType functionality for Private Peering in 'Remove-AzExpressRouteCircutPeeringConfig'.</span></span>
* <span data-ttu-id="89801-199">Código alterado para ignorar caso dos parâmetros AddressPrefixType e PeerAddressType.</span><span class="sxs-lookup"><span data-stu-id="89801-199">Code changed to ignore case for AddressPrefixType and PeerAddressType parameter.</span></span>
* <span data-ttu-id="89801-200">Foi modificada a mensagem de aviso de "New-AzLoadBalancerFrontendIpConfig", "New-AzPublicIpAddress" e "New-AzPublicIpPrefix".</span><span class="sxs-lookup"><span data-stu-id="89801-200">Modified the warning message for 'New-AzLoadBalancerFrontendIpConfig', 'New-AzPublicIpAddress' and 'New-AzPublicIpPrefix'.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="89801-201">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="89801-201">Az.OperationalInsights</span></span>
* <span data-ttu-id="89801-202">Opção "-ForceDelete" adicionada para "Remove-AzOperationalInsightsworkspace"</span><span class="sxs-lookup"><span data-stu-id="89801-202">Added '-ForceDelete' option for 'Remove-AzOperationalInsightsworkspace'</span></span>
* <span data-ttu-id="89801-203">Novo cmdlet "Get-AzOperationalInsightsDeletedWorkspace" adicionado</span><span class="sxs-lookup"><span data-stu-id="89801-203">Added new cmdlet 'Get-AzOperationalInsightsDeletedWorkspace'</span></span>
* <span data-ttu-id="89801-204">Novo cmdlet "Restore-AzOperationalInsightsWorkspace" adicionado</span><span class="sxs-lookup"><span data-stu-id="89801-204">Added new cmdlet 'Restore-AzOperationalInsightsWorkspace'</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-205">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-205">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-206">Experiência de deteção de contentores/itens do Azure Backup melhorada.</span><span class="sxs-lookup"><span data-stu-id="89801-206">Improved the Azure Backup container/item discovery experience.</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-207">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-207">Az.Resources</span></span>
* <span data-ttu-id="89801-208">Propriedades "Condition", "ConditionVersion" e "Description" adicionadas a "New-AzRoleAssignment"</span><span class="sxs-lookup"><span data-stu-id="89801-208">Added properties 'Condition', 'ConditionVersion' and 'Description' to 'New-AzRoleAssignment'</span></span>
    - <span data-ttu-id="89801-209">Isto incluiu todas as alterações relevantes aos modelos de dados</span><span class="sxs-lookup"><span data-stu-id="89801-209">This included all the relevant changes to the data models</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-210">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-210">Az.Sql</span></span>
* <span data-ttu-id="89801-211">Foi corrigido o potencial erro de nome do servidor não sensível a maiúsculas e minúsculas em "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="89801-211">Fixed potential server name case insensitive error in 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="89801-212">Foi corrigido o erro em que era devolvido um nome de base de dados incorreto numa base de dados existente em "New-AzSqlDatabaseSecondary"</span><span class="sxs-lookup"><span data-stu-id="89801-212">Fixed wrong database name returned on existing database error in 'New-AzSqlDatabaseSecondary'</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-213">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-213">Az.Storage</span></span>
* <span data-ttu-id="89801-214">Criação de tokens de SAS de contentores/blobs suportada com nova permissão x,t</span><span class="sxs-lookup"><span data-stu-id="89801-214">Supported create container/blob Sas token with new permission x,t</span></span>
    -  <span data-ttu-id="89801-215">"New-AzStorageBlobSASToken"</span><span class="sxs-lookup"><span data-stu-id="89801-215">'New-AzStorageBlobSASToken'</span></span>
    -  <span data-ttu-id="89801-216">"New-AzStorageContainerSASToken"</span><span class="sxs-lookup"><span data-stu-id="89801-216">'New-AzStorageContainerSASToken'</span></span>
* <span data-ttu-id="89801-217">Criação de tokens de SAS de contas suportada com nova permissão x,t,f</span><span class="sxs-lookup"><span data-stu-id="89801-217">Supported create account Sas token with new permission x,t,f</span></span>
    -  <span data-ttu-id="89801-218">"New-AzStorageAccountSASToken"</span><span class="sxs-lookup"><span data-stu-id="89801-218">'New-AzStorageAccountSASToken'</span></span>
* <span data-ttu-id="89801-219">Obtenção da utilização de partilha de ficheiros única suportada</span><span class="sxs-lookup"><span data-stu-id="89801-219">Supported get single file share usage</span></span>
    - <span data-ttu-id="89801-220">"Get-AzRmStorageShare"</span><span class="sxs-lookup"><span data-stu-id="89801-220">'Get-AzRmStorageShare'</span></span>

## <a name="440---july-2020"></a><span data-ttu-id="89801-221">4.4.0 - Julho de 2020</span><span class="sxs-lookup"><span data-stu-id="89801-221">4.4.0 - July 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="89801-222">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-222">Az.Accounts</span></span>
* <span data-ttu-id="89801-223">Adição do novo cmdlet "Invoke-AzRestMethod"</span><span class="sxs-lookup"><span data-stu-id="89801-223">Added new cmdlet 'Invoke-AzRestMethod'</span></span>
* <span data-ttu-id="89801-224">Correção de um problema que pode causar erros de autenticação em cenários de vários processos, tais como executar vários cmdlets do Azure PowerShell utilizando "Start-Job" [#9448]</span><span class="sxs-lookup"><span data-stu-id="89801-224">Fixed an issue that may cause authentication errors in multi-process scenarios such as running multiple Azure PowerShell cmdlets using 'Start-Job' [#9448]</span></span>

#### <a name="azaks"></a><span data-ttu-id="89801-225">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="89801-225">Az.Aks</span></span>
* <span data-ttu-id="89801-226">Correção do erro "Get-AzAks" uma vez que não recebe todos os clusters [#12296]</span><span class="sxs-lookup"><span data-stu-id="89801-226">Fixed bug 'Get-AzAks' doesn't get all clusters [#12296]</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="89801-227">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="89801-227">Az.AnalysisServices</span></span>
* <span data-ttu-id="89801-228">Remoção da referência do projeto para Autenticação</span><span class="sxs-lookup"><span data-stu-id="89801-228">Removed project reference to Authentication</span></span>

#### <a name="azautomation"></a><span data-ttu-id="89801-229">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="89801-229">Az.Automation</span></span>
* <span data-ttu-id="89801-230">Correção do problema em que a cadeia com chars de fuga não pode ser convertida num objeto json.</span><span class="sxs-lookup"><span data-stu-id="89801-230">Fixed the issue that string with escape chars cannot be converted into json object.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-231">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-231">Az.Compute</span></span>
* <span data-ttu-id="89801-232">Adição do aviso ao utilizar "New-AzVmss" sem a versão de imagem "mais recente"</span><span class="sxs-lookup"><span data-stu-id="89801-232">Added warning when using 'New-AzVmss' without 'latest' image version</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="89801-233">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="89801-233">Az.DataFactory</span></span>
* <span data-ttu-id="89801-234">Adição de parâmetros globais ao Data Factory.</span><span class="sxs-lookup"><span data-stu-id="89801-234">Added global parameters to Data Factory.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="89801-235">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="89801-235">Az.EventGrid</span></span>
* <span data-ttu-id="89801-236">Atualização para utilizar a versão de API 2020-06-01.</span><span class="sxs-lookup"><span data-stu-id="89801-236">Updated to use the 2020-06-01 API version.</span></span>
* <span data-ttu-id="89801-237">Novas funcionalidades adicionadas:</span><span class="sxs-lookup"><span data-stu-id="89801-237">Added new features:</span></span>
    - <span data-ttu-id="89801-238">Mapeamento de entrada</span><span class="sxs-lookup"><span data-stu-id="89801-238">Input mapping</span></span>
    - <span data-ttu-id="89801-239">Esquema de Entrega de Eventos</span><span class="sxs-lookup"><span data-stu-id="89801-239">Event Delivery Schema</span></span>
    - <span data-ttu-id="89801-240">Ligação Privada</span><span class="sxs-lookup"><span data-stu-id="89801-240">Private Link</span></span>
    - <span data-ttu-id="89801-241">Esquema de Eventos na Cloud V10</span><span class="sxs-lookup"><span data-stu-id="89801-241">Cloud Event V10 Schema</span></span>
    - <span data-ttu-id="89801-242">Tópico do Service Bus como Destino</span><span class="sxs-lookup"><span data-stu-id="89801-242">Service Bus Topic As Destination</span></span>
    - <span data-ttu-id="89801-243">Função do Azure como Destino</span><span class="sxs-lookup"><span data-stu-id="89801-243">Azure Function As Destination</span></span>
    - <span data-ttu-id="89801-244">Criação de batches do WebHook</span><span class="sxs-lookup"><span data-stu-id="89801-244">WebHook Batching</span></span>
    - <span data-ttu-id="89801-245">Webhook seguro (suporte de AAD)</span><span class="sxs-lookup"><span data-stu-id="89801-245">Secure webhook (AAD support)</span></span>
    - <span data-ttu-id="89801-246">IpFiltering</span><span class="sxs-lookup"><span data-stu-id="89801-246">IpFiltering</span></span>
* <span data-ttu-id="89801-247">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="89801-247">Updated cmdlets:</span></span>
    - <span data-ttu-id="89801-248">"New-AzEventGridSubscription"/"Update-AzEventGridSubscription":</span><span class="sxs-lookup"><span data-stu-id="89801-248">'New-AzEventGridSubscription'/'Update-AzEventGridSubscription':</span></span>
        - <span data-ttu-id="89801-249">Adicionar novos parâmetros opcionais para suportar a criação de batches do webhook.</span><span class="sxs-lookup"><span data-stu-id="89801-249">Add new optional parameters to support webhook batching.</span></span>
        - <span data-ttu-id="89801-250">Adicionar novos parâmetros opcionais para suportar o webhook seguro através do AAD.</span><span class="sxs-lookup"><span data-stu-id="89801-250">Add new optional parameters to support secured webhook using AAD.</span></span>
        - <span data-ttu-id="89801-251">Adicionar uma nova enumeração para o parâmetro EndpointType para suportar a função do Azure e o tópico do Service Bus enquanto novos destinos.</span><span class="sxs-lookup"><span data-stu-id="89801-251">Add new enum for EndpointType parameter to support azure function and service bus topic as new destinations.</span></span>
        - <span data-ttu-id="89801-252">Adicionar novo parâmetro opcional para o esquema de entrega.</span><span class="sxs-lookup"><span data-stu-id="89801-252">Add new optional parameter for delivery schema.</span></span>
    - <span data-ttu-id="89801-253">"New-AzEventGridTopic"/"Update-AzEventGridTopic" e "New-AzEventGridDomain"/"Update-AzEventGridDomain":</span><span class="sxs-lookup"><span data-stu-id="89801-253">'New-AzEventGridTopic'/'Update-AzEventGridTopic' and 'New-AzEventGridDomain'/'Update-AzEventGridDomain':</span></span>
        - <span data-ttu-id="89801-254">Adicionar novos parâmetros opcionais para suportar IpFiltering.</span><span class="sxs-lookup"><span data-stu-id="89801-254">Add new optional parameters to support IpFiltering.</span></span>
    - <span data-ttu-id="89801-255">"New-AzEventGridTopic"/"New-AzEventGridDomain":</span><span class="sxs-lookup"><span data-stu-id="89801-255">'New-AzEventGridTopic'/'New-AzEventGridDomain':</span></span>
        - <span data-ttu-id="89801-256">Adicionar novos parâmetros opcionais para suportar o Mapeamento de entrada.</span><span class="sxs-lookup"><span data-stu-id="89801-256">Add new optional parameters to support Input mapping.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="89801-257">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="89801-257">Az.FrontDoor</span></span>
* <span data-ttu-id="89801-258">Módulo atualizado para utilizar a API 2020-05-01</span><span class="sxs-lookup"><span data-stu-id="89801-258">Updated module to use API 2020-05-01</span></span>
* <span data-ttu-id="89801-259">Adição de suporte do Private Link para recursos de Armazenamento, Cofre de chaves e Serviço de Aplicações Web</span><span class="sxs-lookup"><span data-stu-id="89801-259">Added Private link support for Storage, Keyvault and Web App Service resources</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="89801-260">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="89801-260">Az.HDInsight</span></span>
* <span data-ttu-id="89801-261">Suporte para a criação de cluster com armazenamento ADLSGen1/2 em clouds nacionais.</span><span class="sxs-lookup"><span data-stu-id="89801-261">Supported creating cluster with ADLSGen1/2 storage in national clouds.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="89801-262">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="89801-262">Az.Monitor</span></span>
* <span data-ttu-id="89801-263">Correção do erro em "Get-AzDiagnosticSetting" quando as métricas ou registos são nulos [#12272]</span><span class="sxs-lookup"><span data-stu-id="89801-263">Fixed bug for 'Get-AzDiagnosticSetting' when metrics or logs are null [#12272]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-264">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-264">Az.Network</span></span>
* <span data-ttu-id="89801-265">Correção da troca de parâmetros na ligação VWan HubVnet</span><span class="sxs-lookup"><span data-stu-id="89801-265">Fixed parameters swap in VWan HubVnet connection</span></span>
* <span data-ttu-id="89801-266">Adição de novos cmdlets para Sites de Aplicações Virtuais da Rede Azure</span><span class="sxs-lookup"><span data-stu-id="89801-266">Added new cmdlets for Azure Network Virtual Appliance Sites</span></span>
    - <span data-ttu-id="89801-267">"Get-AzVirtualApplianceSite"</span><span class="sxs-lookup"><span data-stu-id="89801-267">'Get-AzVirtualApplianceSite'</span></span>
    - <span data-ttu-id="89801-268">"New-AzVirtualApplianceSite"</span><span class="sxs-lookup"><span data-stu-id="89801-268">'New-AzVirtualApplianceSite'</span></span>
    - <span data-ttu-id="89801-269">"Remove-AzVirtualApplianceSite"</span><span class="sxs-lookup"><span data-stu-id="89801-269">'Remove-AzVirtualApplianceSite'</span></span>
    - <span data-ttu-id="89801-270">"Update-AzVirtualApplianceSite"</span><span class="sxs-lookup"><span data-stu-id="89801-270">'Update-AzVirtualApplianceSite'</span></span>
    - <span data-ttu-id="89801-271">"New-AzOffice365PolicyProperty"</span><span class="sxs-lookup"><span data-stu-id="89801-271">'New-AzOffice365PolicyProperty'</span></span>
* <span data-ttu-id="89801-272">Adição de novos cmdlets para Aplicações Virtuais da Rede Azure</span><span class="sxs-lookup"><span data-stu-id="89801-272">Added new cmdlets for Azure Network Virtual Appliance</span></span>
    - <span data-ttu-id="89801-273">"Get-AzNetworkVirtualAppliance"</span><span class="sxs-lookup"><span data-stu-id="89801-273">'Get-AzNetworkVirtualAppliance'</span></span>
    - <span data-ttu-id="89801-274">"New-AzNetworkVirtualAppliance"</span><span class="sxs-lookup"><span data-stu-id="89801-274">'New-AzNetworkVirtualAppliance'</span></span>
    - <span data-ttu-id="89801-275">"Remove-AzNetworkVirtualAppliance"</span><span class="sxs-lookup"><span data-stu-id="89801-275">'Remove-AzNetworkVirtualAppliance'</span></span>
    - <span data-ttu-id="89801-276">"Update-AzNetworkVirtualAppliance"</span><span class="sxs-lookup"><span data-stu-id="89801-276">'Update-AzNetworkVirtualAppliance'</span></span>
    - <span data-ttu-id="89801-277">"Get-AzNetworkVirtualApplianceSku"</span><span class="sxs-lookup"><span data-stu-id="89801-277">'Get-AzNetworkVirtualApplianceSku'</span></span>
    - <span data-ttu-id="89801-278">"New-AzVirtualApplianceSkuProperty"</span><span class="sxs-lookup"><span data-stu-id="89801-278">'New-AzVirtualApplianceSkuProperty'</span></span>
* <span data-ttu-id="89801-279">Gateway de Aplicação integrado para Cmdlets Comuns do Private Link</span><span class="sxs-lookup"><span data-stu-id="89801-279">Onboarded Application Gateway to Private Link Common Cmdlets</span></span>
* <span data-ttu-id="89801-280">StorageSync integrado para Cmdlets Comuns do Private Link</span><span class="sxs-lookup"><span data-stu-id="89801-280">Onboarded StorageSync to Private Link Common Cmdlets</span></span>
* <span data-ttu-id="89801-281">SignalR integrado para Cmdlets Comuns do Private Link</span><span class="sxs-lookup"><span data-stu-id="89801-281">Onboarded SignalR to Private Link Common Cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-282">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-282">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-283">Remoção da referência do projeto para Autenticação</span><span class="sxs-lookup"><span data-stu-id="89801-283">Removed project reference to Authentication</span></span>
* <span data-ttu-id="89801-284">Os cmdlets afinados do Azure Backup ajudam o texto a ser mais preciso.</span><span class="sxs-lookup"><span data-stu-id="89801-284">Azure Backup tuned cmdlets help text to be more accurate.</span></span>
* <span data-ttu-id="89801-285">O Azure Backup adicionou suporte para obter tarefas de agentes MAB através do cmdlet "Get-AzRecoveryServicesBackupJob".</span><span class="sxs-lookup"><span data-stu-id="89801-285">Azure Backup added support for fetching MAB agent jobs using 'Get-AzRecoveryServicesBackupJob' cmdlet.</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-286">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-286">Az.Resources</span></span>
* <span data-ttu-id="89801-287">Atualização de "Save-AzResourceGroupDeploymentTemplate" para utilizar o SDK.</span><span class="sxs-lookup"><span data-stu-id="89801-287">Updated 'Save-AzResourceGroupDeploymentTemplate' to use the SDK.</span></span>
* <span data-ttu-id="89801-288">Adição do cmdlet "Unregister-AzResourceProvider".</span><span class="sxs-lookup"><span data-stu-id="89801-288">Added 'Unregister-AzResourceProvider' cmdlet.</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-289">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-289">Az.Sql</span></span>
* <span data-ttu-id="89801-290">Adição de suporte para o Principal de serviço e utilizadores convidados no cmdlet Set-AzSqlInstanceActiveDirectoryAdministrator</span><span class="sxs-lookup"><span data-stu-id="89801-290">Added support for Service principal and guest users in Set-AzSqlInstanceActiveDirectoryAdministrator cmdlet'</span></span>
* <span data-ttu-id="89801-291">Correção de um erro em cmdlets de Classificação de Dados.</span><span class="sxs-lookup"><span data-stu-id="89801-291">Fixed a bug in Data Classification cmdlets.'</span></span>
* <span data-ttu-id="89801-292">Adição de suporte para a ativação pós-falha do Azure SQL Managed Instance: "Invoke-AzSqlInstanceFailover"</span><span class="sxs-lookup"><span data-stu-id="89801-292">Added support for Azure SQL Managed Instance failover: 'Invoke-AzSqlInstanceFailover'</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-293">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-293">Az.Storage</span></span>
* <span data-ttu-id="89801-294">Correção do erro de que o UserAgent não é adicionado para alguns cmdlets do plano de dados.</span><span class="sxs-lookup"><span data-stu-id="89801-294">Fixed the issue that UserAgent is not added for some data plane cmdlets.</span></span>
* <span data-ttu-id="89801-295">Suporte para a criação/atualização da Conta de armazenamento com MinimumTlsVersion e AllowBlobPublicAccess</span><span class="sxs-lookup"><span data-stu-id="89801-295">Supported create/update Storage account with MinimumTlsVersion and AllowBlobPublicAccess</span></span>
    -  <span data-ttu-id="89801-296">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="89801-296">'New-AzStorageAccount'</span></span>
    -  <span data-ttu-id="89801-297">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="89801-297">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="89801-298">Suporte para Permitir/desativar o controlo de versões no Serviço Blob de uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="89801-298">Support enable/disable versioning on Blob Service of a Storage account</span></span>
    - <span data-ttu-id="89801-299">"Update-AzStorageBlobServiceProperty"</span><span class="sxs-lookup"><span data-stu-id="89801-299">'Update-AzStorageBlobServiceProperty'</span></span>
* <span data-ttu-id="89801-300">Suporte para a lista de blobs com versões de blobs</span><span class="sxs-lookup"><span data-stu-id="89801-300">Support list blobs with blob versions</span></span>
    - <span data-ttu-id="89801-301">"Get-AzStorageBlob"</span><span class="sxs-lookup"><span data-stu-id="89801-301">'Get-AzStorageBlob'</span></span>
* <span data-ttu-id="89801-302">Suporte para obter/remover instantâneo de blob único ou versão do blob</span><span class="sxs-lookup"><span data-stu-id="89801-302">Support get/remove single blob snapshot or blob version</span></span>
    - <span data-ttu-id="89801-303">"Get-AzStorageBlob"</span><span class="sxs-lookup"><span data-stu-id="89801-303">'Get-AzStorageBlob'</span></span>
    - <span data-ttu-id="89801-304">"Remove-AzStorageBlob"</span><span class="sxs-lookup"><span data-stu-id="89801-304">'Remove-AzStorageBlob'</span></span>
* <span data-ttu-id="89801-305">Suporte para pipeline a partir do objeto de blob gerado a partir de Azure.Storage.Blobs V12</span><span class="sxs-lookup"><span data-stu-id="89801-305">Support pipeline from blob object generated from Azure.Storage.Blobs V12</span></span>
    - <span data-ttu-id="89801-306">"Get-AzStorageBlobContent"</span><span class="sxs-lookup"><span data-stu-id="89801-306">'Get-AzStorageBlobContent'</span></span>
    - <span data-ttu-id="89801-307">"New-AzStorageBlobSASToken"</span><span class="sxs-lookup"><span data-stu-id="89801-307">'New-AzStorageBlobSASToken'</span></span>
    - <span data-ttu-id="89801-308">"Remove-AzStorageBlob"</span><span class="sxs-lookup"><span data-stu-id="89801-308">'Remove-AzStorageBlob'</span></span>
    - <span data-ttu-id="89801-309">"Set-AzStorageBlobContent"</span><span class="sxs-lookup"><span data-stu-id="89801-309">'Set-AzStorageBlobContent'</span></span>
    - <span data-ttu-id="89801-310">"Start-AzStorageBlobCopy"</span><span class="sxs-lookup"><span data-stu-id="89801-310">'Start-AzStorageBlobCopy'</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="89801-311">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="89801-311">Az.StorageSync</span></span>
* <span data-ttu-id="89801-312">Adição de uma nova versão StorageSync SDK para ApiVersion 2020-03-01</span><span class="sxs-lookup"><span data-stu-id="89801-312">Added a new version StorageSync SDK targeting ApiVersion 2020-03-01</span></span>
* <span data-ttu-id="89801-313">Adição de cmdlet do Serviço de Sincronização de Armazenamento de Atualização</span><span class="sxs-lookup"><span data-stu-id="89801-313">Added Update Storage Sync Service cmdlet</span></span>
    - <span data-ttu-id="89801-314">"Set-AzStorageSyncService"</span><span class="sxs-lookup"><span data-stu-id="89801-314">'Set-AzStorageSyncService'</span></span>
* <span data-ttu-id="89801-315">Adição de IncomingTrafficPolicy e PrivateEndpointConnections para cmdlets StorageSyncService.</span><span class="sxs-lookup"><span data-stu-id="89801-315">Added IncomingTrafficPolicy and PrivateEndpointConnections to StorageSyncService cmdlets.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="89801-316">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-316">Az.Websites</span></span>
* <span data-ttu-id="89801-317">Adição de suporte para a realização de operações para Slots em grupos de recursos diferentes do Plano do Serviço de Aplicações</span><span class="sxs-lookup"><span data-stu-id="89801-317">Added support to perform operations for Slots not in the same resource group as the App Service Plan</span></span>

## <a name="430---june-2020"></a><span data-ttu-id="89801-318">4.3.0 - Junho de 2020</span><span class="sxs-lookup"><span data-stu-id="89801-318">4.3.0 - June 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="89801-319">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-319">Az.Accounts</span></span>
* <span data-ttu-id="89801-320">Suporte para a deteção da definição do ambiente por predefinição e adição de ambiente através de "Add-AzEnvironment"</span><span class="sxs-lookup"><span data-stu-id="89801-320">Supported discovering environment setting by default and adding environment via 'Add-AzEnvironment'</span></span>
* <span data-ttu-id="89801-321">Atualizar assemblagens pré-carregadas [#12024], [#11976]</span><span class="sxs-lookup"><span data-stu-id="89801-321">Update preloaded assemblies [#12024], [#11976]</span></span>
* <span data-ttu-id="89801-322">Atualização da assemblagem Azure.Core</span><span class="sxs-lookup"><span data-stu-id="89801-322">Updated Azure.Core assembly</span></span>
* <span data-ttu-id="89801-323">Correção de um problema que pode provocar a falha de "Connect-AzAccount" numa execução de múltiplos threads [#11201]</span><span class="sxs-lookup"><span data-stu-id="89801-323">Fixed an issue that may cause 'Connect-AzAccount' to fail in multi-threaded execution [#11201]</span></span>

#### <a name="azaks"></a><span data-ttu-id="89801-324">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="89801-324">Az.Aks</span></span>
* <span data-ttu-id="89801-325">Substituição da utilização da [API AccessProfile](https://docs.microsoft.com/rest/api/aks/managedclusters/getaccessprofile) antiga por chamadas para as APIs [ListClusterAdmin](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusteradmincredentials) e [ListClusterUser](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusterusercredentials)</span><span class="sxs-lookup"><span data-stu-id="89801-325">Replaced usage of old [AccessProfile API](https://docs.microsoft.com/rest/api/aks/managedclusters/getaccessprofile) with calls to [ListClusterAdmin](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusteradmincredentials) and [ListClusterUser](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusterusercredentials) APIs</span></span>

#### <a name="azbatch"></a><span data-ttu-id="89801-326">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="89801-326">Az.Batch</span></span>
* <span data-ttu-id="89801-327">Atualização da versão do SDK de Az.Batch para utilizar "Microsoft.Azure.Management.Batch" para 11.0.0</span><span class="sxs-lookup"><span data-stu-id="89801-327">Updated Az.Batch to use 'Microsoft.Azure.Management.Batch' SDK version to 11.0.0</span></span>
* <span data-ttu-id="89801-328">Adição da capacidade de definir a Identidade BatchAccount no cmdlet "New-AzBatchAccount"</span><span class="sxs-lookup"><span data-stu-id="89801-328">Added the ability to set the BatchAccount Identity in the 'New-AzBatchAccount' cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="89801-329">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="89801-329">Az.CognitiveServices</span></span>
* <span data-ttu-id="89801-330">Suporte para a apresentação das capacidades da conta.</span><span class="sxs-lookup"><span data-stu-id="89801-330">Supported displaying account capabilities.</span></span>
* <span data-ttu-id="89801-331">Suporte para a modificação de PublicNetworkAccess.</span><span class="sxs-lookup"><span data-stu-id="89801-331">Supported modifying PublicNetworkAccess.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-332">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-332">Az.Compute</span></span>
* <span data-ttu-id="89801-333">Adição do parâmetro SimulateEviction aos cmdlets Set-AzVM e Set-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="89801-333">Added SimulateEviction parameter to Set-AzVM and Set-AzVmssVM cmdlets.</span></span>
* <span data-ttu-id="89801-334">Adição de "Premium_LRS" ao mecanismo de preenchimento de argumentos do parâmetro StorageAccountType para o cmdlet New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="89801-334">Added 'Premium_LRS' to the argument completer of StorageAccountType parameter for New-AzGalleryImageVersion cmdlet.</span></span>
* <span data-ttu-id="89801-335">Adição de subestados a VMCustomScriptExtension [#11297]</span><span class="sxs-lookup"><span data-stu-id="89801-335">Added Substatuses to VMCustomScriptExtension [#11297]</span></span>
* <span data-ttu-id="89801-336">Adição de "Delete" ao mecanismo de preenchimento de argumentos do parâmetro EvictionPolicy para os cmdlets New-AzVM e New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="89801-336">Added 'Delete' to the argument completer of EvictionPolicy parameter for New-AzVM and New-AzVMConfig cmdlets.</span></span>
* <span data-ttu-id="89801-337">Correção do nome da nova Extensão de VM para SAP</span><span class="sxs-lookup"><span data-stu-id="89801-337">Fixed name of new VM Extension for SAP</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="89801-338">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="89801-338">Az.DataFactory</span></span>
* <span data-ttu-id="89801-339">Atualização da versão do SDK de .Net do ADF para 4.9.0</span><span class="sxs-lookup"><span data-stu-id="89801-339">Updated ADF .Net SDK version to 4.9.0</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="89801-340">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="89801-340">Az.EventHub</span></span>
* <span data-ttu-id="89801-341">Adição de parâmetros de Identidade Gerida aos cmdlets "New-AzEventHubNamespace" e "Set-AzEventHubNamespace"</span><span class="sxs-lookup"><span data-stu-id="89801-341">Added Managed Identity parameters to 'New-AzEventHubNamespace' and 'Set-AzEventHubNamespace' cmdlets</span></span>

#### <a name="azfunctions"></a><span data-ttu-id="89801-342">Az.Functions</span><span class="sxs-lookup"><span data-stu-id="89801-342">Az.Functions</span></span>
* <span data-ttu-id="89801-343">Adição de suporte para a criação de aplicações de funções do PowerShell 7.0 e de Java 11</span><span class="sxs-lookup"><span data-stu-id="89801-343">Added support to create PowerShell 7.0 and Java 11 function apps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="89801-344">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="89801-344">Az.HDInsight</span></span>
* <span data-ttu-id="89801-345">Suporte para listagem de anfitriões e reinício de anfitriões específicos do cluster HDInsight.</span><span class="sxs-lookup"><span data-stu-id="89801-345">Supported listing hosts and restart specific hosts of the HDInsight cluster.</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="89801-346">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="89801-346">Az.HealthcareApis</span></span>
* <span data-ttu-id="89801-347">Atualização da versão do SDK para 1.1.0</span><span class="sxs-lookup"><span data-stu-id="89801-347">Updated the SDK version to 1.1.0</span></span>
* <span data-ttu-id="89801-348">Adição de suporte para as definições de Exportação e a Identidade Gerida</span><span class="sxs-lookup"><span data-stu-id="89801-348">Added support for Export settings and Managed Identity</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="89801-349">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="89801-349">Az.Monitor</span></span>
* <span data-ttu-id="89801-350">Correção do parâmetro de objeto de entrada para "Set-AzActivityLogAlert"</span><span class="sxs-lookup"><span data-stu-id="89801-350">Fixed input object parameter for 'Set-AzActivityLogAlert'</span></span>
* <span data-ttu-id="89801-351">Correção do parâmetro "InputObject" para "Set-AzActionGroup" [#10868]</span><span class="sxs-lookup"><span data-stu-id="89801-351">Fixed 'InputObject' parameter for 'Set-AzActionGroup' [#10868]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-352">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-352">Az.Network</span></span>
* <span data-ttu-id="89801-353">Adição de suporte para o parâmetro AddressPrefixType a "Remove-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="89801-353">Added support for AddressPrefixType parameter to 'Remove-AzExpressRouteCircuitConnectionConfig'</span></span>
* <span data-ttu-id="89801-354">Adição de novos cmdlets para a Política de Firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="89801-354">Added new cmdlets for Azure FirewallPolicy</span></span>
    - <span data-ttu-id="89801-355">"New-AzFirewallPolicyDnsSetting"</span><span class="sxs-lookup"><span data-stu-id="89801-355">'New-AzFirewallPolicyDnsSetting'</span></span>
    - <span data-ttu-id="89801-356">Suporte para FQDN de Destino nas Regras de Rede para a Política de Firewall</span><span class="sxs-lookup"><span data-stu-id="89801-356">Support for Destination FQDN in Network Rules for Firewall Policy</span></span>
* <span data-ttu-id="89801-357">Adição de suporte para operações de conjuntos de endereços back-end</span><span class="sxs-lookup"><span data-stu-id="89801-357">Added support for backend address pool operations</span></span>
    - <span data-ttu-id="89801-358">"New-AzLoadBalancerBackendAddressConfig"</span><span class="sxs-lookup"><span data-stu-id="89801-358">'New-AzLoadBalancerBackendAddressConfig'</span></span>
    - <span data-ttu-id="89801-359">"New-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="89801-359">'New-AzLoadBalancerBackendAddressPool'</span></span>
    - <span data-ttu-id="89801-360">"Set-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="89801-360">'Set-AzLoadBalancerBackendAddressPool'</span></span>
    - <span data-ttu-id="89801-361">"Remove-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="89801-361">'Remove-AzLoadBalancerBackendAddressPool'</span></span>
    - <span data-ttu-id="89801-362">"Get-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="89801-362">'Get-AzLoadBalancerBackendAddressPool'</span></span>
* <span data-ttu-id="89801-363">Adição de validação de nomes para "New-AzIpGroup"</span><span class="sxs-lookup"><span data-stu-id="89801-363">Added name validation for 'New-AzIpGroup'</span></span>
* <span data-ttu-id="89801-364">Adição de novos cmdlets para a Política de Firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="89801-364">Added new cmdlets for Azure FirewallPolicy</span></span>
    - <span data-ttu-id="89801-365">"New-AzFirewallPolicyThreatIntelWhitelist"</span><span class="sxs-lookup"><span data-stu-id="89801-365">'New-AzFirewallPolicyThreatIntelWhitelist'</span></span>
* <span data-ttu-id="89801-366">Foram atualizados os seguintes comandos para a funcionalidade: Definição/remoção de servidores DNS personalizados no P2SVpnGateway de VirtualWan.</span><span class="sxs-lookup"><span data-stu-id="89801-366">Updated below commands for feature: Custom dns servers set/remove on VirtualWan P2SVpnGateway.</span></span>
    - <span data-ttu-id="89801-367">Atualização de New-AzP2sVpnGateway: Adição do parâmetro opcional "-CustomDnsServer" para os clientes especificarem os respetivos servidores DNS a definir no P2SVpnGateway, o qual pode ser utilizado por clientes do tipo Ponto a site.</span><span class="sxs-lookup"><span data-stu-id="89801-367">Updated New-AzP2sVpnGateway: Added optional parameter '-CustomDnsServer' for customers to specify their dns servers to set on P2SVpnGateway, which can be used by Point to site clients.</span></span>
    - <span data-ttu-id="89801-368">Atualização de Update-AzP2sVpnGateway: Adição do parâmetro opcional "-CustomDnsServer" para os clientes especificarem os respetivos servidores DNS a definir no P2SVpnGateway, o qual pode ser utilizado por clientes do tipo Ponto a site.</span><span class="sxs-lookup"><span data-stu-id="89801-368">Updated Update-AzP2sVpnGateway: Added optional parameter '-CustomDnsServer' for customers to specify their dns servers to set on P2SVpnGateway, which can be used by Point to site clients.</span></span>
* <span data-ttu-id="89801-369">Atualização de "Update-AzVpnGateway"</span><span class="sxs-lookup"><span data-stu-id="89801-369">Updated 'Update-AzVpnGateway'</span></span>
    - <span data-ttu-id="89801-370">Adição do parâmetro opcional "-BgpPeeringAddress" para os clientes especificarem os respetivos bgps personalizados a definir no VpnGateway.</span><span class="sxs-lookup"><span data-stu-id="89801-370">Added optional parameter '-BgpPeeringAddress' for customers to specify their custom bgps to set on VpnGateway.</span></span>
* <span data-ttu-id="89801-371">Adição de novo cmdlet para suportar a reposição do estado de encaminhamento de um recurso VirtualHub:</span><span class="sxs-lookup"><span data-stu-id="89801-371">Added new cmdlet to support resetting the routing state of a VirtualHub resource:</span></span>
    - <span data-ttu-id="89801-372">"Reset-AzHubRouter"</span><span class="sxs-lookup"><span data-stu-id="89801-372">'Reset-AzHubRouter'</span></span>
* <span data-ttu-id="89801-373">Atualização dos elementos indicados abaixo com base na alteração recente de Swagger para a Política de Firewall</span><span class="sxs-lookup"><span data-stu-id="89801-373">Updated below things based on recent swagger change for Firewall Policy</span></span>
    - <span data-ttu-id="89801-374">Alteração de nomes para RuleGroup, RuleCollectionGroup e RuleType</span><span class="sxs-lookup"><span data-stu-id="89801-374">Changes names for RuleGroup, RuleCollectionGroup and RuleType</span></span>
    - <span data-ttu-id="89801-375">Adição de suporte para Coleções de Regras de NAT da Política de Firewall para suportar várias Coleções de Regras de NAT</span><span class="sxs-lookup"><span data-stu-id="89801-375">Added support for Firewall Policy NAT Rule Collections to support multiple NAT Rule Collection</span></span>
* <span data-ttu-id="89801-376">[Alteração Interruptiva] Adição do parâmetro obrigatório "SourceIpGroup" para "New-AzFirewallPolicyApplicationRule" e "New-AzFirewallPolicyNetworkRule".</span><span class="sxs-lookup"><span data-stu-id="89801-376">[Breaking Change] Added mandatory parameter 'SourceIpGroup' for 'New-AzFirewallPolicyApplicationRule' and 'New-AzFirewallPolicyNetworkRule'.</span></span>
* <span data-ttu-id="89801-377">[Alteração Interruptiva] Correção do parâmetro "SourceAddress" de "New-AzFirewallPolicyApplicationRule" de modo a ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89801-377">[Breaking Change] Fixed 'New-AzFirewallPolicyApplicationRule', parameter 'SourceAddress' to be mandatory.</span></span>
* <span data-ttu-id="89801-378">[Alteração Interruptiva] Correção do parâmetro "SourceAddress" de "New-AzFirewallPolicyApplicationRule" de modo a ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89801-378">[Breaking Change] Fixed 'New-AzFirewallPolicyApplicationRule', parameter 'SourceAddress' to be mandatory.</span></span>
* <span data-ttu-id="89801-379">[Alteração Interruptiva] Remoção de parâmetros obrigatórios: "TranslatedAddress", "TranslatedPort" para "New-AzFirewallPolicyNatRuleCollection".</span><span class="sxs-lookup"><span data-stu-id="89801-379">[Breaking Change] Removed mandatory parameters: 'TranslatedAddress', 'TranslatedPort' for 'New-AzFirewallPolicyNatRuleCollection'.</span></span>
* <span data-ttu-id="89801-380">Adição de novos cmdlets para suportar PrivateLink no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="89801-380">Added new cmdlets to support PrivateLink On Application Gateway</span></span>
    - <span data-ttu-id="89801-381">"New-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="89801-381">'New-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="89801-382">"Get-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="89801-382">'Get-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="89801-383">"New-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="89801-383">'New-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="89801-384">"Set-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="89801-384">'Set-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="89801-385">"Remove-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="89801-385">'Remove-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="89801-386">"New-AzApplicationGatewayPrivateLinkIpConfiguration"</span><span class="sxs-lookup"><span data-stu-id="89801-386">'New-AzApplicationGatewayPrivateLinkIpConfiguration'</span></span>
* <span data-ttu-id="89801-387">Adição de novos cmdlets para o recurso subordinado HubRouteTables de VirtualHub.</span><span class="sxs-lookup"><span data-stu-id="89801-387">Added new cmdlets for HubRouteTables child resource of VirtualHub.</span></span>
    - <span data-ttu-id="89801-388">"New-AzVHubRoute"</span><span class="sxs-lookup"><span data-stu-id="89801-388">'New-AzVHubRoute'</span></span>
    - <span data-ttu-id="89801-389">"New-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="89801-389">'New-AzVHubRouteTable'</span></span>
    - <span data-ttu-id="89801-390">"Get-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="89801-390">'Get-AzVHubRouteTable'</span></span>
    - <span data-ttu-id="89801-391">"Update-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="89801-391">'Update-AzVHubRouteTable'</span></span>
    - <span data-ttu-id="89801-392">"Remove-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="89801-392">'Remove-AzVHubRouteTable'</span></span>
* <span data-ttu-id="89801-393">Atualização dos cmdlets existentes para suportar o parâmetro de entrada opcional RoutingConfiguration para encaminhamento personalizado em VirtualWan.</span><span class="sxs-lookup"><span data-stu-id="89801-393">Updated existing cmdlets to support optional RoutingConfiguration input parameter for custom routing in VirtualWan.</span></span>
    - <span data-ttu-id="89801-394">"New-AzExpressRouteConnection"</span><span class="sxs-lookup"><span data-stu-id="89801-394">'New-AzExpressRouteConnection'</span></span>
    - <span data-ttu-id="89801-395">"Set-AzExpressRouteConnection"</span><span class="sxs-lookup"><span data-stu-id="89801-395">'Set-AzExpressRouteConnection'</span></span>
    - <span data-ttu-id="89801-396">"New-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="89801-396">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="89801-397">"Update-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="89801-397">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="89801-398">"New-AzVpnConnection"</span><span class="sxs-lookup"><span data-stu-id="89801-398">'New-AzVpnConnection'</span></span>
    - <span data-ttu-id="89801-399">"Update-AzVpnConnection"</span><span class="sxs-lookup"><span data-stu-id="89801-399">'Update-AzVpnConnection'</span></span>
    - <span data-ttu-id="89801-400">"New-AzP2sVpnGateway"</span><span class="sxs-lookup"><span data-stu-id="89801-400">'New-AzP2sVpnGateway'</span></span>
    - <span data-ttu-id="89801-401">"Update-AzP2sVpnGateway"</span><span class="sxs-lookup"><span data-stu-id="89801-401">'Update-AzP2sVpnGateway'</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="89801-402">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="89801-402">Az.OperationalInsights</span></span>
* <span data-ttu-id="89801-403">Correção do erro PSWorkspace não implementa IOperationalInsightsWorkspace [#12135]</span><span class="sxs-lookup"><span data-stu-id="89801-403">Fixed bug PSWorkspace doesn't implement IOperationalInsightsWorkspace [#12135]</span></span>
* <span data-ttu-id="89801-404">Adição de "pergb2018" ao conjunto de valores válidos do parâmetro "Sku" em "Set-AzOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="89801-404">Added 'pergb2018' to valid value set of parameter 'Sku' in 'Set-AzOperationalInsightsWorkspace'</span></span> 
* <span data-ttu-id="89801-405">Adição do alias "FunctionParameters" para o parâmetro "FunctionParameter" a</span><span class="sxs-lookup"><span data-stu-id="89801-405">Added alias 'FunctionParameters' for parameter 'FunctionParameter' to</span></span>
    - <span data-ttu-id="89801-406">"New-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="89801-406">'New-AzOperationalInsightsSavedSearch'</span></span>
    - <span data-ttu-id="89801-407">"Set-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="89801-407">'Set-AzOperationalInsightsSavedSearch'</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-408">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-408">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-409">Adição de suporte no Azure Backup para a obtenção de itens de MAB.</span><span class="sxs-lookup"><span data-stu-id="89801-409">Azure Backup added support for fetching MAB items.</span></span>
* <span data-ttu-id="89801-410">Suporte do Azure Site Recovery para o tipo de disco "StandardSSD_LRS"</span><span class="sxs-lookup"><span data-stu-id="89801-410">Azure Site Recovery supports disk type 'StandardSSD_LRS'</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-411">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-411">Az.Resources</span></span>
* <span data-ttu-id="89801-412">Adição de "UsageLocation", "GivenName", "Surname", "AccountEnabled", "MailNickname", "Mail" em "PSADUser" [#10526] [#10497]</span><span class="sxs-lookup"><span data-stu-id="89801-412">Added 'UsageLocation', 'GivenName', 'Surname', 'AccountEnabled', 'MailNickname', 'Mail' on 'PSADUser' [#10526] [#10497]</span></span>
* <span data-ttu-id="89801-413">Correção do problema em que "-Mail" não funciona em "Get-AzADUser" [#11981]</span><span class="sxs-lookup"><span data-stu-id="89801-413">Fixed issue that '-Mail' doesn't work on 'Get-AzADUser' [#11981]</span></span>
* <span data-ttu-id="89801-414">Adição do parâmetro "-ExcludeChangeType" a "Get-AzDeploymentWhatIfResult" e "Get-AzResourceGroupDeploymentWhatIfResult"</span><span class="sxs-lookup"><span data-stu-id="89801-414">Added '-ExcludeChangeType' parameter to 'Get-AzDeploymentWhatIfResult' and 'Get-AzResourceGroupDeploymentWhatIfResult'</span></span>
* <span data-ttu-id="89801-415">Adição do parâmetro "-WhatIfExcludeChangeType" a "New-AzDeployment" e "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="89801-415">Added '-WhatIfExcludeChangeType' parameter to 'New-AzDeployment' and 'New-AzResourceGroupDeployment'</span></span>
* <span data-ttu-id="89801-416">Atualização de cmdlets "Test-Az\*Deployment" para apresentação de mensagens de erro melhores</span><span class="sxs-lookup"><span data-stu-id="89801-416">Updated 'Test-Az\*Deployment' cmdlets to show better error messages</span></span>
* <span data-ttu-id="89801-417">Correção da mensagem de ajuda para o parâmetro "-Name" de criação de implementação e cmdlets What-If</span><span class="sxs-lookup"><span data-stu-id="89801-417">Fixed help message for '-Name' parameter of deployment create and What-If cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-418">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-418">Az.Sql</span></span>
* <span data-ttu-id="89801-419">Adição de suporte para o principal de serviço para o cmdlet Set SQL Server Azure Active Directory Admin</span><span class="sxs-lookup"><span data-stu-id="89801-419">Added support for service principal for Set SQL Server Azure Active Directory Admin cmdlet</span></span>
* <span data-ttu-id="89801-420">Correção de problema de sincronização em cmdlets de Classificação de Dados.</span><span class="sxs-lookup"><span data-stu-id="89801-420">Fixed sync issue in Data Classification cmdlets.</span></span>
* <span data-ttu-id="89801-421">Suporte para a pesquisa de utilizador por correio em "Set-AzSqlServerActiveDirectoryAdministrator" [#12192]</span><span class="sxs-lookup"><span data-stu-id="89801-421">Supported searching user by mail on 'Set-AzSqlServerActiveDirectoryAdministrator' [#12192]</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-422">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-422">Az.Storage</span></span>
* <span data-ttu-id="89801-423">Suporte para a criação de Conta de armazenamento com RequireInfrastructureEncryption</span><span class="sxs-lookup"><span data-stu-id="89801-423">Supported create Storage account with RequireInfrastructureEncryption</span></span>
    -  <span data-ttu-id="89801-424">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="89801-424">'New-AzStorageAccount'</span></span>
* <span data-ttu-id="89801-425">Mudança da lógica de carregamento de Azure.Core para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-425">Moved the logic of loading Azure.Core to Az.Accounts</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="89801-426">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-426">Az.Websites</span></span>
* <span data-ttu-id="89801-427">Adição de salvaguarda para eliminar a aplicação Web criada em caso de falha do restauro em "Restore-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="89801-427">Added safeguard to delete created webapp if restore failed in 'Restore-AzDeletedWebApp'</span></span>
* <span data-ttu-id="89801-428">Adição de "SourceWebApp.Location" para "New-AzWebApp" e "New-AzWebAppSlot"</span><span class="sxs-lookup"><span data-stu-id="89801-428">Added 'SourceWebApp.Location' for 'New-AzWebApp' and 'New-AzWebAppSlot'</span></span>
* <span data-ttu-id="89801-429">Correção do erro que impedia a alteração de definições de Contentor em "Set-AzWebApp" e "Set-AzWebAppSlot"</span><span class="sxs-lookup"><span data-stu-id="89801-429">Fixed bug that prevented changing Container settings in 'Set-AzWebApp' and 'Set-AzWebAppSlot'</span></span>
* <span data-ttu-id="89801-430">Correção do erro para obter SiteConfig quando -Name não é fornecido para Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="89801-430">Fixed bug to get SiteConfig when -Name is not given for Get-AzWebApp</span></span>
* <span data-ttu-id="89801-431">Adição de suporte para a criação de ASP para Aplicações Linux</span><span class="sxs-lookup"><span data-stu-id="89801-431">Added a support to create ASP for Linux Apps</span></span>
* <span data-ttu-id="89801-432">Adição de exceções para clonagem entre grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="89801-432">Added exceptions for clone across resource groups</span></span>

## <a name="420---june-2020"></a><span data-ttu-id="89801-433">4.2.0 - Junho de 2020</span><span class="sxs-lookup"><span data-stu-id="89801-433">4.2.0 - June 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="89801-434">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-434">Az.Accounts</span></span>
* <span data-ttu-id="89801-435">Correção de um problema que fazia com que o Az ignorasse registos nas tarefas da Automatização do Azure ou do PowerShell [#11492]</span><span class="sxs-lookup"><span data-stu-id="89801-435">Fixed an issue that may cause Az to skip logs in Azure Automation or PowerShell jobs [#11492]</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="89801-436">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="89801-436">Az.AnalysisServices</span></span>
* <span data-ttu-id="89801-437">Atualização da versão de assemblagem dos cmdlets de plano de dados</span><span class="sxs-lookup"><span data-stu-id="89801-437">Updated assembly version of data plane cmdlets</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="89801-438">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="89801-438">Az.ApiManagement</span></span>
* <span data-ttu-id="89801-439">Atualização da versão de assemblagem dos cmdlets de gestão de serviços</span><span class="sxs-lookup"><span data-stu-id="89801-439">Updated assembly version of service management cmdlets</span></span>

#### <a name="azbilling"></a><span data-ttu-id="89801-440">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="89801-440">Az.Billing</span></span>
* <span data-ttu-id="89801-441">Atualização da versão de assemblagem dos cmdlets de consumo</span><span class="sxs-lookup"><span data-stu-id="89801-441">Updated assembly version of consumption cmdlets</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="89801-442">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="89801-442">Az.CognitiveServices</span></span>
* <span data-ttu-id="89801-443">Suporte para o controlo de PrivateEndpoint e PublicNetworkAccess.</span><span class="sxs-lookup"><span data-stu-id="89801-443">Support PrivateEndpoint and PublicNetworkAccess control.</span></span> 

#### <a name="azdatafactory"></a><span data-ttu-id="89801-444">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="89801-444">Az.DataFactory</span></span>
* <span data-ttu-id="89801-445">Atualização da versão de assemblagem dos cmdlets V2 de fábrica de dados</span><span class="sxs-lookup"><span data-stu-id="89801-445">Updated assembly version of data factory V2 cmdlets</span></span>

#### <a name="azdatashare"></a><span data-ttu-id="89801-446">Az.DataShare</span><span class="sxs-lookup"><span data-stu-id="89801-446">Az.DataShare</span></span>
* <span data-ttu-id="89801-447">Disponibilidade geral do módulo "Az.DataShare"</span><span class="sxs-lookup"><span data-stu-id="89801-447">General availability of ''Az.DataShare'' module</span></span>

#### <a name="azdesktopvirtualization"></a><span data-ttu-id="89801-448">Az.DesktopVirtualization</span><span class="sxs-lookup"><span data-stu-id="89801-448">Az.DesktopVirtualization</span></span>
* <span data-ttu-id="89801-449">Disponibilidade geral do módulo "Az.DesktopVirtualization"</span><span class="sxs-lookup"><span data-stu-id="89801-449">General availability of ''Az.DesktopVirtualization'' module</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="89801-450">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="89801-450">Az.OperationalInsights</span></span>
* <span data-ttu-id="89801-451">Atualização do SDK para a versão 0.21.0</span><span class="sxs-lookup"><span data-stu-id="89801-451">Upgraded SDK to 0.21.0</span></span>
* <span data-ttu-id="89801-452">Adição de parâmetros opcionais a</span><span class="sxs-lookup"><span data-stu-id="89801-452">Added optional parameters to</span></span> 
    - <span data-ttu-id="89801-453">"New-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="89801-453">'New-AzOperationalInsightsSavedSearch'</span></span>
    - <span data-ttu-id="89801-454">"Set-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="89801-454">'Set-AzOperationalInsightsSavedSearch'</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="89801-455">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="89801-455">Az.PolicyInsights</span></span>
* <span data-ttu-id="89801-456">Correção do exemplo 3 de "Start-AzPolicyComplianceScan"</span><span class="sxs-lookup"><span data-stu-id="89801-456">Corrected example 3 for 'Start-AzPolicyComplianceScan'</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="89801-457">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="89801-457">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="89801-458">Atualização da versão de assemblagem dos cmdlets do PowerBI</span><span class="sxs-lookup"><span data-stu-id="89801-458">Updated assembly version of PowerBI cmdlets</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="89801-459">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="89801-459">Az.PrivateDns</span></span>
* <span data-ttu-id="89801-460">Correção da formatação da cadeia de saída verbosa de Remove-AzPrivateDnsRecordSet</span><span class="sxs-lookup"><span data-stu-id="89801-460">Corrected verbose output string formatting for Remove-AzPrivateDnsRecordSet</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-461">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-461">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-462">Suporte do Azure Site Recovery para a criação de um plano de recuperação para replicação zona a zona a partir de uma entrada xml.</span><span class="sxs-lookup"><span data-stu-id="89801-462">Azure Site Recovery support for creating recovery plan for zone to zone replication from xml input.</span></span>
* <span data-ttu-id="89801-463">Atualização da versão de assemblagem dos cmdlets do SiteRecovery e Backup</span><span class="sxs-lookup"><span data-stu-id="89801-463">Updated assembly version of SiteRecovery and Backup cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-464">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-464">Az.Resources</span></span>
* <span data-ttu-id="89801-465">Adição do parâmetro Tail aos cmdlets Get-AzDeploymentScriptLog e Save-AzDeploymentScriptLog</span><span class="sxs-lookup"><span data-stu-id="89801-465">Added Tail parameter to Get-AzDeploymentScriptLog and Save-AzDeploymentScriptLog cmdlets</span></span>
* <span data-ttu-id="89801-466">Formatação da propriedade Output e apresentação da mesma na saída do cmdlet Get-AzDeploymentScript</span><span class="sxs-lookup"><span data-stu-id="89801-466">Formatted Output property and show it on the Get-AzDeploymentScript cmdlet output</span></span>
* <span data-ttu-id="89801-467">Mudança de nome do parâmetro -DeploymentScriptInputObject para -DeploymentScriptObject</span><span class="sxs-lookup"><span data-stu-id="89801-467">Renamed -DeploymentScriptInputObject parameter to -DeploymentScriptObject</span></span>
* <span data-ttu-id="89801-468">Correção do nome em falta do ficheiro/destino nas mensagens de cmdlet.</span><span class="sxs-lookup"><span data-stu-id="89801-468">Fixed missing file/target name in cmdlet messages.</span></span>
* <span data-ttu-id="89801-469">Atualização da versão de assemblagem dos cmdlets de gestor de recursos e de etiquetas</span><span class="sxs-lookup"><span data-stu-id="89801-469">Updated assembly version of resource manager and tags cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-470">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-470">Az.Sql</span></span>
* <span data-ttu-id="89801-471">Adição de UsePrivateLinkConnection a "New-AzSqlSyncGroup", "Update-AzSqlSyncGroup", "New-AzSqlSyncMember" e "Update-AzSqlSyncMember"</span><span class="sxs-lookup"><span data-stu-id="89801-471">Added UsePrivateLinkConnection to 'New-AzSqlSyncGroup', 'Update-AzSqlSyncGroup', 'New-AzSqlSyncMember' and 'Update-AzSqlSyncMember'</span></span>
* <span data-ttu-id="89801-472">Adição de SyncMemberAzureDatabaseResourceId a "New-AzSqlSyncMember" e "Update-AzSqlSyncMember"</span><span class="sxs-lookup"><span data-stu-id="89801-472">Added SyncMemberAzureDatabaseResourceId to 'New-AzSqlSyncMember' and 'Update-AzSqlSyncMember'</span></span>
* <span data-ttu-id="89801-473">Adição do suporte de pesquisa de Utilizador convidado ao cmdlet Set SQL Server Azure Active Directory Admin</span><span class="sxs-lookup"><span data-stu-id="89801-473">Added Guest user lookup support to Set SQL Server Azure Active Directory Admin cmdlet</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-474">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-474">Az.Storage</span></span>
* <span data-ttu-id="89801-475">Atualização da versão de assemblagem dos cmdlets de plano de dados</span><span class="sxs-lookup"><span data-stu-id="89801-475">Updated assembly version of data plane cmdlets</span></span>

## <a name="410---may-2020"></a><span data-ttu-id="89801-476">4.1.0 - Maio de 2020</span><span class="sxs-lookup"><span data-stu-id="89801-476">4.1.0 - May 2020</span></span>
### <a name="highlights-since-the-last-release"></a><span data-ttu-id="89801-477">Destaques desde a última versão</span><span class="sxs-lookup"><span data-stu-id="89801-477">Highlights since the last release</span></span>
* <span data-ttu-id="89801-478">Versões do PowerShell suportadas: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span><span class="sxs-lookup"><span data-stu-id="89801-478">Supported PowerShell versions: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span></span>
* <span data-ttu-id="89801-479">Disponibilidade geral de Az.Functions</span><span class="sxs-lookup"><span data-stu-id="89801-479">General availability of Az.Functions</span></span> 
* <span data-ttu-id="89801-480">Az.ApiManagement, Az.Batch, Az.Compute, Az.KeyVault, Az.Monitor, Az.Network, Az.OperationalInsights, Az.Resources e Az.Storage são alvo de grandes versões</span><span class="sxs-lookup"><span data-stu-id="89801-480">Az.ApiManagement, Az.Batch, Az.Compute, Az.KeyVault, Az.Monitor, Az.Network, Az.OperationalInsights, Az.Resources, and Az.Storage have major release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="89801-481">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-481">Az.Accounts</span></span>
* <span data-ttu-id="89801-482">"Add-AzEnvironment" e "Set-AzEnvironment" foram atualizados para aceitar os parâmetros "AzureSynapseAnalyticsEndpointResourceId" e "AzureSynapseAnalyticsEndpointSuffix"</span><span class="sxs-lookup"><span data-stu-id="89801-482">Updated 'Add-AzEnvironment' and 'Set-AzEnvironment' to accept parameters 'AzureSynapseAnalyticsEndpointResourceId' and 'AzureSynapseAnalyticsEndpointSuffix'</span></span>
* <span data-ttu-id="89801-483">Foram adicionadas assemblagens relacionadas ao Azure.Core em Az.Accounts; as plataformas suportadas do PowerShell incluem Windows PowerShell 5.1, PowerShell Core 6.2.4, PowerShell 7+</span><span class="sxs-lookup"><span data-stu-id="89801-483">Added Azure.Core related assemblies into Az.Accounts, supported PowerShell platforms include Windows PowerShell 5.1, PowerShell Core 6.2.4, PowerShell 7+</span></span>

#### <a name="azaks"></a><span data-ttu-id="89801-484">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="89801-484">Az.Aks</span></span>
* <span data-ttu-id="89801-485">Versão da API atualizada para 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="89801-485">Upgraded API Version to 2019-10-01</span></span>
* <span data-ttu-id="89801-486">Suportado para criar o AKS com contentores do Windows</span><span class="sxs-lookup"><span data-stu-id="89801-486">Supported to create AKS using Windows container</span></span>
* <span data-ttu-id="89801-487">Novos cmdlets fornecidos: "New-AzAksNodePool", "Update-AzAksNodePool", "Remove-AzAksNodePool",        "Get-AzAksNodePool", "Install-AzAksKubectl", "Get-AzAksVersion"</span><span class="sxs-lookup"><span data-stu-id="89801-487">Provided new cmdlets: 'New-AzAksNodePool', 'Update-AzAksNodePool', 'Remove-AzAksNodePool',        'Get-AzAksNodePool', 'Install-AzAksKubectl', 'Get-AzAksVersion'</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="89801-488">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="89801-488">Az.ApiManagement</span></span>
* <span data-ttu-id="89801-489">"New-AzApiManagement" e "Set-AzApiManagement": o nome do parâmetro [-AssignIdentity] foi mudado para [-SystemAssignedIdentity]</span><span class="sxs-lookup"><span data-stu-id="89801-489">'New-AzApiManagement' and 'Set-AzApiManagement': [-AssignIdentity] parameter renamed as [-SystemAssignedIdentity]</span></span>
* <span data-ttu-id="89801-490">"New-AzApiManagement" e "Set-AzApiManagement": Novo parâmetro adicionado: [-UserAssignedIdentity <String[]>]</span><span class="sxs-lookup"><span data-stu-id="89801-490">'New-AzApiManagement' and 'Set-AzApiManagement': New parameter added: [-UserAssignedIdentity <String[]>]</span></span>
* <span data-ttu-id="89801-491">"Get-AzApiManagementProperty": o nome foi mudado para "Get-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="89801-491">'Get-AzApiManagementProperty': renamed as 'Get-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="89801-492">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="89801-492">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="89801-493">"New-AzApiManagementProperty": o nome foi mudado para "New-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="89801-493">'New-AzApiManagementProperty': renamed as 'New-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="89801-494">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="89801-494">PropertyId parameter renamed as NamedValueId.</span></span> 
* <span data-ttu-id="89801-495">"Set-AzApiManagementProperty": o nome foi mudado para "Set-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="89801-495">'Set-AzApiManagementProperty': renamed as 'Set-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="89801-496">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="89801-496">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="89801-497">"Remove-AzApiManagementProperty": o nome foi mudado para "Remove-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="89801-497">'Remove-AzApiManagementProperty': renamed as 'Remove-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="89801-498">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="89801-498">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="89801-499">Foi adicionado o cmdlet novo "Get-AzApiManagementAuthorizationServerClientSecret" e "Get-AzApiManagementAuthorizationServer" vai deixar de devolver o segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="89801-499">Added new 'Get-AzApiManagementAuthorizationServerClientSecret' cmdlet and 'Get-AzApiManagementAuthorizationServer' will not return client secret anymore.</span></span>
* <span data-ttu-id="89801-500">Foi adicionado o cmdlet novo "Get-AzApiManagementNamedValueSecretValue" e "Get-AzApiManagementNamedValue" vai deixar de devolver o valor do segredo.</span><span class="sxs-lookup"><span data-stu-id="89801-500">Added new 'Get-AzApiManagementNamedValueSecretValue' cmdlet and 'Get-AzApiManagementNamedValue' will not return secret value.</span></span>
* <span data-ttu-id="89801-501">Foi adicionado o cmdlet novo "Get-AzApiManagementOpenIdConnectProviderClientSecret" e "Get-AzApiManagementOpenIdConnectProvider" vai deixar de devolver o segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="89801-501">Added new 'Get-AzApiManagementOpenIdConnectProviderClientSecret' cmdlet and 'Get-AzApiManagementOpenIdConnectProvider' will not return client secret anymore.</span></span>
* <span data-ttu-id="89801-502">Foi adicionado o cmdlet "Get-AzApiManagementSubscriptionKey" e "Get-AzApiManagementSubscription" vai deixar de devolver chaves de subscrições.</span><span class="sxs-lookup"><span data-stu-id="89801-502">Added new 'Get-AzApiManagementSubscriptionKey' cmdlet and 'Get-AzApiManagementSubscription' will not return subscription keys anymore.</span></span>
* <span data-ttu-id="89801-503">Foi adicionado o cmdlet novo "Get-AzApiManagementTenantAccessSecret" e "Get-AzApiManagementTenantAccess" vai deixar de devolver chaves.</span><span class="sxs-lookup"><span data-stu-id="89801-503">Added new 'Get-AzApiManagementTenantAccessSecret' cmdlet and 'Get-AzApiManagementTenantAccess' will not return keys anymore.</span></span>
* <span data-ttu-id="89801-504">Foi adicionado o cmdlet novo "Get-AzApiManagementTenantGitAccessSecret" e "Get-AzApiManagementTenantGitAccess" vai deixar de devolver chaves.</span><span class="sxs-lookup"><span data-stu-id="89801-504">Added new 'Get-AzApiManagementTenantGitAccessSecret' cmdlet and 'Get-AzApiManagementTenantGitAccess' will not return keys anymore.</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="89801-505">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="89801-505">Az.ApplicationInsights</span></span>
* <span data-ttu-id="89801-506">Parâmetros adicionados: "RetentionInDays" "PublicNetworkAccessForIngestion" "PublicNetworkAccessForQuery" a "New-AzApplicationInsights"</span><span class="sxs-lookup"><span data-stu-id="89801-506">Added Parameters: 'RetentionInDays' 'PublicNetworkAccessForIngestion' 'PublicNetworkAccessForQuery' for 'New-AzApplicationInsights'</span></span>
* <span data-ttu-id="89801-507">Foi criado o cmdlet "Update-AzApplicationInsights”</span><span class="sxs-lookup"><span data-stu-id="89801-507">Created cmdlet 'Update-AzApplicationInsights'</span></span>
* <span data-ttu-id="89801-508">Foram criados cmdlets para a Conta de Armazenamento Associada</span><span class="sxs-lookup"><span data-stu-id="89801-508">Created cmdlets for Linked Storage Account</span></span>

#### <a name="azbatch"></a><span data-ttu-id="89801-509">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="89801-509">Az.Batch</span></span>
* <span data-ttu-id="89801-510">Az.Batch foi atualizado para utilizar a versão do SDK "Microsoft.Azure.Batc" 13.0.0 e a versão do SDK "Microsoft.Azure.Management.Batch" 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="89801-510">Updated Az.Batch to use 'Microsoft.Azure.Batch' SDK version 13.0.0 and 'Microsoft.Azure.Management.Batch' SDK version 9.0.0.</span></span>
* <span data-ttu-id="89801-511">Foi adicionada a capacidade de selecionar o tipo de certificado que vai ser adicionado mediante a utilização do novo parâmetro "-CertificateKind" para "New-AzBatchCertificate".</span><span class="sxs-lookup"><span data-stu-id="89801-511">Added the ability to select the kind of certificate being added using the new '-CertificateKind' parameter to 'New-AzBatchCertificate'.</span></span>
* <span data-ttu-id="89801-512">A propriedade "ApplicationPackages" foi removida de "PSApplication", que anteriormente era sempre ''.</span><span class="sxs-lookup"><span data-stu-id="89801-512">Removed 'ApplicationPackages' property from 'PSApplication' which was previously always ''.</span></span>
  - <span data-ttu-id="89801-513">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com "Get-AzBatchApplicationPackage".</span><span class="sxs-lookup"><span data-stu-id="89801-513">The specific packages inside of an application now can be retrieved using 'Get-AzBatchApplicationPackage'.</span></span> <span data-ttu-id="89801-514">Por exemplo: "Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication".</span><span class="sxs-lookup"><span data-stu-id="89801-514">For example: 'Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication'.</span></span>
* <span data-ttu-id="89801-515">Agora, ao utilizar "New-AzBatchPool" para criar um conjunto, a propriedade "VirtualMachineImageId" de "PSImageReference" só pode fazer referência a uma imagem do Shared Image Gallery.</span><span class="sxs-lookup"><span data-stu-id="89801-515">When creating a pool using 'New-AzBatchPool', the 'VirtualMachineImageId' property of 'PSImageReference' can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="89801-516">Ao utilizar "New-AzBatchPool" para criar um conjunto, o conjunto pode ser aprovisionado sem um IP público mediante a utilização da nova propriedade "PublicIPAddressConfiguration" de "PSNetworkConfiguration".</span><span class="sxs-lookup"><span data-stu-id="89801-516">When creating a pool using 'New-AzBatchPool', the pool can be provisioned without a public IP using the new 'PublicIPAddressConfiguration' property of 'PSNetworkConfiguration'.</span></span>
  - <span data-ttu-id="89801-517">A propriedade "PublicIPs" de "PSNetworkConfiguration" foi igualmente movida para "PSPublicIPAddressConfiguration".</span><span class="sxs-lookup"><span data-stu-id="89801-517">The 'PublicIPs' property of 'PSNetworkConfiguration' has moved in to 'PSPublicIPAddressConfiguration' as well.</span></span> <span data-ttu-id="89801-518">Esta propriedade só pode ser especificada se "IPAddressProvisioningType" for "UserManaged".</span><span class="sxs-lookup"><span data-stu-id="89801-518">This property can only be specified if 'IPAddressProvisioningType' is 'UserManaged'.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-519">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-519">Az.Compute</span></span>
* <span data-ttu-id="89801-520">Foi adicionado o parâmetro HostId ao cmdlet "Update-AzVM"</span><span class="sxs-lookup"><span data-stu-id="89801-520">Added HostId parameter to 'Update-AzVM' cmdlet</span></span>
* <span data-ttu-id="89801-521">Os documentos de Ajuda para os cmdlets "New-AzVMConfig", "New-AzVmssConfig", "Update-AzVmss", "Set-AzVMOperatingSystem" e "Set-AzVmssOsProfile" foram atualizados.</span><span class="sxs-lookup"><span data-stu-id="89801-521">Updated Help documents for 'New-AzVMConfig', 'New-AzVmssConfig', 'Update-AzVmss', 'Set-AzVMOperatingSystem' and 'Set-AzVmssOsProfile' cmdlets.</span></span>
* <span data-ttu-id="89801-522">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="89801-522">Breaking changes</span></span>
    - <span data-ttu-id="89801-523">O parâmetro FilterExpression foi removido do cmdlet "Get-AzVMImage".</span><span class="sxs-lookup"><span data-stu-id="89801-523">FilterExpression parameter is removed from 'Get-AzVMImage' cmdlet.</span></span>
    - <span data-ttu-id="89801-524">O parâmetro AssignIdentity foi removido dos cmdlets "New-AzVmssConfig", "New-AzVMConfig" e "Update-AzVM".</span><span class="sxs-lookup"><span data-stu-id="89801-524">AssignIdentity parameter is removed from 'New-AzVmssConfig', 'New-AzVMConfig' and 'Update-AzVM' cmdlets.</span></span>
    - <span data-ttu-id="89801-525">AutomaticRepairMaxInstanceRepairsPercent foi removido dos cmdlets "New-AzVmssConfig" e "Update-AzVmss".</span><span class="sxs-lookup"><span data-stu-id="89801-525">AutomaticRepairMaxInstanceRepairsPercent is removed from 'New-AzVmssConfig' and 'Update-AzVmss' cmdlets.</span></span>
    - <span data-ttu-id="89801-526">As propriedades AvailabilitySetsColocationStatus, VirtualMachinesColocationStatus e VirtualMachineScaleSetsColocationStatus foram removidas de ProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="89801-526">AvailabilitySetsColocationStatus, VirtualMachinesColocationStatus and VirtualMachineScaleSetsColocationStatus properties are removed from ProximityPlacementGroup.</span></span>
    - <span data-ttu-id="89801-527">A propriedade MaxInstanceRepairsPercent foi removida de AutomaticRepairsPolicy.</span><span class="sxs-lookup"><span data-stu-id="89801-527">MaxInstanceRepairsPercent property is removed from AutomaticRepairsPolicy.</span></span>
    - <span data-ttu-id="89801-528">Os tipos de AvailabilitySets, VirtualMachines e VirtualMachineScaleSets foram alterados de IList<SubResource> para IList<SubResourceWithColocationStatus>.</span><span class="sxs-lookup"><span data-stu-id="89801-528">The types of AvailabilitySets, VirtualMachines and VirtualMachineScaleSets are changed from IList<SubResource> to IList<SubResourceWithColocationStatus>.</span></span>
* <span data-ttu-id="89801-529">A descrição do cmdlet "Get-AzVM" foi atualizada para o descrever melhor.</span><span class="sxs-lookup"><span data-stu-id="89801-529">Description for 'Get-AzVM' cmdlet has been updated to better describe it.</span></span> 

#### <a name="azdatafactory"></a><span data-ttu-id="89801-530">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="89801-530">Az.DataFactory</span></span>
* <span data-ttu-id="89801-531">CRUD suportado das propriedades de fluxo de dados no IR Gerido.</span><span class="sxs-lookup"><span data-stu-id="89801-531">Supported CRUD of data flow runtime properties in Managed IR.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="89801-532">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="89801-532">Az.FrontDoor</span></span>
* <span data-ttu-id="89801-533">Foram adicionados cmdlets novos para criação, atualização, obtenção e eliminação do objeto de Motor de Regras do Front Door</span><span class="sxs-lookup"><span data-stu-id="89801-533">Added new cmdlets for creation, update, retreival, and deletion of Front Door Rules Engine object</span></span>
* <span data-ttu-id="89801-534">Foram adicionados cmdlets de programas auxiliares para construção do objeto de Motor de Regras do Front Door</span><span class="sxs-lookup"><span data-stu-id="89801-534">Added helper cmdlets for construction of Front Door Rules Engine object</span></span>
* <span data-ttu-id="89801-535">Foi adicionada a referência ao Motor de Regras ao objeto Regra de Encaminhamento do Front Door.</span><span class="sxs-lookup"><span data-stu-id="89801-535">Added Rules Engine reference to Front Door Routing Rule object.</span></span>
* <span data-ttu-id="89801-536">Foram adicionados parâmetros do Private Link ao objeto de Back-end do Front Door</span><span class="sxs-lookup"><span data-stu-id="89801-536">Added Private Link parameters to Front Door Backend object</span></span>

#### <a name="azfunctions"></a><span data-ttu-id="89801-537">Az.Functions</span><span class="sxs-lookup"><span data-stu-id="89801-537">Az.Functions</span></span>
* <span data-ttu-id="89801-538">Disponibilidade geral do módulo Az.Functions</span><span class="sxs-lookup"><span data-stu-id="89801-538">General availability of ''Az.Functions'' module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="89801-539">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="89801-539">Az.HDInsight</span></span>
* <span data-ttu-id="89801-540">Encriptação de discos de chave gerida pelo cliente suportada</span><span class="sxs-lookup"><span data-stu-id="89801-540">Supported Customer-managed key disk encryption.</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="89801-541">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="89801-541">Az.HealthcareApis</span></span>
* <span data-ttu-id="89801-542">As políticas de acesso já não são predefinidas para o principal atual</span><span class="sxs-lookup"><span data-stu-id="89801-542">Access policies are no longer defaulted to the current principal</span></span>

#### <a name="aziothub"></a><span data-ttu-id="89801-543">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="89801-543">Az.IotHub</span></span>
* <span data-ttu-id="89801-544">Foi adicionado um cmdlet para invocar uma consulta num hub IoT para obter informações mediante a utilização de uma linguagem tipo SQL.</span><span class="sxs-lookup"><span data-stu-id="89801-544">Added cmdlet to invoke a query in an IoT hub to retrieve information using a SQL-like language.</span></span>
* <span data-ttu-id="89801-545">Foi corrigido um problema em que "Add-AzIotHubDevice" falha ao criar um Dispositivo Compatível com o Edge sem dispositivos subordinados [#11597]</span><span class="sxs-lookup"><span data-stu-id="89801-545">Fix issue that 'Add-AzIotHubDevice' fails to create Edge Enabled Device without child devices [#11597]</span></span>
* <span data-ttu-id="89801-546">Foi adicionado o cmdlet para gerar o token de SAS para o Hub IoT, um dispositivo ou um módulo.</span><span class="sxs-lookup"><span data-stu-id="89801-546">Added cmdlet to generate SAS token for Iot Hub, device or module.</span></span>
* <span data-ttu-id="89801-547">Foi adicionado um cmdlet para invocar a consulta de métricas de configuração.</span><span class="sxs-lookup"><span data-stu-id="89801-547">Added cmdlet to invoke configuration metrics query.</span></span>
* <span data-ttu-id="89801-548">Gerir implementações automáticas do IoT Edge em escala.</span><span class="sxs-lookup"><span data-stu-id="89801-548">Manage IoT Edge automatic deployment at scale.</span></span> <span data-ttu-id="89801-549">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="89801-549">New cmdlets are:</span></span>
    - <span data-ttu-id="89801-550">"Add-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="89801-550">'Add-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="89801-551">"Get-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="89801-551">'Get-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="89801-552">"Remove-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="89801-552">'Remove-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="89801-553">"Set-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="89801-553">'Set-AzIotHubDeployment'</span></span>
* <span data-ttu-id="89801-554">Foi adicionado um cmdlet para invocar uma consulta de métricas de implementação do IoT Edge.</span><span class="sxs-lookup"><span data-stu-id="89801-554">Added cmdlet to invoke an IoT Edge deployment metrics query.</span></span>
* <span data-ttu-id="89801-555">Foi adicionado um cmdlet para aplicar o conteúdo da configuração ao dispositivo edge especificado.</span><span class="sxs-lookup"><span data-stu-id="89801-555">Added cmdlet to apply the configuration content to the specified edge device.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="89801-556">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="89801-556">Az.KeyVault</span></span>
* <span data-ttu-id="89801-557">Foram removidos dois aliases: "New-AzKeyVaultCertificateAdministratorDetails" e "New-AzKeyVaultCertificateOrganizationDetails"</span><span class="sxs-lookup"><span data-stu-id="89801-557">Removed two aliases: 'New-AzKeyVaultCertificateAdministratorDetails' and 'New-AzKeyVaultCertificateOrganizationDetails'</span></span>
* <span data-ttu-id="89801-558">A eliminação recuperável foi ativada por predefinição ao criar um cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="89801-558">Enabled soft delete by default when creating a key vault</span></span>
* <span data-ttu-id="89801-559">Podem ser definidas regras de rede para governar a acessibilidade a partir de localizações na rede ao criar um cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="89801-559">Network rules can be set to govern the accessibility from specific network locations when creating a key vault</span></span>
* <span data-ttu-id="89801-560">Foi adicionado suporte para Bring Your Own Key (BYOK)</span><span class="sxs-lookup"><span data-stu-id="89801-560">Added support to bring your own key (BYOK)</span></span>
    - <span data-ttu-id="89801-561">"Add-AzKeyVaultKey" suporta a geração de chaves de intercâmbio de chaves</span><span class="sxs-lookup"><span data-stu-id="89801-561">'Add-AzKeyVaultKey' supports generating a key exchange key</span></span>
    - <span data-ttu-id="89801-562">"Get-AzKeyVaultKey" suporta a transferência de chaves públicas no formato PEM</span><span class="sxs-lookup"><span data-stu-id="89801-562">'Get-AzKeyVaultKey' supports downloading a public key in PEM format</span></span>
* <span data-ttu-id="89801-563">"KeyOps" foi atualizado como parte do documento de ajuda de "Add-AzKeyVaultKey"</span><span class="sxs-lookup"><span data-stu-id="89801-563">Updated the 'KeyOps' part of the help document of 'Add-AzKeyVaultKey'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="89801-564">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="89801-564">Az.Monitor</span></span>
* <span data-ttu-id="89801-565">Foi corrigido um erro em "Set-AzDiagnosticSettings"; a política de retenção não se aplicará a todas as categorias [#11589]</span><span class="sxs-lookup"><span data-stu-id="89801-565">Fixed bug for 'Set-AzDiagnosticSettings', retention policy won't apply to all categories [#11589]</span></span>
* <span data-ttu-id="89801-566">Suporte para critérios de disponibilidade de WebTest para alertas de métricas V2</span><span class="sxs-lookup"><span data-stu-id="89801-566">Supported WebTest availability criteria for metric alert V2</span></span>
    - <span data-ttu-id="89801-567">Novo "New-AzMetricAlertRuleV2Criteria": foi adicionada uma opção para criar critérios de disponibilidade WebTest</span><span class="sxs-lookup"><span data-stu-id="89801-567">'New-AzMetricAlertRuleV2Criteria': an option to create webtest availability criteria was added</span></span>
    - <span data-ttu-id="89801-568">"Add-AzMetricAlertRuleV2": suporta os novos critérios de disponibilidade de WebTest</span><span class="sxs-lookup"><span data-stu-id="89801-568">'Add-AzMetricAlertRuleV2': supports the new webtest availability criteria</span></span>
* <span data-ttu-id="89801-569">Foi removida a definição redundante de RetentionPolicy em PSLogProfile [#7608]</span><span class="sxs-lookup"><span data-stu-id="89801-569">Removed redundant definition for RetentionPolicy in PSLogProfile [#7608]</span></span>
* <span data-ttu-id="89801-570">Foram removidas as propriedades redundantes definidas em PSEventData [#11353]</span><span class="sxs-lookup"><span data-stu-id="89801-570">Removed redundant properties difined in PSEventData [#11353]</span></span>
* <span data-ttu-id="89801-571">O nome de "Get-AzLog" foi mudado para "Get-AzActivityLog"</span><span class="sxs-lookup"><span data-stu-id="89801-571">Renamed 'Get-AzLog' to 'Get-AzActivityLog'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-572">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-572">Az.Network</span></span>
* <span data-ttu-id="89801-573">Foi adicionado um atributo de alteração interruptiva para notificar que o comportamento predefinido da Zona vai ser alterado</span><span class="sxs-lookup"><span data-stu-id="89801-573">Added breaking change attribute to notify that Zone default behaviour will be changed</span></span>
    - <span data-ttu-id="89801-574">"New-AzPublicIpAddress"</span><span class="sxs-lookup"><span data-stu-id="89801-574">'New-AzPublicIpAddress'</span></span>
    - <span data-ttu-id="89801-575">"New-AzPublicIpPrefix"</span><span class="sxs-lookup"><span data-stu-id="89801-575">'New-AzPublicIpPrefix'</span></span>
    - <span data-ttu-id="89801-576">"New-AzLoadBalancerFrontendIpConfig"</span><span class="sxs-lookup"><span data-stu-id="89801-576">'New-AzLoadBalancerFrontendIpConfig'</span></span>
* <span data-ttu-id="89801-577">Foi adicionado suportado para um recurso de nível superior novo SecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="89801-577">Added support for a new top level resource SecurityPartnerProvider</span></span>
    - <span data-ttu-id="89801-578">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="89801-578">New cmdlets added:</span></span>
        - <span data-ttu-id="89801-579">New-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="89801-579">New-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="89801-580">Remove-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="89801-580">Remove-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="89801-581">Get-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="89801-581">Get-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="89801-582">Set-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="89801-582">Set-AzSecurityPartnerProvider</span></span>
* <span data-ttu-id="89801-583">Foi adicionado "RequiredZoneNames" em "PSPrivateLinkResource" e "GroupId" em "PSPrivateEndpointConnection”</span><span class="sxs-lookup"><span data-stu-id="89801-583">Added 'RequiredZoneNames' on 'PSPrivateLinkResource' and 'GroupId' on 'PSPrivateEndpointConnection'</span></span>
* <span data-ttu-id="89801-584">Foi corrigido o tipo incorreto do parâmetro SuccessThresholdRoundTripTimeMs para New-AzNetworkWatcherConnectionMonitorTestConfigurationObject</span><span class="sxs-lookup"><span data-stu-id="89801-584">Fixed incorrect type of SuccessThresholdRoundTripTimeMs parameter for New-AzNetworkWatcherConnectionMonitorTestConfigurationObject</span></span>
* <span data-ttu-id="89801-585">Foram atualizados os cmdlets VirtualWan para definir o valor predefinido do argumento AllowVnetToVnetTraffic como Verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="89801-585">Updated VirtualWan cmdlets to set default value of AllowVnetToVnetTraffic argument to True.</span></span>
    - <span data-ttu-id="89801-586">"New-AzVirtualWan"</span><span class="sxs-lookup"><span data-stu-id="89801-586">'New-AzVirtualWan'</span></span>
    - <span data-ttu-id="89801-587">"Update-AzVirtualWan"</span><span class="sxs-lookup"><span data-stu-id="89801-587">'Update-AzVirtualWan'</span></span>
* <span data-ttu-id="89801-588">Foram adicionados cmdlets para suportar o grupo de zonas DNS para pontos finais privados</span><span class="sxs-lookup"><span data-stu-id="89801-588">Added new cmdlets to support DNS zone group for private endpoint</span></span>
    - <span data-ttu-id="89801-589">"New-AzPrivateDnsZoneConfig"</span><span class="sxs-lookup"><span data-stu-id="89801-589">'New-AzPrivateDnsZoneConfig'</span></span>
    - <span data-ttu-id="89801-590">"Get-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="89801-590">'Get-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="89801-591">"New-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="89801-591">'New-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="89801-592">"Set-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="89801-592">'Set-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="89801-593">"Remove-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="89801-593">'Remove-AzPrivateDnsZoneGroup'</span></span>
* <span data-ttu-id="89801-594">Foram adicionados os parâmetros "DNSEnableProxy", "DNSRequireProxyForNetworkRules" e "DNSServers" a "AzureFirewall"</span><span class="sxs-lookup"><span data-stu-id="89801-594">Added 'DNSEnableProxy', 'DNSRequireProxyForNetworkRules' and 'DNSServers' parameters to 'AzureFirewall'</span></span>
* <span data-ttu-id="89801-595">Foram adicionados os parâmetros "EnableDnsProxy", "DnsProxyNotRequiredForNetworkRule" e "DnsServer" a "AzureFirewall"</span><span class="sxs-lookup"><span data-stu-id="89801-595">Added 'EnableDnsProxy', 'DnsProxyNotRequiredForNetworkRule' and 'DnsServer' parameters to 'AzureFirewall'</span></span>
    - <span data-ttu-id="89801-596">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="89801-596">Updated cmdlet:</span></span>
        - <span data-ttu-id="89801-597">New-AzFirewall</span><span class="sxs-lookup"><span data-stu-id="89801-597">New-AzFirewall</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="89801-598">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="89801-598">Az.OperationalInsights</span></span>
* <span data-ttu-id="89801-599">O código legado foi atualizado para aplicar o SDK recém-gerado</span><span class="sxs-lookup"><span data-stu-id="89801-599">Updated legacy code to apply new generated SDK</span></span>
* <span data-ttu-id="89801-600">Foram eliminados cmdlets devido a APIs preteridas</span><span class="sxs-lookup"><span data-stu-id="89801-600">Deleted cmdlets due to deprecated APIs</span></span>
    - <span data-ttu-id="89801-601">"Get-AzOperationalInsightsSavedSearchResult" (alias "Get-AzOperationalInsightsSavedSearchResults")</span><span class="sxs-lookup"><span data-stu-id="89801-601">'Get-AzOperationalInsightsSavedSearchResult' (alias 'Get-AzOperationalInsightsSavedSearchResults')</span></span>
    - <span data-ttu-id="89801-602">"Get-AzOperationalInsightsSearchResult" (alias "Get-AzOperationalInsightsSearchResults")</span><span class="sxs-lookup"><span data-stu-id="89801-602">'Get-AzOperationalInsightsSearchResult' (alias 'Get-AzOperationalInsightsSearchResults')</span></span>
    - <span data-ttu-id="89801-603">"Get-AzOperationalInsightsLinkTarget" (alias "Get-AzOperationalInsightsLinkTargets")</span><span class="sxs-lookup"><span data-stu-id="89801-603">'Get-AzOperationalInsightsLinkTarget' (alias 'Get-AzOperationalInsightsLinkTargets')</span></span>
* <span data-ttu-id="89801-604">Foram adicionados parâmetros para "Set-AzOperationalInsightsWorkspace" e "New-AzOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="89801-604">Added parameters for 'Set-AzOperationalInsightsWorkspace' and 'New-AzOperationalInsightsWorkspace'</span></span>
* <span data-ttu-id="89801-605">Foram criados cmdlets para a Conta de Armazenamento Associada</span><span class="sxs-lookup"><span data-stu-id="89801-605">Created cmdlets for Linked Stoarge Account</span></span>
* <span data-ttu-id="89801-606">Foram criados cmdlets para Clusters e para o Serviço Associado</span><span class="sxs-lookup"><span data-stu-id="89801-606">Created cmdlets for Clusters and Linked Service</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-607">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-607">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-608">O Azure Site Recovery adicionou suporte para proteger máquinas virtuais de grupo de colocação por proximidade para fornecedor do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-608">Azure Site Recovery added support for protecting proximity placement group virtual machines for Azure to Azure provider.</span></span>
* <span data-ttu-id="89801-609">O Azure Site Recovery adicionou suporte para a replicação de zona para zona.</span><span class="sxs-lookup"><span data-stu-id="89801-609">Azure Site Recovery added support for zone to zone replication.</span></span>
* <span data-ttu-id="89801-610">O Azure Backup adicionou suporte para a retenção de longo prazo para Pontos de Recuperação de Partilhas de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-610">Azure Backup Added Long term retention support for Azure FileShare Recovery Points.</span></span>
* <span data-ttu-id="89801-611">O Azure Backup adicionou propriedades de exclusão de discos à saída do cmdlet "Get-AzRecoveryServicesBackupItem".</span><span class="sxs-lookup"><span data-stu-id="89801-611">Azure Backup Added disk exclusion properties to 'Get-AzRecoveryServicesBackupItem' cmdlet output.</span></span>
* <span data-ttu-id="89801-612">Foi adicionado o ponto final privado para o ficheiro de credenciais de Cofre para o Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="89801-612">Added private endpoint for Vault credential file for site recovery service.</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-613">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-613">Az.Resources</span></span>
* <span data-ttu-id="89801-614">Foi adicionado um aviso de mensagem relativo a um atraso na vista ao criar uma Definição de Função nova</span><span class="sxs-lookup"><span data-stu-id="89801-614">Added message warning about view delay when creating a new Role Definition</span></span>
* <span data-ttu-id="89801-615">Os cmdlets de política foram alterados para produzir objetos de tipos compatíveis</span><span class="sxs-lookup"><span data-stu-id="89801-615">Changed policy cmdlets to output strongly-typed objects</span></span>
* <span data-ttu-id="89801-616">Foi removido o parâmetro "-TenantLevel" utilizado no cmdlet "Get-AzResourceLock" [#11335]</span><span class="sxs-lookup"><span data-stu-id="89801-616">Removed '-TenantLevel' parameter used for on the 'Get-AzResourceLock' cmdlet [#11335]</span></span>
* <span data-ttu-id="89801-617">"Remove-AzResourceGroup -Id ResourceId" foi corrigido [#9882]</span><span class="sxs-lookup"><span data-stu-id="89801-617">Fixed 'Remove-AzResourceGroup -Id ResourceId'[#9882]</span></span>
* <span data-ttu-id="89801-618">Foi adicionado um cmdlet novo para obter resultados de What-If de modelos do ARM no âmbito de um grupo de recursos: "Get-AzDeploymentResourceGroupWhatIfResult"</span><span class="sxs-lookup"><span data-stu-id="89801-618">Added new cmdlet for getting ARM template What-If results at resource group scope: 'Get-AzDeploymentResourceGroupWhatIfResult'</span></span>
* <span data-ttu-id="89801-619">Foi adicionado um cmdlet novo para obter resultados de What-If de modelos do ARM no âmbito de uma subscrição: "Get-AzDeploymentWhatIfResult"</span><span class="sxs-lookup"><span data-stu-id="89801-619">Added new cmdlet for getting ARM template What-If results at subscription scope: 'Get-AzDeploymentWhatIfResult'</span></span>
   - <span data-ttu-id="89801-620">Alias: "Get-AzSubscriptionDeploymentWhatIf"</span><span class="sxs-lookup"><span data-stu-id="89801-620">Alias: 'Get-AzSubscriptionDeploymentWhatIf'</span></span>
* <span data-ttu-id="89801-621">Os parâmetros "-WhatIf" e "-Confirm" foram substituídos para "New-AzDeployment" e "New-AzResourceGroupDeployment" para utilizar resultados de What-If de modelos do ARM</span><span class="sxs-lookup"><span data-stu-id="89801-621">Overrode '-WhatIf' and '-Confirm' parameters for 'New-AzDeployment' and 'New-AzResourceGroupDeployment' to use ARM template What-If results</span></span>
* <span data-ttu-id="89801-622">Foi adicionada a mensagem de descontinuação para o parâmetro "ApiVersion" em cmdlets implementados</span><span class="sxs-lookup"><span data-stu-id="89801-622">Added deprecation message for 'ApiVersion' parameter in deployment cmdlets</span></span>
* <span data-ttu-id="89801-623">Foi adicionada a capacidade para mostrar mensagens de erro melhoradas relativas a falhas em implementações</span><span class="sxs-lookup"><span data-stu-id="89801-623">Added capability to show improved error messages for deployment failures</span></span>
* <span data-ttu-id="89801-624">Foi adicionado o registo de correlationId para falhas em implementações</span><span class="sxs-lookup"><span data-stu-id="89801-624">Added correlationId logging for deployment failures</span></span>
* <span data-ttu-id="89801-625">Foi adicionada a propriedade "error" à saída do script de implementação</span><span class="sxs-lookup"><span data-stu-id="89801-625">Added 'error' property to the deployment script output</span></span>
* <span data-ttu-id="89801-626">O nuget Microsoft.Azure.Management.ResourceManager foi atualizado para "3.7.1-preview"</span><span class="sxs-lookup"><span data-stu-id="89801-626">Updated nuget Microsoft.Azure.Management.ResourceManager to '3.7.1-preview'</span></span>
* <span data-ttu-id="89801-627">Foram removidos casos de teste específicos, uma vez que a propriedade Error em DeploymentValidateResult foi alterada para apenas de leitura a partir de 3.7.1-preview</span><span class="sxs-lookup"><span data-stu-id="89801-627">Removed specific test cases as Error property in DeploymentValidateResult has changed to readonly from nuget 3.7.1-preview</span></span>
* <span data-ttu-id="89801-628">GenericResourceExpanded foi importado do SDK ResourceManager 3.7.1-preview</span><span class="sxs-lookup"><span data-stu-id="89801-628">Brought GenericResourceExpanded from SDK ResourceManager 3.7.1-preview</span></span>
* <span data-ttu-id="89801-629">Foi adicionado suporte para etiquetas a todos os cmdlets Get para implementação, bem como</span><span class="sxs-lookup"><span data-stu-id="89801-629">Added tag support for all Get cmdlets for deployment, as well as</span></span>
    - <span data-ttu-id="89801-630">"New-AzDeployment"</span><span class="sxs-lookup"><span data-stu-id="89801-630">'New-AzDeployment'</span></span>
    - <span data-ttu-id="89801-631">"New-AzManagementGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="89801-631">'New-AzManagementGroupDeployment'</span></span>
    - <span data-ttu-id="89801-632">"New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="89801-632">'New-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="89801-633">"New-AzTenantDeployment"</span><span class="sxs-lookup"><span data-stu-id="89801-633">'New-AzTenantDeployment'</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="89801-634">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="89801-634">Az.ServiceFabric</span></span>
* <span data-ttu-id="89801-635">Foi corrigido um erro na adição de certificados mediante a utilização de --SecretIdentifier que obtinha o thumbprint de certificado incorreto</span><span class="sxs-lookup"><span data-stu-id="89801-635">Fixed bug in add certificate using --SecretIdentifier that was getting the wrong certificate thumbprint</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-636">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-636">Az.Sql</span></span>
* <span data-ttu-id="89801-637">Foi melhorado o desempenho de:</span><span class="sxs-lookup"><span data-stu-id="89801-637">Enhance performance of:</span></span>
    - <span data-ttu-id="89801-638">"Set-AzSqlDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="89801-638">'Set-AzSqlDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="89801-639">"Set-AzSqlInstanceDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="89801-639">'Set-AzSqlInstanceDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="89801-640">"Remove-AzSqlDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="89801-640">'Remove-AzSqlDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="89801-641">"Remove-AzSqlInstanceDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="89801-641">'Remove-AzSqlInstanceDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="89801-642">"Enable-AzSqlDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="89801-642">'Enable-AzSqlDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="89801-643">"Enable-AzSqlInstanceDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="89801-643">'Enable-AzSqlInstanceDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="89801-644">"Disable-AzSqlDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="89801-644">'Disable-AzSqlDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="89801-645">"Disable-AzSqlInstanceDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="89801-645">'Disable-AzSqlInstanceDatabaseSensitivityRecommendation'</span></span>
* <span data-ttu-id="89801-646">Foi removida a validação do lado do cliente do parâmetro "RetentionDays" do cmdlet "Set-AzSqlDatabaseBackupShortTermRetentionPolicy"</span><span class="sxs-lookup"><span data-stu-id="89801-646">Removed client-side validation of 'RetentionDays' parameter from cmdlet 'Set-AzSqlDatabaseBackupShortTermRetentionPolicy'</span></span>
* <span data-ttu-id="89801-647">Auditoria a uma conta de armazenamento na Vnet; corrigido um erro ao criar uma função de Contribuidor de Dados de Blobs de Armazenamento.</span><span class="sxs-lookup"><span data-stu-id="89801-647">Auditing to a storage account in Vnet, fixing a bug when creating a Storage Blob Data Contributor role.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-648">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-648">Az.Storage</span></span>
* <span data-ttu-id="89801-649">Foi adicionado "-AsJob" ao cmdlet para obter/listar contas "Get-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="89801-649">Added '-AsJob' to get/list account cmdlet 'Get-AzStorageAccount'</span></span>
* <span data-ttu-id="89801-650">KeyVersion foi tornado opcional ao atualizar a conta de Armazenamento com KeyvaultEncryption, para suportar a rotação automática de chaves</span><span class="sxs-lookup"><span data-stu-id="89801-650">Make KeyVersion to optional when update Storage account with KeyvaultEncryption, to support key auto-rotation</span></span>
    - <span data-ttu-id="89801-651">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="89801-651">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="89801-652">Corrigida a remoção de falha do Diretório de Ficheiros do Azure com o pipeline</span><span class="sxs-lookup"><span data-stu-id="89801-652">Fixed remove Azure File Directory fail with pipeline</span></span>
    - <span data-ttu-id="89801-653">"Remove-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="89801-653">'Remove-AzStorageDirectory'</span></span>
* <span data-ttu-id="89801-654">Corrigido [#9880]: A definição do valor DefaultAction de NetWorkRule foi alterado para estar alinhado com o swagger.</span><span class="sxs-lookup"><span data-stu-id="89801-654">Fixed [#9880]: Change NetWorkRule DefaultAction value defination to align with swagger.</span></span>
    - <span data-ttu-id="89801-655">"Update-AzStorageAccountNetworkRuleSet"</span><span class="sxs-lookup"><span data-stu-id="89801-655">'Update-AzStorageAccountNetworkRuleSet'</span></span>
    - <span data-ttu-id="89801-656">"Get-AzStorageAccountNetworkRuleSet"</span><span class="sxs-lookup"><span data-stu-id="89801-656">'Get-AzStorageAccountNetworkRuleSet'</span></span>
* <span data-ttu-id="89801-657">Corrigido [#11624]: Ignorar regras duplicadas ao adicionar NetworkRules, para evitar falhas de servidores</span><span class="sxs-lookup"><span data-stu-id="89801-657">Fixed [#11624]: Skip duplicated rules when add NetworkRules, to avoid server failure</span></span>
    - <span data-ttu-id="89801-658">"Add-AzStorageAccountNetworkRule"</span><span class="sxs-lookup"><span data-stu-id="89801-658">'Add-AzStorageAccountNetworkRule'</span></span>
* <span data-ttu-id="89801-659">O SDK Microsoft.Azure.Cosmos.Table foi atualizado para 1.0.7</span><span class="sxs-lookup"><span data-stu-id="89801-659">Upgraded Microsoft.Azure.Cosmos.Table SDK to 1.0.7</span></span>
* <span data-ttu-id="89801-660">Foi adicionada uma mensagem de aviso para relembrar o utilizador para listar novamente com ContinuationToken apenas quando são devolvidos itens de peças na lista DataLake Gen2 Items,</span><span class="sxs-lookup"><span data-stu-id="89801-660">Added a warning message to remind user to list again with ContinuationToken when only part items are returned in list DataLake Gen2 Items,</span></span>
    - <span data-ttu-id="89801-661">"Get-AzDataLakeGen2ChildItem"</span><span class="sxs-lookup"><span data-stu-id="89801-661">'Get-AzDataLakeGen2ChildItem'</span></span>
* <span data-ttu-id="89801-662">Suportado para criar ou atualizar a conta de Armazenamento com a Autenticação do Active Directory Domain Service dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="89801-662">Supported to create or update Storage account with Azure Files Active Directory Domain Service Authentication</span></span>
    -  <span data-ttu-id="89801-663">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="89801-663">'New-AzStorageAccount'</span></span>
    -  <span data-ttu-id="89801-664">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="89801-664">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="89801-665">Suportado para os comandos "new" ou "list" de chaves de Kerberos da conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="89801-665">Supported to new or list Kerberos keys of Storage account</span></span>
    -  <span data-ttu-id="89801-666">"New-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="89801-666">'New-AzStorageAccountKey'</span></span>
    -  <span data-ttu-id="89801-667">"Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="89801-667">'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="89801-668">Suportada conta de Armazenamento de ativação pós-falha</span><span class="sxs-lookup"><span data-stu-id="89801-668">Supported failover Storage account</span></span>
    - <span data-ttu-id="89801-669">"Invoke-AzStorageAccountFailover"</span><span class="sxs-lookup"><span data-stu-id="89801-669">'Invoke-AzStorageAccountFailover'</span></span>
* <span data-ttu-id="89801-670">Ajuda de "Get-AzStorageBlobCopyState" atualizada</span><span class="sxs-lookup"><span data-stu-id="89801-670">Updated help of 'Get-AzStorageBlobCopyState'</span></span>
* <span data-ttu-id="89801-671">Ajuda de "Get-AzStorageFileCopyState" e "Start-AzStorageBlobCopy" atualizada</span><span class="sxs-lookup"><span data-stu-id="89801-671">Updated help of 'Get-AzStorageFileCopyState' and 'Start-AzStorageBlobCopy'</span></span>
* <span data-ttu-id="89801-672">Integração da biblioteca de cliente do Armazenamento v12 para cmdlets de Filas e Ficheiros</span><span class="sxs-lookup"><span data-stu-id="89801-672">Integrated Storage client library v12 to Queue and File cmdlets</span></span>
* <span data-ttu-id="89801-673">Alteração ao tipo de saída de CloudFile para AzureStorageFile; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="89801-673">Changed output type from CloudFile to AzureStorageFile, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="89801-674">"Get-AzStorageFile"</span><span class="sxs-lookup"><span data-stu-id="89801-674">'Get-AzStorageFile'</span></span>
    - <span data-ttu-id="89801-675">"Remove-AzStorageFile"</span><span class="sxs-lookup"><span data-stu-id="89801-675">'Remove-AzStorageFile'</span></span>
    - <span data-ttu-id="89801-676">"Get-AzStorageFileContent"</span><span class="sxs-lookup"><span data-stu-id="89801-676">'Get-AzStorageFileContent'</span></span>
    - <span data-ttu-id="89801-677">"Set-AzStorageFileContent"</span><span class="sxs-lookup"><span data-stu-id="89801-677">'Set-AzStorageFileContent'</span></span>
    - <span data-ttu-id="89801-678">"Start-AzStorageFileCopy"</span><span class="sxs-lookup"><span data-stu-id="89801-678">'Start-AzStorageFileCopy'</span></span>
* <span data-ttu-id="89801-679">Alteração ao tipo de saída de CloudFileDirectory para AzureStorageFileDirectory; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="89801-679">Changed output type from CloudFileDirectory to AzureStorageFileDirectory, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="89801-680">"New-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="89801-680">'New-AzStorageDirectory'</span></span>
    - <span data-ttu-id="89801-681">"Remove-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="89801-681">'Remove-AzStorageDirectory'</span></span>
* <span data-ttu-id="89801-682">Alteração ao tipo de saída de CloudFileShare para AzureStorageFileShare; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="89801-682">Changed output type from CloudFileShare to AzureStorageFileShare, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="89801-683">"Get-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="89801-683">'Get-AzStorageShare'</span></span>
    - <span data-ttu-id="89801-684">"New-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="89801-684">'New-AzStorageShare'</span></span>
    - <span data-ttu-id="89801-685">"Remove-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="89801-685">'Remove-AzStorageShare'</span></span>
* <span data-ttu-id="89801-686">Alteração ao tipo de saída de FileShareProperties para AzureStorageFileShare; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="89801-686">Changed output type from FileShareProperties to AzureStorageFileShare, the original output will become a sub child property of the new output</span></span>
    - <span data-ttu-id="89801-687">"Set-AzStorageShareQuota"</span><span class="sxs-lookup"><span data-stu-id="89801-687">'Set-AzStorageShareQuota'</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="89801-688">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="89801-688">Az.TrafficManager</span></span>
* <span data-ttu-id="89801-689">Corrigido o nome de perfil errado na saída verbosa de "DisableAzureTrafficManagerEndpoint"</span><span class="sxs-lookup"><span data-stu-id="89801-689">Fixed incorrect profile name in 'DisableAzureTrafficManagerEndpoint' verbose output</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="89801-690">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-690">Az.Websites</span></span>
* <span data-ttu-id="89801-691">Corrigido um erro ortográfico na ajuda de "Update-AzWebAppAccessRestrictionConfig".</span><span class="sxs-lookup"><span data-stu-id="89801-691">Fixed typo on help of 'Update-AzWebAppAccessRestrictionConfig'.</span></span>

## <a name="380---april-2020"></a><span data-ttu-id="89801-692">3.8.0 - Abril de 2020</span><span class="sxs-lookup"><span data-stu-id="89801-692">3.8.0 - April 2020</span></span>
### <a name="highlights-since-the-last-release"></a><span data-ttu-id="89801-693">Destaques desde a última versão</span><span class="sxs-lookup"><span data-stu-id="89801-693">Highlights since the last release</span></span>
* <span data-ttu-id="89801-694">Versões do Powershell suportadas pelo Az.Storage: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span><span class="sxs-lookup"><span data-stu-id="89801-694">PowerShell versions that Az.Storage supports: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="89801-695">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-695">Az.Accounts</span></span>
* <span data-ttu-id="89801-696">Atualização do URL de inquérito do Azure PowerShell em "Resolve-AzError" [#11507]</span><span class="sxs-lookup"><span data-stu-id="89801-696">Updated Azure PowerShell survey URL in 'Resolve-AzError' [#11507]</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="89801-697">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="89801-697">Az.ApiManagement</span></span>
* <span data-ttu-id="89801-698">Adicionado aviso de alteração interruptiva para a alteração de resultados de cmdlets de Ficheiro do Azure numa versão futura</span><span class="sxs-lookup"><span data-stu-id="89801-698">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="89801-699">Documentação atualizada de "Set-AzApiManagementGroup" para especificar o parâmetro GroupId</span><span class="sxs-lookup"><span data-stu-id="89801-699">'Set-AzApiManagementGroup' Updated documentation to specify the GroupId parameter</span></span>

#### <a name="azcdn"></a><span data-ttu-id="89801-700">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="89801-700">Az.Cdn</span></span>
* <span data-ttu-id="89801-701">Correção da apresentação do SKU de preços relacionados com ChinaCDN</span><span class="sxs-lookup"><span data-stu-id="89801-701">Fixed ChinaCDN related pricing SKU display</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="89801-702">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="89801-702">Az.CognitiveServices</span></span>
* <span data-ttu-id="89801-703">Suporte para Identidade, Encriptação, UserOwnedStorage</span><span class="sxs-lookup"><span data-stu-id="89801-703">Supported Identity, Encryption, UserOwnedStorage</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-704">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-704">Az.Compute</span></span>
* <span data-ttu-id="89801-705">Adicionado o cmdlet "Set-AzVmssOrchestrationServiceState".</span><span class="sxs-lookup"><span data-stu-id="89801-705">Added 'Set-AzVmssOrchestrationServiceState' cmdlet.</span></span>
* <span data-ttu-id="89801-706">"Get-AzVmss" com -InstanceView mostra os estados de OrchestrationService.</span><span class="sxs-lookup"><span data-stu-id="89801-706">'Get-AzVmss' with -InstanceView shows OrchestrationService states.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="89801-707">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="89801-707">Az.IotHub</span></span>
* <span data-ttu-id="89801-708">Gestão da configuração do dispositivo duplo de IoT. Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="89801-708">Manage IoT device twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="89801-709">"Get-AzIotHubDeviceTwin"</span><span class="sxs-lookup"><span data-stu-id="89801-709">'Get-AzIotHubDeviceTwin'</span></span>
    - <span data-ttu-id="89801-710">"Update-AzIotHubDeviceTwin"</span><span class="sxs-lookup"><span data-stu-id="89801-710">'Update-AzIotHubDeviceTwin'</span></span>
* <span data-ttu-id="89801-711">Adicionado cmdlet para invocar o método direto num dispositivo num hub IoT.</span><span class="sxs-lookup"><span data-stu-id="89801-711">Added cmdlet to invoke direct method on a device in an Iot Hub.</span></span>
* <span data-ttu-id="89801-712">Gestão da configuração do módulo duplo do dispositivo de IoT. Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="89801-712">Manage IoT device module twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="89801-713">"Get-AzIotHubModuleTwin"</span><span class="sxs-lookup"><span data-stu-id="89801-713">'Get-AzIotHubModuleTwin'</span></span>
    - <span data-ttu-id="89801-714">"Update-AzIotHubModuleTwin"</span><span class="sxs-lookup"><span data-stu-id="89801-714">'Update-AzIotHubModuleTwin'</span></span>
* <span data-ttu-id="89801-715">Gestão da configuração da gestão automática de dispositivos IoT em escala.</span><span class="sxs-lookup"><span data-stu-id="89801-715">Manage IoT automatic device management configuration at scale.</span></span> <span data-ttu-id="89801-716">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="89801-716">New cmdlets are:</span></span>
    - <span data-ttu-id="89801-717">"Add-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="89801-717">'Add-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="89801-718">"Get-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="89801-718">'Get-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="89801-719">"Remove-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="89801-719">'Remove-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="89801-720">"Set-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="89801-720">'Set-AzIotHubConfiguration'</span></span>
* <span data-ttu-id="89801-721">Adicionado cmdlet para invocar um método de módulo de periferia num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="89801-721">Added cmdlet to invoke an edge module method in an Iot Hub.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="89801-722">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="89801-722">Az.KeyVault</span></span>
* <span data-ttu-id="89801-723">Adicionado um novo cmdlet "Update-AzKeyVault" que pode permitir a eliminação recuperável e a proteção contra remoções num cofre</span><span class="sxs-lookup"><span data-stu-id="89801-723">Added a new cmdlet 'Update-AzKeyVault' that can enable soft delete and purge protection on a vault</span></span>
* <span data-ttu-id="89801-724">Adicionado suporte para Microsoft.PowerShell.SecretManagement [#11178]</span><span class="sxs-lookup"><span data-stu-id="89801-724">Added support to Microsoft.PowerShell.SecretManagement [#11178]</span></span>
* <span data-ttu-id="89801-725">Correção do erro nos exemplos de "Remove-AzKeyVaultManagedStorageSasDefinition" [#11479]</span><span class="sxs-lookup"><span data-stu-id="89801-725">Fixed error in the examples of 'Remove-AzKeyVaultManagedStorageSasDefinition' [#11479]</span></span>
* <span data-ttu-id="89801-726">Adicionado suporte para o ponto final privado</span><span class="sxs-lookup"><span data-stu-id="89801-726">Added support to private endpoint</span></span>

#### <a name="azmaintenance"></a><span data-ttu-id="89801-727">Az.Maintenance</span><span class="sxs-lookup"><span data-stu-id="89801-727">Az.Maintenance</span></span>
* <span data-ttu-id="89801-728">Publicação da versão de lançamento dos cmdlets de Manutenção para Disponibilidade Geral</span><span class="sxs-lookup"><span data-stu-id="89801-728">Publishing release version of Maintenance cmdlets for GA</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="89801-729">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="89801-729">Az.Monitor</span></span>
* <span data-ttu-id="89801-730">Adicionados cmdlets para o âmbito de ligação privada</span><span class="sxs-lookup"><span data-stu-id="89801-730">Added cmdlets for private link scope</span></span>
    - <span data-ttu-id="89801-731">"Get-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="89801-731">'Get-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="89801-732">"Remove-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="89801-732">'Remove-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="89801-733">"New-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="89801-733">'New-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="89801-734">"Update-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="89801-734">'Update-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="89801-735">"Get-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="89801-735">'Get-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="89801-736">"New-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="89801-736">'New-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="89801-737">"Remove-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="89801-737">'Remove-AzInsightsPrivateLinkScopedResource'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-738">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-738">Az.Network</span></span>
* <span data-ttu-id="89801-739">Atualização dos cmdlets para permitir a ligação num IP privado para o Gateway de Rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="89801-739">Updated cmdlets to enable connection on private IP for Virtual Network Gateway.</span></span>
    - <span data-ttu-id="89801-740">"New-AzVirtualNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="89801-740">'New-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="89801-741">"Set-AzVirtualNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="89801-741">'Set-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="89801-742">"New-AzVirtualNetworkGatewayConnection"</span><span class="sxs-lookup"><span data-stu-id="89801-742">'New-AzVirtualNetworkGatewayConnection'</span></span>
    - <span data-ttu-id="89801-743">"Set-AzVirtualNetworkGatewayConnection"</span><span class="sxs-lookup"><span data-stu-id="89801-743">'Set-AzVirtualNetworkGatewayConnection'</span></span>
* <span data-ttu-id="89801-744">Atualização dos cmdlets para permitir LocalNetworkGateways e VpnSites com base em FQDN</span><span class="sxs-lookup"><span data-stu-id="89801-744">Updated cmdlets to enable FQDN based LocalNetworkGateways and VpnSites</span></span>
    - <span data-ttu-id="89801-745">"New-AzLocalNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="89801-745">'New-AzLocalNetworkGateway'</span></span>
    - <span data-ttu-id="89801-746">"New-AzVpnSiteLink"</span><span class="sxs-lookup"><span data-stu-id="89801-746">'New-AzVpnSiteLink'</span></span>
* <span data-ttu-id="89801-747">Adicionado suporte para a família de endereços IPv6 em ExpressRouteCircuitConnectionConfig (Alcance Global)</span><span class="sxs-lookup"><span data-stu-id="89801-747">Added support for IPv6 address family in ExpressRouteCircuitConnectionConfig (Global Reach)</span></span>
    - <span data-ttu-id="89801-748">Adicionado "Set-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="89801-748">Added 'Set-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="89801-749">permite a definição de todas as propriedades existentes, incluindo o IPv6CircuitConnectionProperties</span><span class="sxs-lookup"><span data-stu-id="89801-749">allows setting of all the existing properties including the IPv6CircuitConnectionProperties</span></span>
    - <span data-ttu-id="89801-750">Atualização de "Add-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="89801-750">Updated 'Add-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="89801-751">Adicionado outro parâmetro opcional AddressPrefixType para especificar a família de endereços do prefixo de endereço</span><span class="sxs-lookup"><span data-stu-id="89801-751">Added another optional parameter AddressPrefixType to specify the address family of address prefix</span></span>
* <span data-ttu-id="89801-752">Atualização dos cmdlets para permitir a definição do Tempo Limite de DPD nas Ligações do Gateway de Rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="89801-752">Updated cmdlets to enable setting of DPD Timeout on Virtual Network Gateway Connections.</span></span>
    - <span data-ttu-id="89801-753">New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="89801-753">New-AzVirtualNetworkGatewayConnection</span></span>
    - <span data-ttu-id="89801-754">Set-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="89801-754">Set-AzVirtualNetworkGatewayConnection</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="89801-755">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="89801-755">Az.PolicyInsights</span></span>
* <span data-ttu-id="89801-756">Adicionado o cmdlet "Start-AzPolicyComplianceScan" para acionar análises de conformidade de políticas</span><span class="sxs-lookup"><span data-stu-id="89801-756">Added 'Start-AzPolicyComplianceScan' cmdlet for triggering policy compliance scans</span></span>
* <span data-ttu-id="89801-757">Adição de definição de políticas, definição de conjuntos e versões de atribuição ao resultado de "Get-AzPolicyState"</span><span class="sxs-lookup"><span data-stu-id="89801-757">Added policy definition, set definition, and assignment versions to 'Get-AzPolicyState' output</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="89801-758">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="89801-758">Az.ServiceFabric</span></span>
* <span data-ttu-id="89801-759">Melhorias da formatação e usabilidade do código dos exemplos de "New-AzServiceFabricCluster"</span><span class="sxs-lookup"><span data-stu-id="89801-759">Improved code formatting and usability of 'New-AzServiceFabricCluster' examples</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-760">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-760">Az.Sql</span></span>
* <span data-ttu-id="89801-761">Adicionados os cmdlets "Get-AzSqlInstanceOperation" e "Stop-AzSqlInstanceOperation"</span><span class="sxs-lookup"><span data-stu-id="89801-761">Added cmdlets 'Get-AzSqlInstanceOperation' and 'Stop-AzSqlInstanceOperation'</span></span>
* <span data-ttu-id="89801-762">Suporte de auditorias a uma conta de armazenamento numa VNet.</span><span class="sxs-lookup"><span data-stu-id="89801-762">Supported auditing to a storage account in VNet.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-763">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-763">Az.Storage</span></span>
* <span data-ttu-id="89801-764">Adicionado aviso de alteração interruptiva para a alteração de resultados de cmdlets de Ficheiro do Azure numa versão futura</span><span class="sxs-lookup"><span data-stu-id="89801-764">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="89801-765">Suportado novo SkuName StandardGZRS, StandardRAGZRS ao criar/atualizar a Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="89801-765">Supported new SkuName StandardGZRS, StandardRAGZRS when create/update Storage account</span></span>
    - <span data-ttu-id="89801-766">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="89801-766">'New-AzStorageAccount'</span></span>
    - <span data-ttu-id="89801-767">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="89801-767">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="89801-768">Suportado o DataLake Gen2</span><span class="sxs-lookup"><span data-stu-id="89801-768">Supported DataLake Gen2</span></span>
    - <span data-ttu-id="89801-769">"New-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="89801-769">'New-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="89801-770">"Get-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="89801-770">'Get-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="89801-771">"Get-AzDataLakeGen2ChildItem"</span><span class="sxs-lookup"><span data-stu-id="89801-771">'Get-AzDataLakeGen2ChildItem'</span></span>
    - <span data-ttu-id="89801-772">"Move-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="89801-772">'Move-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="89801-773">"Set-AzDataLakeGen2ItemAclObject"</span><span class="sxs-lookup"><span data-stu-id="89801-773">'Set-AzDataLakeGen2ItemAclObject'</span></span>
    - <span data-ttu-id="89801-774">"Update-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="89801-774">'Update-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="89801-775">"Get-AzDataLakeGen2ItemContent"</span><span class="sxs-lookup"><span data-stu-id="89801-775">'Get-AzDataLakeGen2ItemContent'</span></span>
    - <span data-ttu-id="89801-776">"Remove-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="89801-776">'Remove-AzDataLakeGen2Item'</span></span>

## <a name="0100-preview---april-2020"></a><span data-ttu-id="89801-777">0.10.0-preview - Abril de 2020</span><span class="sxs-lookup"><span data-stu-id="89801-777">0.10.0-preview - April 2020</span></span>
### <a name="general"></a><span data-ttu-id="89801-778">Geral</span><span class="sxs-lookup"><span data-stu-id="89801-778">General</span></span>
* <span data-ttu-id="89801-779">Os módulos Az já estão disponíveis em pré-visualização no Azure Stack Hub.</span><span class="sxs-lookup"><span data-stu-id="89801-779">Az modules is now available in preview on Azure Stack Hub.</span></span> <span data-ttu-id="89801-780">Isto permite a compatibilidade entre plataformas diferentes com o Linux e macOS.</span><span class="sxs-lookup"><span data-stu-id="89801-780">This allows for cross-platform compatibility with Linux and macOs.</span></span> <span data-ttu-id="89801-781">Agora, o Azure Stack Hub suporta o PowerShell Core com os módulos Az. Obtenha mais informações [aqui](https://aka.ms/az4AzureStack)</span><span class="sxs-lookup"><span data-stu-id="89801-781">Azure Stack Hub now supports PowerShell core with the Az modules, more information [here](https://aka.ms/az4AzureStack)</span></span>
* <span data-ttu-id="89801-782">Os módulos Az suportam o perfil 2019-03-01-hybrid:</span><span class="sxs-lookup"><span data-stu-id="89801-782">Az modules support profile 2019-03-01-hybrid:</span></span>
  - <span data-ttu-id="89801-783">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="89801-783">Az.Billing</span></span>
  - <span data-ttu-id="89801-784">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-784">Az.Compute</span></span>
  - <span data-ttu-id="89801-785">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="89801-785">Az.DataBoxEdge</span></span>
  - <span data-ttu-id="89801-786">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="89801-786">Az.EventHub</span></span>
  - <span data-ttu-id="89801-787">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="89801-787">Az.IotHub</span></span>
  - <span data-ttu-id="89801-788">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="89801-788">Az.KeyVault</span></span>
  - <span data-ttu-id="89801-789">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="89801-789">Az.Monitor</span></span>
  - <span data-ttu-id="89801-790">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-790">Az.Network</span></span>
  - <span data-ttu-id="89801-791">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-791">Az.Resources</span></span>
  - <span data-ttu-id="89801-792">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-792">Az.Storage</span></span>
  - <span data-ttu-id="89801-793">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-793">Az.Websites</span></span>
* <span data-ttu-id="89801-794">Foram introduzidos três novos módulos do PowerShell para Az que funcionam com o Azure Stack Hub. São eles o Az.Databox, Az.IotHub e Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="89801-794">Three new PowerShell modules for az have been introduced that work with Azure Stack Hub, which are Az.Databox, Az.IotHub, and Az.EventHub</span></span>
* <span data-ttu-id="89801-795">Os comandos permanecem sensivelmente iguais, com pequenas alterações como, por exemplo, a alteração do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="89801-795">Commands remain relatively the same, with minor changes such as changing AzureRM to Az</span></span>
* <span data-ttu-id="89801-796">Veja uma ligação atualizada à documentação do PowerShell para o Azure Stack Hub [aqui](https://aka.ms/InstallASHPowerShell)</span><span class="sxs-lookup"><span data-stu-id="89801-796">Updated link to PowerShell documentation for Azure Stack Hub can be found [here](https://aka.ms/InstallASHPowerShell)</span></span>

## <a name="370---march-2020"></a><span data-ttu-id="89801-797">3.7.0 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="89801-797">3.7.0 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="89801-798">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-798">Az.Accounts</span></span>
* <span data-ttu-id="89801-799">Foram corrigidos os parâmetros "Get-AzTenant"/"Get-AzDefault"/"Set-AzDefault" que emitiam uma NullReferenceException quando a sessão não estava iniciada [#10292]</span><span class="sxs-lookup"><span data-stu-id="89801-799">Fixed 'Get-AzTenant'/'Get-AzDefault'/'Set-AzDefault' throw NullReferenceException when not login [#10292]</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-800">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-800">Az.Compute</span></span>
* <span data-ttu-id="89801-801">Foram adicionados os seguintes parâmetros ao cmdlet "New-AzDiskConfig":</span><span class="sxs-lookup"><span data-stu-id="89801-801">Added the following parameters to 'New-AzDiskConfig' cmdlet:</span></span>
    - <span data-ttu-id="89801-802">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span><span class="sxs-lookup"><span data-stu-id="89801-802">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span></span>
* <span data-ttu-id="89801-803">A propriedade Encryption foi permitida para o parâmetro Target do cmdlet "New-AzGalleryImageVersion".</span><span class="sxs-lookup"><span data-stu-id="89801-803">Allowed Encryption property to Target parameter of 'New-AzGalleryImageVersion' cmdlet.</span></span>
* <span data-ttu-id="89801-804">Foi corrigido o problema de tempDisk para os cmdlets "Set-AzVmss" -Reimage e "Invoke-AzVMReimage".</span><span class="sxs-lookup"><span data-stu-id="89801-804">Fixed tempDisk issue for 'Set-AzVmss' -Reimage and 'Invoke-AzVMReimage' cmdlets.</span></span> <span data-ttu-id="89801-805">[#11354]</span><span class="sxs-lookup"><span data-stu-id="89801-805">[#11354]</span></span>
* <span data-ttu-id="89801-806">Foi adicionado suporte aos cmdlets abaixo para a nova Extensão SAP</span><span class="sxs-lookup"><span data-stu-id="89801-806">Added support to below cmdlets for new SAP Extension</span></span>
    - <span data-ttu-id="89801-807">"Set-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="89801-807">'Set-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="89801-808">"Get-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="89801-808">'Get-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="89801-809">"Remove-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="89801-809">'Remove-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="89801-810">"Update-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="89801-810">'Update-AzVMAEMExtension'</span></span>
* <span data-ttu-id="89801-811">Foram corrigidos os erros em exemplos do documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="89801-811">Fixed errors in examples of help document</span></span>
* <span data-ttu-id="89801-812">É apresentado o valor de cadeia exato para o PowerState da VM no formato de tabela.</span><span class="sxs-lookup"><span data-stu-id="89801-812">Showed the exact string value for VM PowerState in the table format.</span></span>
* <span data-ttu-id="89801-813">"New-AzVmssConfig": foi corrigida a serialização da propriedade AutomaticRepairs quando a opção SinglePlacementGroup está desativada.</span><span class="sxs-lookup"><span data-stu-id="89801-813">'New-AzVmssConfig': fixed serialization of AutomaticRepairs property when SinglePlacementGroup is disabled.</span></span> <span data-ttu-id="89801-814">[#11257]</span><span class="sxs-lookup"><span data-stu-id="89801-814">[#11257]</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="89801-815">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="89801-815">Az.DataFactory</span></span>
* <span data-ttu-id="89801-816">Atualização da versão do SDK .Net do ADF para 4.8.0</span><span class="sxs-lookup"><span data-stu-id="89801-816">Updated ADF .Net SDK version to 4.8.0</span></span>
* <span data-ttu-id="89801-817">Foram adicionados parâmetros opcionais ao comando "Invoke-AzDataFactoryV2Pipeline" para suportar uma nova execução</span><span class="sxs-lookup"><span data-stu-id="89801-817">Added optional parameters to 'Invoke-AzDataFactoryV2Pipeline' command to support rerun</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="89801-818">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="89801-818">Az.DataLakeStore</span></span>
* <span data-ttu-id="89801-819">Foi adicionada a descrição da alteração interruptiva para "Export-AzDataLakeStoreItem" e "Import-AzDataLakeStoreItem"</span><span class="sxs-lookup"><span data-stu-id="89801-819">Added breaking change description for 'Export-AzDataLakeStoreItem' and 'Import-AzDataLakeStoreItem'</span></span>
* <span data-ttu-id="89801-820">Foi adicionada a opção de codificação de bytes para "New-AzDataLakeStoreItem", "Add-AzDAtaLakeStoreItemContent" e "Get-AzDAtaLakeStoreItemContent"</span><span class="sxs-lookup"><span data-stu-id="89801-820">Added option of Byte encoding for 'New-AzDataLakeStoreItem', 'Add-AzDAtaLakeStoreItemContent', and 'Get-AzDAtaLakeStoreItemContent'</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="89801-821">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="89801-821">Az.HDInsight</span></span>
* <span data-ttu-id="89801-822">É suportada a versão de TLS mínima suportada ao criar o cluster.</span><span class="sxs-lookup"><span data-stu-id="89801-822">Supported specifying minimal supported TLS version when creating cluster.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="89801-823">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="89801-823">Az.IotHub</span></span>
* <span data-ttu-id="89801-824">Foi adicionado suporte para gerir as definições distribuídas por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="89801-824">Added support to manage distributed settings per-device.</span></span> <span data-ttu-id="89801-825">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="89801-825">New Cmdlets are:</span></span>
    - <span data-ttu-id="89801-826">"Get-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="89801-826">'Get-AzIotHubDistributedTracing'</span></span>
    - <span data-ttu-id="89801-827">"Set-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="89801-827">'Set-AzIotHubDistributedTracing'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="89801-828">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="89801-828">Az.KeyVault</span></span>
* <span data-ttu-id="89801-829">Foram adicionados os atributos da alteração interruptiva a "New-AzKeyVault"</span><span class="sxs-lookup"><span data-stu-id="89801-829">Added breaking change attributes to 'New-AzKeyVault'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="89801-830">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="89801-830">Az.Monitor</span></span>
* <span data-ttu-id="89801-831">Foi atualizada a documentação de "New-AzScheduledQueryRuleLogMetricTrigger"</span><span class="sxs-lookup"><span data-stu-id="89801-831">Updated documentation for 'New-AzScheduledQueryRuleLogMetricTrigger'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-832">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-832">Az.Network</span></span>
* <span data-ttu-id="89801-833">Foram atualizados os cmdlets para permitir VirtualHubVnetConnections entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="89801-833">Updated cmdlets to allow cross-tenant VirtualHubVnetConnections</span></span>
    - <span data-ttu-id="89801-834">"New-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="89801-834">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="89801-835">"Update-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="89801-835">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="89801-836">"New-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="89801-836">'New-AzVirtualHub'</span></span>
    - <span data-ttu-id="89801-837">"Update-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="89801-837">'Update-AzVirtualHub'</span></span>
* <span data-ttu-id="89801-838">Foi removida a dependência do SDK do SQL Management</span><span class="sxs-lookup"><span data-stu-id="89801-838">Removed Sql Management SDK dependency</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="89801-839">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="89801-839">Az.PolicyInsights</span></span>
* <span data-ttu-id="89801-840">Mensagens de erro melhoradas</span><span class="sxs-lookup"><span data-stu-id="89801-840">Improved error messages</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-841">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-841">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-842">O Azure Site Recovery adicionou suporte para nova proteção e atualização das propriedades de VM para Máquinas Virtuais encriptadas em disco do Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-842">Azure Site Recovery added support for doing reprotect and updated vm properties for Azure disk encrypted Virtual Machines.</span></span>
* <span data-ttu-id="89801-843">Foi adicionada monitorização DR das propriedades VmwareToAzure ao Azure Site Recovery</span><span class="sxs-lookup"><span data-stu-id="89801-843">Added Azure Site Recovery VmwareToAzure properties DR monitoring</span></span>
* <span data-ttu-id="89801-844">O Azure Backup adicionou suporte para repetir a atualização de políticas para itens falhados.</span><span class="sxs-lookup"><span data-stu-id="89801-844">Azure Backup added support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="89801-845">O Azure Backup adicionou suporte para definições de exclusão do disco durante a cópia de segurança e o restauro.</span><span class="sxs-lookup"><span data-stu-id="89801-845">Azure Backup Added support for disk exclusion settings during backup and restore.</span></span>
* <span data-ttu-id="89801-846">O Azure Backup adicionou suporte para restaurar vários ficheiros/pastas no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="89801-846">Azure Backup Added Support for Restoring Multiple files/folders in AzureFileShare</span></span>
* <span data-ttu-id="89801-847">O Azure Backup adicionou suporte para o Resourcegroup especificado pelo utilizador durante a atualização da Política IaasVM</span><span class="sxs-lookup"><span data-stu-id="89801-847">Azure Backup Added support for User-specified Resourcegroup support while updating IaasVM Policy</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-848">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-848">Az.Resources</span></span>
* <span data-ttu-id="89801-849">Foi corrigido o parâmetro "Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType" para utilizar a apiVersion real dos recursos em vez da apiVersion predefinida [#11267]</span><span class="sxs-lookup"><span data-stu-id="89801-849">Fixed 'Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType' to use actual apiVersion of resources instead of default apiVersion [#11267]</span></span>
* <span data-ttu-id="89801-850">Foi adicionado o registo de correlationId para cenários de erro</span><span class="sxs-lookup"><span data-stu-id="89801-850">Added correlationId logging for error scenarios</span></span>
* <span data-ttu-id="89801-851">Pequena alteração à documentação referente a "Get-AzResourceLock".</span><span class="sxs-lookup"><span data-stu-id="89801-851">Small documentation change to 'Get-AzResourceLock'.</span></span> <span data-ttu-id="89801-852">Exemplo adicionado.</span><span class="sxs-lookup"><span data-stu-id="89801-852">Added example.</span></span>
* <span data-ttu-id="89801-853">Aspas com caráter de escape no valor de parâmetro "Get-AzADUser" [#11317]</span><span class="sxs-lookup"><span data-stu-id="89801-853">Escaped single quote in parameter value of 'Get-AzADUser' [#11317]</span></span>
* <span data-ttu-id="89801-854">Foram adicionados novos cmdlets aos Scripts de Implementação ("Get-AzDeploymentScript", "Get-AzDeploymentScriptLog", "Save-AzDeploymentScriptLog", "Remove-AzDeploymentScript")</span><span class="sxs-lookup"><span data-stu-id="89801-854">Added new cmdlets for Deployment Scripts ('Get-AzDeploymentScript', 'Get-AzDeploymentScriptLog', 'Save-AzDeploymentScriptLog', 'Remove-AzDeploymentScript')</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-855">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-855">Az.Sql</span></span>
* <span data-ttu-id="89801-856">Foi adicionado um parâmetro secundário legível a "Invoke-AzSqlDatabaseFailover"</span><span class="sxs-lookup"><span data-stu-id="89801-856">Added readable secondary parameter to 'Invoke-AzSqlDatabaseFailover'</span></span>
* <span data-ttu-id="89801-857">Foi adicionado o cmdlet "Disable-AzSqlServerActiveDirectoryOnlyAuthentication"</span><span class="sxs-lookup"><span data-stu-id="89801-857">Added cmdlet 'Disable-AzSqlServerActiveDirectoryOnlyAuthentication'</span></span>
* <span data-ttu-id="89801-858">Classificação de sensibilidade guardada ao classificar as colunas na base de dados.</span><span class="sxs-lookup"><span data-stu-id="89801-858">Saved sensitivity rank when classifying columns in the database.</span></span>

#### <a name="azsupport"></a><span data-ttu-id="89801-859">Az.Support</span><span class="sxs-lookup"><span data-stu-id="89801-859">Az.Support</span></span>
* <span data-ttu-id="89801-860">Disponibilidade geral do módulo "Az.Support"</span><span class="sxs-lookup"><span data-stu-id="89801-860">General availability of 'Az.Support' module</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="89801-861">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-861">Az.Websites</span></span>
* <span data-ttu-id="89801-862">Foi adicionado suporte para utilizar Regras de Encaminhamento de Tráfego webapp através dos novos cmdlets abaixo</span><span class="sxs-lookup"><span data-stu-id="89801-862">Added support for working with webapp Traffic Routing Rules via below new cmdlets</span></span>
    - <span data-ttu-id="89801-863">"Get-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="89801-863">'Get-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="89801-864">"Update-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="89801-864">'Update-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="89801-865">"Add-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="89801-865">'Add-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="89801-866">"Remove-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="89801-866">'Remove-AzWebAppTrafficRouting'</span></span>

## <a name="361---march-2020"></a><span data-ttu-id="89801-867">3.6.1 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="89801-867">3.6.1 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="89801-868">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-868">Az.Accounts</span></span>
* <span data-ttu-id="89801-869">Abrir a página de inquérito do Azure PowerShell em "Send-Feedback" [#11020]</span><span class="sxs-lookup"><span data-stu-id="89801-869">Open Azure PowerShell survey page in 'Send-Feedback' [#11020]</span></span>
* <span data-ttu-id="89801-870">Apresentar o URL de inquérito do Azure PowerShell em "Resolve-Error" [#11021]</span><span class="sxs-lookup"><span data-stu-id="89801-870">Display Azure PowerShell survey URL in 'Resolve-Error' [#11021]</span></span>
* <span data-ttu-id="89801-871">Adicionada versão de Az em UserAgent</span><span class="sxs-lookup"><span data-stu-id="89801-871">Added Az version in UserAgent</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="89801-872">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="89801-872">Az.ApiManagement</span></span>
* <span data-ttu-id="89801-873">Adicionado suporte para a obtenção e configuração do Domínio Personalizado no Ponto Final do DeveloperPortal [#11007]</span><span class="sxs-lookup"><span data-stu-id="89801-873">Added support for retrieving and configuring Custom Domain on the DeveloperPortal Endpoint [#11007]</span></span>
* <span data-ttu-id="89801-874">"Export-AzApiManagementApi" Adicionado suporte para a transferência da definição da API no formato JSON [#9987]</span><span class="sxs-lookup"><span data-stu-id="89801-874">'Export-AzApiManagementApi' Added support for downloading Api Definition in Json format [#9987]</span></span>
* <span data-ttu-id="89801-875">"Import-AzApiManagementApi" Adicionado suporte para a importação da definição de OpenApi 3.0 a partir de documento JSON</span><span class="sxs-lookup"><span data-stu-id="89801-875">'Import-AzApiManagementApi' Added support for importing OpenApi 3.0 definition from Json document</span></span>
* <span data-ttu-id="89801-876">"New-AzApiManagementIdentityProvider" e "Set-AzApiManagementIdentityProvider" Adicionado suporte para a configuração de "Inquilino de Início de Sessão" para Fornecedor de AAD B2C [#9784]</span><span class="sxs-lookup"><span data-stu-id="89801-876">'New-AzApiManagementIdentityProvider' and 'Set-AzApiManagementIdentityProvider' Added support for configuring 'Signin Tenant' for AAD B2C Provider [#9784]</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="89801-877">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="89801-877">Az.DataLakeStore</span></span>
* <span data-ttu-id="89801-878">Adicionada referência a System.Buffers explicitamente em csproj e psd1.</span><span class="sxs-lookup"><span data-stu-id="89801-878">Added reference to System.Buffers explicitly in csproj and psd1.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="89801-879">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="89801-879">Az.IotHub</span></span>
* <span data-ttu-id="89801-880">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="89801-880">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="89801-881">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="89801-881">New Cmdlets are:</span></span>
    - <span data-ttu-id="89801-882">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="89801-882">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="89801-883">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="89801-883">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="89801-884">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="89801-884">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="89801-885">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="89801-885">'Set-AzIotHubDevice'</span></span>
* <span data-ttu-id="89801-886">Adicionado suporte para a gestão de módulos num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="89801-886">Added support to manage modules on a target Iot device in an Iot Hub.</span></span> <span data-ttu-id="89801-887">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="89801-887">New Cmdlets are:</span></span>
    - <span data-ttu-id="89801-888">"Add-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="89801-888">'Add-AzIotHubModule'</span></span>
    - <span data-ttu-id="89801-889">"Get-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="89801-889">'Get-AzIotHubModule'</span></span>
    - <span data-ttu-id="89801-890">"Remove-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="89801-890">'Remove-AzIotHubModule'</span></span>
    - <span data-ttu-id="89801-891">"Set-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="89801-891">'Set-AzIotHubModule'</span></span>
* <span data-ttu-id="89801-892">Adicionado cmdlet para obter a cadeia de ligação de um dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="89801-892">Added cmdlet to get the connection string of a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="89801-893">Adicionado cmdlet para obter a cadeia de ligação de um módulo num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="89801-893">Added cmdlet to get the connection string of a module on a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="89801-894">Adicionado suporte para obter/definir dispositivo principal de um dispositivo IoT.</span><span class="sxs-lookup"><span data-stu-id="89801-894">Added support to get/set parent device of an IoT device.</span></span> <span data-ttu-id="89801-895">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="89801-895">New Cmdlets are:</span></span>
    - <span data-ttu-id="89801-896">"Get-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="89801-896">'Get-AzIotHubDeviceParent'</span></span>
    - <span data-ttu-id="89801-897">"Set-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="89801-897">'Set-AzIotHubDeviceParent'</span></span>
* <span data-ttu-id="89801-898">Adicionado suporte para gerir relações principal-subordinado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="89801-898">Added support to manage device parent-child relationship.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="89801-899">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="89801-899">Az.Monitor</span></span>
* <span data-ttu-id="89801-900">Corrigido o valor de saída de "Get-AzMetricDefinition" [#9714]</span><span class="sxs-lookup"><span data-stu-id="89801-900">Fixed output value for 'Get-AzMetricDefinition' [#9714]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-901">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-901">Az.Network</span></span>
* <span data-ttu-id="89801-902">Sdk Sql Management atualizado.</span><span class="sxs-lookup"><span data-stu-id="89801-902">Updated Sql Management SDK.</span></span>
* <span data-ttu-id="89801-903">Corrigido um problema de diferença de nomes na classe PrivateLinkServiceConnectionState.</span><span class="sxs-lookup"><span data-stu-id="89801-903">Fixed a naming-difference issue in PrivateLinkServiceConnectionState class.</span></span>
    - <span data-ttu-id="89801-904">Mapeamento do campo ActionsRequired para ActionRequired.</span><span class="sxs-lookup"><span data-stu-id="89801-904">Mapping the field ActionsRequired to ActionRequired.</span></span>
* <span data-ttu-id="89801-905">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="89801-905">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-906">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-906">Az.Resources</span></span>
* <span data-ttu-id="89801-907">Correção para erro de referência nula em "Get-AzRoleAssignment"</span><span class="sxs-lookup"><span data-stu-id="89801-907">Fixed for null reference bug in 'Get-AzRoleAssignment'</span></span>
* <span data-ttu-id="89801-908">Comutadores "-Force" e "-PassThru" marcados como opcionais em "Remove-AzADGroup" [#10849]</span><span class="sxs-lookup"><span data-stu-id="89801-908">Marked switch '-Force' and '-PassThru' optional in 'Remove-AzADGroup' [#10849]</span></span>
* <span data-ttu-id="89801-909">Corrigido problema em que "MailNickname" não devolve "Remove-AzADGroup" [#11167]</span><span class="sxs-lookup"><span data-stu-id="89801-909">Fixed issue that 'MailNickname' doesn't return in 'Remove-AzADGroup' [#11167]</span></span>
* <span data-ttu-id="89801-910">Corrigido problema em que a operação de pipe "Remove-AzADGroup" não funciona [#11171]</span><span class="sxs-lookup"><span data-stu-id="89801-910">Fixed issue that 'Remove-AzADGroup' pipe operation doesn't work [#11171]</span></span>
* <span data-ttu-id="89801-911">Correção para erro de referência nula em GetAzureRoleAssignmentCommand</span><span class="sxs-lookup"><span data-stu-id="89801-911">Fixed for null reference bug in GetAzureRoleAssignmentCommand</span></span>
* <span data-ttu-id="89801-912">Adicionados atributos de alterações interruptivas para futuras alterações a cmdlets de política</span><span class="sxs-lookup"><span data-stu-id="89801-912">Added breaking change attributes for upcoming changes to policy cmdlets</span></span>
* <span data-ttu-id="89801-913">"Get-AzResourceGroup" atualizado para realizar filtragem de etiqueta de grupo de recursos no lado do servidor</span><span class="sxs-lookup"><span data-stu-id="89801-913">Updated 'Get-AzResourceGroup' to perform resource group tag filtering on server-side</span></span>
* <span data-ttu-id="89801-914">Cmdlets Tag alargados para accept -ResourceId</span><span class="sxs-lookup"><span data-stu-id="89801-914">Extended Tag cmdlets to accept -ResourceId</span></span>
    - <span data-ttu-id="89801-915">Get-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="89801-915">Get-AzTag -ResourceId</span></span>
    - <span data-ttu-id="89801-916">New-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="89801-916">New-AzTag -ResourceId</span></span>
    - <span data-ttu-id="89801-917">Remove-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="89801-917">Remove-AzTag -ResourceId</span></span>
* <span data-ttu-id="89801-918">Adicionado cmdlet Tag novo</span><span class="sxs-lookup"><span data-stu-id="89801-918">Added new Tag cmdlet</span></span>
    - <span data-ttu-id="89801-919">Update-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="89801-919">Update-AzTag -ResourceId</span></span>
* <span data-ttu-id="89801-920">ScopedDeployment trazido de SDK 3.3.0</span><span class="sxs-lookup"><span data-stu-id="89801-920">Brought ScopedDeployment from SDK 3.3.0</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-921">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-921">Az.Sql</span></span>
* <span data-ttu-id="89801-922">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="89801-922">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="89801-923">Adicionado suporte para configuração de cópia de segurança de Retenção de Longo Prazo para Bases de Dados Geridas</span><span class="sxs-lookup"><span data-stu-id="89801-923">Added support for Long Term Retention backup configuration for Managed Databases</span></span>
    - <span data-ttu-id="89801-924">Política Get/Set numa base de dados gerida</span><span class="sxs-lookup"><span data-stu-id="89801-924">Get/Set LTR policy on a managed database</span></span>
    - <span data-ttu-id="89801-925">Obter cópia(s) de segurança LTR por base de dados gerida, por instância gerida ou por localização</span><span class="sxs-lookup"><span data-stu-id="89801-925">Get LTR backup(s) by managed database, managed instance, or by location</span></span>
    - <span data-ttu-id="89801-926">Remover uma cópia de segurança LTR</span><span class="sxs-lookup"><span data-stu-id="89801-926">Remove an LTR backup</span></span>
    - <span data-ttu-id="89801-927">Restaurar uma cópia de segurança LTR para criar uma base de dados gerida nova</span><span class="sxs-lookup"><span data-stu-id="89801-927">Restore an LTR backup to create a new managed database</span></span>
* <span data-ttu-id="89801-928">Adicionado MinimalTlsVersion a New-AzSqlServer e Set-AzSqlServer</span><span class="sxs-lookup"><span data-stu-id="89801-928">Added MinimalTlsVersion to New-AzSqlServer and Set-AzSqlServer</span></span>
* <span data-ttu-id="89801-929">Adicionado MinimalTlsVersion a New-AzSqlInstance e Set-AzSqlInstance</span><span class="sxs-lookup"><span data-stu-id="89801-929">Added MinimalTlsVersion to New-AzSqlInstance and Set-AzSqlInstance</span></span>
* <span data-ttu-id="89801-930">Versão de SDK SQL atualizada para Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-930">Bumped SQL SDK version for Az.Network</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-931">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-931">Az.Storage</span></span>
* <span data-ttu-id="89801-932">AllowProtectedAppendWrite suportada em ImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="89801-932">Supported AllowProtectedAppendWrite in ImmutabilityPolicy</span></span>
    - <span data-ttu-id="89801-933">"Set-AzRmStorageContainerImmutabilityPolicy"</span><span class="sxs-lookup"><span data-stu-id="89801-933">'Set-AzRmStorageContainerImmutabilityPolicy'</span></span>
* <span data-ttu-id="89801-934">Adicionada uma mensagem de aviso de alteração interruptiva para alteração do tipo AzureStorageTable numa futura versão</span><span class="sxs-lookup"><span data-stu-id="89801-934">Added breaking change warning message for AzureStorageTable type change in a future release</span></span>
    - <span data-ttu-id="89801-935">"New-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="89801-935">'New-AzStorageTable'</span></span>
    - <span data-ttu-id="89801-936">"Get-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="89801-936">'Get-AzStorageTable'</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="89801-937">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-937">Az.Websites</span></span>
* <span data-ttu-id="89801-938">Adicionado o parâmetro Tag para "New-AzAppServicePlan" e "Set-AzAppServicePlan"</span><span class="sxs-lookup"><span data-stu-id="89801-938">Added Tag parameter for 'New-AzAppServicePlan' and 'Set-AzAppServicePlan'</span></span>
* <span data-ttu-id="89801-939">Paragem da execução de cmdlet caso seja emitida uma exceção ao adicionar um domínio personalizado a um site</span><span class="sxs-lookup"><span data-stu-id="89801-939">Stop cmdlet execution if an exception is thrown when adding a custom domain to a website</span></span>
* <span data-ttu-id="89801-940">Adicionado suporte para a realização de operações para Serviços de Aplicações em grupos de recursos diferentes do Plano do Serviço de Aplicações</span><span class="sxs-lookup"><span data-stu-id="89801-940">Added support to perform operations for App Services not in the same resource group as the App Service Plan</span></span>
* <span data-ttu-id="89801-941">Aplicada restrição de acesso a WebApp/Função em diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="89801-941">Applied access restriction to WebApp/Function in different resource groups</span></span>
* <span data-ttu-id="89801-942">Corrigido problema para definir os nomes de anfitrião personalizados para WebAppSlots</span><span class="sxs-lookup"><span data-stu-id="89801-942">Fixed issue to set custom hostnames for WebAppSlots</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="89801-943">3.5.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="89801-943">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="89801-944">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="89801-944">Highlights since the last major release</span></span>
* <span data-ttu-id="89801-945">Telemetria do lado do cliente atualizada.</span><span class="sxs-lookup"><span data-stu-id="89801-945">Updated client side telemetry.</span></span>
* <span data-ttu-id="89801-946">O Az.IotHub adicionou cmdlets para suportar a gestão de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="89801-946">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="89801-947">O Az.SqlVirtualMachine adicionou cmdlets ao Serviço de Escuta do Grupo de Disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="89801-947">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="89801-948">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-948">Az.Accounts</span></span>
* <span data-ttu-id="89801-949">SubscriptionId, TenantId e tempo de execução adicionados aos dados de telemetria do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="89801-949">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="89801-950">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="89801-950">Az.Automation</span></span>
* <span data-ttu-id="89801-951">Foi corrigido o erro no Exemplo 1 na documentação de referência de "New-AzAutomationSoftwareUpdateConfiguration"</span><span class="sxs-lookup"><span data-stu-id="89801-951">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="89801-952">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="89801-952">Az.CognitiveServices</span></span>
* <span data-ttu-id="89801-953">SDK atualizado para a versão 7.0</span><span class="sxs-lookup"><span data-stu-id="89801-953">Updated SDK to 7.0</span></span>
* <span data-ttu-id="89801-954">Mensagem de erro melhorada quando o servidor responde ao corpo vazio</span><span class="sxs-lookup"><span data-stu-id="89801-954">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-955">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-955">Az.Compute</span></span>
* <span data-ttu-id="89801-956">Valor vazio permitido para ProximityPlacementGroupId durante a atualização</span><span class="sxs-lookup"><span data-stu-id="89801-956">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="89801-957">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="89801-957">Az.FrontDoor</span></span>
* <span data-ttu-id="89801-958">Cmdlet adicionado para obter definições de regras geridas que podem ser utilizadas na WAF</span><span class="sxs-lookup"><span data-stu-id="89801-958">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="89801-959">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="89801-959">Az.IotHub</span></span>
* <span data-ttu-id="89801-960">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="89801-960">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="89801-961">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="89801-961">New Cmdlets are:</span></span>
    - <span data-ttu-id="89801-962">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="89801-962">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="89801-963">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="89801-963">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="89801-964">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="89801-964">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="89801-965">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="89801-965">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="89801-966">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="89801-966">Az.KeyVault</span></span>
* <span data-ttu-id="89801-967">Texto duplicado fixo para Add-AzKeyVaultKey.md</span><span class="sxs-lookup"><span data-stu-id="89801-967">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="89801-968">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="89801-968">Az.Monitor</span></span>
* <span data-ttu-id="89801-969">Descrição fixa do cmdlet Get-AzLog.</span><span class="sxs-lookup"><span data-stu-id="89801-969">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="89801-970">Foi adicionado um novo parâmetro chamado ActionGroupId ao comando "New-AzMetricAlertRuleV2".</span><span class="sxs-lookup"><span data-stu-id="89801-970">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="89801-971">O utilizador pode fornecer ActionGroupId(string) ou ActionGorup(ActivityLogAlertActionGroup).</span><span class="sxs-lookup"><span data-stu-id="89801-971">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-972">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-972">Az.Network</span></span>
* <span data-ttu-id="89801-973">Foi adicionada uma nota de parâmetro adicional para o parâmetro "-EnableProxyProtocol" para o cmdlet "New-AzPrivateLinkService".</span><span class="sxs-lookup"><span data-stu-id="89801-973">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="89801-974">Exemplo de FilterData fixo em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="89801-974">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="89801-975">Exemplo de Captura de Pacotes adicionado para capturar todos os pacotes internos e externos em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="89801-975">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="89801-976">Política do Azure Firewall suportada em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="89801-976">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="89801-977">Não foram adicionados novos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="89801-977">No new cmdlets are added.</span></span> <span data-ttu-id="89801-978">Simplificação da restrição da política de firewall em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="89801-978">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-979">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-979">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-980">Suporte adicionado da funcionalidade Restaurar como ficheiros para Bases de Dados SQL.</span><span class="sxs-lookup"><span data-stu-id="89801-980">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-981">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-981">Az.Resources</span></span>
* <span data-ttu-id="89801-982">Cmdlets de implementação de modelos refatorizados</span><span class="sxs-lookup"><span data-stu-id="89801-982">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="89801-983">Foram adicionados novos cmdlets para gerir implementações no grupo de gestão: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="89801-983">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="89801-984">Foram adicionados novos cmdlets para gerir implementações no inquilino: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="89801-984">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="89801-985">Cmdlets \*-AzDeployment refatorizados para trabalhar especificamente no âmbito da subscrição</span><span class="sxs-lookup"><span data-stu-id="89801-985">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="89801-986">Foram criados aliases \*-AzSubscriptionDeployment para os cmdlets \*-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="89801-986">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="89801-987">"Update-AzADApplication" fixo quando o parâmetro "AvailableToOtherTenants" não está definido</span><span class="sxs-lookup"><span data-stu-id="89801-987">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="89801-988">ApplicationObjectWithoutCredentialParameterSet removido para evitar AmbiguousParameterSetException.</span><span class="sxs-lookup"><span data-stu-id="89801-988">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="89801-989">Ficheiros de ajuda regenerados</span><span class="sxs-lookup"><span data-stu-id="89801-989">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-990">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-990">Az.Sql</span></span>
* <span data-ttu-id="89801-991">Suporte adicionado para restauro para um ponto anterior no tempo entre subscrições nas Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="89801-991">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="89801-992">Suporte adicionado para alterar a geração de hardware das Instâncias Geridas de SQL existentes</span><span class="sxs-lookup"><span data-stu-id="89801-992">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="89801-993">Exemplos de ajuda "Update-AzSqlServerVulnerabilityAssessmentSetting" fixos: saída do parâmetro/propriedade - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="89801-993">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="89801-994">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="89801-994">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="89801-995">Cmdlets adicionados para o Serviço de Escuta do Grupo de Disponibilidade</span><span class="sxs-lookup"><span data-stu-id="89801-995">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="89801-996">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="89801-996">Az.StorageSync</span></span>
* <span data-ttu-id="89801-997">Conjuntos de carateres suportados atualizados em "Invoke-AzStorageSyncCompatibilityCheck".</span><span class="sxs-lookup"><span data-stu-id="89801-997">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="89801-998">3.4.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="89801-998">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="89801-999">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="89801-999">Highlights since the last major release</span></span>
* <span data-ttu-id="89801-1000">Versão inicial Az.CosmosDB 0.1.0 lançada</span><span class="sxs-lookup"><span data-stu-id="89801-1000">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="89801-1001">Foi adicionado suporte para Az.Network ConnectionMonitor V2</span><span class="sxs-lookup"><span data-stu-id="89801-1001">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="89801-1002">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-1002">Az.Accounts</span></span>
* <span data-ttu-id="89801-1003">Foi desativada a gravação automática de contexto quando AzureRmContext.json não está disponível</span><span class="sxs-lookup"><span data-stu-id="89801-1003">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="89801-1004">Atualização da referência ao Azure Powershell Common para a pré-visualização 1.3.5</span><span class="sxs-lookup"><span data-stu-id="89801-1004">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="89801-1005">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="89801-1005">Az.ApiManagement</span></span>
* <span data-ttu-id="89801-1006">**Get-AzApiManagementApiSchema** Foi corrigido ao obter Open-Api Schema associado a uma API   https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="89801-1006">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="89801-1007">**New-AzApiManagementProduct**\* e **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="89801-1007">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="89801-1008">Foi corrigida a documentação para https://github.com/Azure/azure-powershell/issues/10472</span><span class="sxs-lookup"><span data-stu-id="89801-1008">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="89801-1009">**Set-AzApiManagementApi** Exemplo adicionado para mostrar como atualizar o ServiceUrl com o cmdlet</span><span class="sxs-lookup"><span data-stu-id="89801-1009">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-1010">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-1010">Az.Compute</span></span>
* <span data-ttu-id="89801-1011">Foi limitado o número de estados de VM a 100 para evitar limitações quando Get-AzVM-Status é executado sem o nome da VM.</span><span class="sxs-lookup"><span data-stu-id="89801-1011">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="89801-1012">Foi adicionado o cmdlet Update-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="89801-1012">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="89801-1013">Foram adicionados os parâmetros EncryptionType e DiskEncryptionSetId aos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="89801-1013">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="89801-1014">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="89801-1014">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="89801-1015">Foi adicionado o parâmetro ColocationStatus ao cmdlet Get-AzProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="89801-1015">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="89801-1016">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="89801-1016">Az.DataFactory</span></span>
* <span data-ttu-id="89801-1017">Atualização do SDK .NET do ADF para a versão 4.7.0</span><span class="sxs-lookup"><span data-stu-id="89801-1017">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="89801-1018">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="89801-1018">Az.DeploymentManager</span></span>
* <span data-ttu-id="89801-1019">Adiciona operações LIST para os recursos</span><span class="sxs-lookup"><span data-stu-id="89801-1019">Adds LIST operations for resources</span></span>
* <span data-ttu-id="89801-1020">Adiciona a capacidade de realizar operações nos passos de Verificação de Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="89801-1020">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="89801-1021">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="89801-1021">Az.HDInsight</span></span>
* <span data-ttu-id="89801-1022">Foi corrigido o erro do documento de New-AzHDInsightCluster.</span><span class="sxs-lookup"><span data-stu-id="89801-1022">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="89801-1023">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="89801-1023">Az.KeyVault</span></span>
* <span data-ttu-id="89801-1024">Foi adicionado o alias do Nome ao atributo VaultName para tornar Remove-AzureKeyVault consistente com New-AzureKeyVault.</span><span class="sxs-lookup"><span data-stu-id="89801-1024">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-1025">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-1025">Az.Network</span></span>
* <span data-ttu-id="89801-1026">Foi adicionado um novo exemplo a Set-AzNetworkWatcherConfigFlowLog.md para demonstrar o cenário de desativação da Análise de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="89801-1026">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="89801-1027">Foi adicionado suporte para atribuir a configuração IP de gestão ao Azure Firewall, uma sub-rede dedicada e IP Público que a firewall utilizará no tráfego de gestão</span><span class="sxs-lookup"><span data-stu-id="89801-1027">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="89801-1028">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="89801-1028">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="89801-1029">Foi adicionado o parâmetro -ManagementPublicIpAddress (não obrigatório) que aceita um objeto de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="89801-1029">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="89801-1030">Foi adicionado o método SetManagementIpConfiguration no objeto de firewall. Requer uma sub-rede e um endereço IP Público como entrada. O nome da sub-rede tem de ser "AzureFirewallManagementSubnet"</span><span class="sxs-lookup"><span data-stu-id="89801-1030">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="89801-1031">Foram corrigidos os exemplos de Get-AzNetworkSecurityGroup para mostrar exemplos de NSGs em vez de interfaces de rede.</span><span class="sxs-lookup"><span data-stu-id="89801-1031">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="89801-1032">Foi corrigido um erro no comando New-AzVpnSite que estava a impedir o ID do recurso de concluir um parâmetro.</span><span class="sxs-lookup"><span data-stu-id="89801-1032">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="89801-1033">Foi adicionado suporte para a Configuração do URL em Reescrever Conjunto de Ações de Regras no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="89801-1033">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="89801-1034">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="89801-1034">New cmdlets added:</span></span>
        - <span data-ttu-id="89801-1035">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="89801-1035">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="89801-1036">Foram atualizados cmdlets com o parâmetro opcional - UrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="89801-1036">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="89801-1037">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="89801-1037">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="89801-1038">Foi adicionado suporte para os recursos do NetworkWatcher ConnectionMonitor versão 2</span><span class="sxs-lookup"><span data-stu-id="89801-1038">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="89801-1039">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="89801-1039">Az.PolicyInsights</span></span>
* <span data-ttu-id="89801-1040">Foi adicionado suporte para avaliar a conformidade antes de determinar o recurso a remediar</span><span class="sxs-lookup"><span data-stu-id="89801-1040">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="89801-1041">Foi adicionado o parâmetro "-ResourceDiscoverMode" a Start-AzPolicyRemediation</span><span class="sxs-lookup"><span data-stu-id="89801-1041">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="89801-1042">Foi adicionado o cmdlet Get-AzPolicyMetadata para obter os recursos de metadados da política</span><span class="sxs-lookup"><span data-stu-id="89801-1042">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="89801-1043">Get-AzPolicyState e Get-AzPolicyStateSummary atualizados para a versão da API 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="89801-1043">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-1044">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-1044">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-1045">Foi adicionado suporte do Azure Site Recovery para remover um disco replicado.</span><span class="sxs-lookup"><span data-stu-id="89801-1045">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="89801-1046">O Azure Backup adicionou suporte para adicionar etiquetas ao criar um Cofre dos Serviços de Recuperação.</span><span class="sxs-lookup"><span data-stu-id="89801-1046">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-1047">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-1047">Az.Resources</span></span>
* <span data-ttu-id="89801-1048">-Scope foi tornado opcional nos cmdlets \*-AzPolicyAssignment com subscrição de contexto predefinida</span><span class="sxs-lookup"><span data-stu-id="89801-1048">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="89801-1049">Foram adicionados exemplos de criação de ADServicePrincipal com credenciais de palavras-passe e chaves</span><span class="sxs-lookup"><span data-stu-id="89801-1049">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-1050">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-1050">Az.Sql</span></span>
<span data-ttu-id="89801-1051">Foi corrigido o cmdlet New-AzSqlDatabaseSecondary para verificar a existência de PartnerDatabaseName em vez da existência de DatabaseName.</span><span class="sxs-lookup"><span data-stu-id="89801-1051">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-1052">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-1052">Az.Storage</span></span>
* <span data-ttu-id="89801-1053">Foi definido o suporte de Tipo de Chave de Encriptação na Tabela/Fila em Criar Conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="89801-1053">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="89801-1054">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="89801-1054">New-AzStorageAccount</span></span>
* <span data-ttu-id="89801-1055">Será apresentado RequestId quando StorageException não tiver ExtendedErrorInformation</span><span class="sxs-lookup"><span data-stu-id="89801-1055">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="89801-1056">Foi corrigido o exemplo 6 do cmdlet Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="89801-1056">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="89801-1057">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-1057">Az.Websites</span></span>
* <span data-ttu-id="89801-1058">Set-AzWebapp e Set-AzWebappSlot suportam as propriedades AlwaysOn, MinTls e FtpsState</span><span class="sxs-lookup"><span data-stu-id="89801-1058">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="89801-1059">Foi corrigido o problema em que a definição de HttpsOnly, juntamente com a alteração de AppservicePlan ao utilizar o único comando Set-AzWebApp, estava a repor HttpsOnly para o valor predefinido</span><span class="sxs-lookup"><span data-stu-id="89801-1059">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="89801-1060">3.3.0 – janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="89801-1060">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="89801-1061">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-1061">Az.Accounts</span></span>
* <span data-ttu-id="89801-1062">Add-AzEnvironment e Set-AzEnvironment foram atualizados para aceitar os parâmetros AzureAttestationServiceEndpointResourceId e AzureAttestationServiceEndpointSuffix</span><span class="sxs-lookup"><span data-stu-id="89801-1062">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="89801-1063">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="89801-1063">Az.Cdn</span></span>
* <span data-ttu-id="89801-1064">Apresentação dos detalhes da resposta de erro no cmdlet New-AzCdnEndpoint</span><span class="sxs-lookup"><span data-stu-id="89801-1064">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-1065">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-1065">Az.Compute</span></span>
* <span data-ttu-id="89801-1066">Correção do cmdlet Set-AzVMCustomScriptExtension para uma VM com disco OD gerido sem perfil de SO.</span><span class="sxs-lookup"><span data-stu-id="89801-1066">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="89801-1067">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="89801-1067">Az.ContainerInstance</span></span>
* <span data-ttu-id="89801-1068">Foram corrigidos os nomes de parâmetros utilizados pelo exemplo de New-AzContainerGroup</span><span class="sxs-lookup"><span data-stu-id="89801-1068">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="89801-1069">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="89801-1069">Az.DataBoxEdge</span></span>
* <span data-ttu-id="89801-1070">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="89801-1070">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="89801-1071">Obter o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="89801-1071">Get the Edge Storage Container</span></span>
* <span data-ttu-id="89801-1072">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="89801-1072">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="89801-1073">Criar novo Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="89801-1073">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="89801-1074">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="89801-1074">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="89801-1075">Remover o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="89801-1075">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="89801-1076">Foi adicionado o cmdlet "Invoke-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="89801-1076">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="89801-1077">Invocar ação para atualizar os dados no Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="89801-1077">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="89801-1078">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="89801-1078">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="89801-1079">Obter a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="89801-1079">Get the Edge Storage Account</span></span>
* <span data-ttu-id="89801-1080">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="89801-1080">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="89801-1081">Criar nova Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="89801-1081">Create new Edge Storage Account</span></span>
* <span data-ttu-id="89801-1082">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="89801-1082">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="89801-1083">Remover a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="89801-1083">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="89801-1084">Invocar o cmdlet "Invoke-AzDataBoxEdgeShare"</span><span class="sxs-lookup"><span data-stu-id="89801-1084">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="89801-1085">Invocar ação para atualizar os dados na partilha</span><span class="sxs-lookup"><span data-stu-id="89801-1085">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="89801-1086">Foi adicionado o cmdlet "Set-AzDataBoxEdgeStorageAccountCredential"</span><span class="sxs-lookup"><span data-stu-id="89801-1086">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="89801-1087">Definição de AzDataBoxEdgeStorageAccountCredential</span><span class="sxs-lookup"><span data-stu-id="89801-1087">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="89801-1088">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="89801-1088">Az.DataFactory</span></span>
* <span data-ttu-id="89801-1089">Adição das propriedades AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId e VersionStatus para o cmd Get-AzDataFactoryV2IntegrationRuntime</span><span class="sxs-lookup"><span data-stu-id="89801-1089">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="89801-1090">Atualização do SDK .NET do ADF para a versão 4.6.0</span><span class="sxs-lookup"><span data-stu-id="89801-1090">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="89801-1091">Adição do parâmetro "PublicIPs" para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a criação de Azure-SSIS IR com endereços IP públicos estáticos.</span><span class="sxs-lookup"><span data-stu-id="89801-1091">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="89801-1092">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="89801-1092">Az.DevTestLabs</span></span>
* <span data-ttu-id="89801-1093">Remoção da ligação quebrada em Get-AzDtlAllowedVMSizesPolicy.md</span><span class="sxs-lookup"><span data-stu-id="89801-1093">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="89801-1094">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="89801-1094">Az.EventHub</span></span>
* <span data-ttu-id="89801-1095">Correção do problema 10634: Correção da referência de objeto nulo para remover eventhubnamespace</span><span class="sxs-lookup"><span data-stu-id="89801-1095">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="89801-1096">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="89801-1096">Az.HDInsight</span></span>
* <span data-ttu-id="89801-1097">Correção do erro Invoke-AzHDInsightHiveJob.md.</span><span class="sxs-lookup"><span data-stu-id="89801-1097">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="89801-1098">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="89801-1098">Az.MachineLearning</span></span>
* <span data-ttu-id="89801-1099">Foram removidos os cmdlets abaixo porque MachineLearningCompute já não está disponível</span><span class="sxs-lookup"><span data-stu-id="89801-1099">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="89801-1100">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="89801-1100">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="89801-1101">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="89801-1101">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="89801-1102">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="89801-1102">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="89801-1103">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="89801-1103">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="89801-1104">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="89801-1104">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="89801-1105">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="89801-1105">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="89801-1106">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="89801-1106">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-1107">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-1107">Az.Network</span></span>
* <span data-ttu-id="89801-1108">Atualização da dependência de Microsoft.Azure.Management.SQL da versão 1.36-preview para 1.37-preview</span><span class="sxs-lookup"><span data-stu-id="89801-1108">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-1109">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-1109">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-1110">Alteração do Azure Site Recovery para suportar VMs de disco gerido com encriptação inativa com chaves geridas pelo cliente para o fornecedor do Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-1110">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="89801-1111">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-1111">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="89801-1112">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional ao nível do disco para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-1112">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="89801-1113">Suporte do Azure Site Recovery para atualizar o item protegido por replicação com encriptação de discos e definir o mapa para HyperV para o Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-1113">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-1114">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-1114">Az.Resources</span></span>
* <span data-ttu-id="89801-1115">Correção de um erro no documento de ajuda de "Remove-AzTag".</span><span class="sxs-lookup"><span data-stu-id="89801-1115">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-1116">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-1116">Az.Sql</span></span>
* <span data-ttu-id="89801-1117">Correção da funcionalidade dos cmdlets de linha de base do conjunto de avaliação de vulnerabilidades para funcionar na base de dados mestre da base de dados do Azure e limitá-la nas bases de dados do sistema de instância gerida</span><span class="sxs-lookup"><span data-stu-id="89801-1117">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="89801-1118">Correção de um erro ao criar o grupo de ativação pós-falha de instância SQL</span><span class="sxs-lookup"><span data-stu-id="89801-1118">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="89801-1119">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="89801-1119">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="89801-1120">Adição de DR como um novo tipo de Licença válido</span><span class="sxs-lookup"><span data-stu-id="89801-1120">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-1121">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-1121">Az.Storage</span></span>
* <span data-ttu-id="89801-1122">Adição de uma mensagem de aviso de alteração interruptiva para alteração do valor de DefaultAction numa futura versão</span><span class="sxs-lookup"><span data-stu-id="89801-1122">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="89801-1123">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="89801-1123">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="89801-1124">Suporte para obter a hora da última sincronização da conta de armazenamento ao executar get-AzureRMStorageAccount com o parâmetro -IncludeGeoReplicationStats</span><span class="sxs-lookup"><span data-stu-id="89801-1124">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span>
    - <span data-ttu-id="89801-1125">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="89801-1125">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="89801-1126">3.2.0 - Dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-1126">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="89801-1127">Geral</span><span class="sxs-lookup"><span data-stu-id="89801-1127">General</span></span>
* <span data-ttu-id="89801-1128">Atualização das referências em .psd1 para utilizar o caminho relativo para todos os módulos</span><span class="sxs-lookup"><span data-stu-id="89801-1128">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="89801-1129">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-1129">Az.Accounts</span></span>
* <span data-ttu-id="89801-1130">Definição do UserAgent correto para telemetria do lado do cliente para a pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="89801-1130">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="89801-1131">Apresentação de mensagem de erro amigável de utilizador quando o contexto é nulo na pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="89801-1131">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="89801-1132">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="89801-1132">Az.Batch</span></span>
* <span data-ttu-id="89801-1133">Correção do problema [10602](https://github.com/Azure/azure-powershell/issues/10602), em que **New-AzBatchPool** não enviava corretamente "VirtualMachineConfiguration.ContainerConfiguration" ou "VirtualMachineConfiguration.DataDisks" para o servidor.</span><span class="sxs-lookup"><span data-stu-id="89801-1133">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="89801-1134">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="89801-1134">Az.DataFactory</span></span>
* <span data-ttu-id="89801-1135">Atualização do SDK .NET do ADF para a versão 4.5.0</span><span class="sxs-lookup"><span data-stu-id="89801-1135">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="89801-1136">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="89801-1136">Az.FrontDoor</span></span>
* <span data-ttu-id="89801-1137">Adição do suporte de exclusão de regras geridas pela WAF</span><span class="sxs-lookup"><span data-stu-id="89801-1137">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="89801-1138">Adição de SocketAddr ao preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="89801-1138">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="89801-1139">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="89801-1139">Az.HealthcareApis</span></span>
* <span data-ttu-id="89801-1140">Processamento de Exceções</span><span class="sxs-lookup"><span data-stu-id="89801-1140">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="89801-1141">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="89801-1141">Az.KeyVault</span></span>
* <span data-ttu-id="89801-1142">Correção do erro em que era acedido um valor potencialmente não definido</span><span class="sxs-lookup"><span data-stu-id="89801-1142">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="89801-1143">Gestão de Certificados de Criptografia de Curva Elíptica</span><span class="sxs-lookup"><span data-stu-id="89801-1143">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="89801-1144">Adicionado suporte para especificar a Curva das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="89801-1144">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="89801-1145">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="89801-1145">Az.Monitor</span></span>
* <span data-ttu-id="89801-1146">Adição de um argumento opcional ao comando Adicionar Definições de Diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="89801-1146">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="89801-1147">Um argumento de opção que, se estiver presente, indica que a exportação para o Log Analytics deve ser feita para um esquema fixo (também conhecido como</span><span class="sxs-lookup"><span data-stu-id="89801-1147">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="89801-1148">tipo de dados dedicado)</span><span class="sxs-lookup"><span data-stu-id="89801-1148">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-1149">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-1149">Az.Network</span></span>
* <span data-ttu-id="89801-1150">Suporte para IpGroups na aplicação AzureFirewall, Nat e Regras de Rede.</span><span class="sxs-lookup"><span data-stu-id="89801-1150">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-1151">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-1151">Az.Resources</span></span>
* <span data-ttu-id="89801-1152">Correção de um problema em que a implementação do modelo não consegue ler um parâmetro se o nome estiver em conflito com um nome de parâmetro incorporado.</span><span class="sxs-lookup"><span data-stu-id="89801-1152">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="89801-1153">Os cmdlets da política foram atualizados para utilizar a nova versão de API 2019-09-01 que introduz suporte de agrupamento nas definições do conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="89801-1153">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-1154">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-1154">Az.Sql</span></span>
* <span data-ttu-id="89801-1155">Criação do armazenamento atualizada na ativação automática da Avaliação de Vulnerabilidades para StorageV2</span><span class="sxs-lookup"><span data-stu-id="89801-1155">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-1156">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-1156">Az.Storage</span></span>
* <span data-ttu-id="89801-1157">Suporte para gerar um token de SAS baseado na Identidade do Blob/Contentor com Contexto de Armazenamento baseado na autenticação OAuth</span><span class="sxs-lookup"><span data-stu-id="89801-1157">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="89801-1158">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="89801-1158">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="89801-1159">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="89801-1159">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="89801-1160">Suporte para revogar as Chaves de Delegação do Utilizador da Conta de Armazenamento, pelo que todos os tokens de SAS da identidade são revogados</span><span class="sxs-lookup"><span data-stu-id="89801-1160">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="89801-1161">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="89801-1161">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="89801-1162">Atualização de Microsoft.Azure.Management.Storage 14.2.0 para suportar a nova versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="89801-1162">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="89801-1163">Suporte de QuotaGiB (Quota de Partilha em Gibibye) para obter valores superiores a 5120 no plano de Gestão de cmdlets de Partilha de Ficheiros e foi adicionado o alias do parâmetro "Quota" ao parâmetro "QuotaGiB".</span><span class="sxs-lookup"><span data-stu-id="89801-1163">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span>
    - <span data-ttu-id="89801-1164">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="89801-1164">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="89801-1165">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="89801-1165">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="89801-1166">Adição do alias do parâmetro "QuotaGiB" ao parâmetro "Quota"</span><span class="sxs-lookup"><span data-stu-id="89801-1166">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="89801-1167">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="89801-1167">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="89801-1168">Correção do problema em que Set-AzStorageContainerAcl consegue limpar a Política de Acesso armazenada</span><span class="sxs-lookup"><span data-stu-id="89801-1168">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="89801-1169">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="89801-1169">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="89801-1170">3.1.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-1170">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="89801-1171">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="89801-1171">Highlights since the last major release</span></span>
* <span data-ttu-id="89801-1172">Az.DataBoxEdge 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="89801-1172">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="89801-1173">Az.SqlVirtualMachine 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="89801-1173">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-1174">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-1174">Az.Compute</span></span>
* <span data-ttu-id="89801-1175">Funcionalidade de Reaplicação da VM</span><span class="sxs-lookup"><span data-stu-id="89801-1175">VM Reapply feature</span></span>
    - <span data-ttu-id="89801-1176">Adição do parâmetro Reapply ao cmdlet Set-AzVM</span><span class="sxs-lookup"><span data-stu-id="89801-1176">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="89801-1177">Funcionalidade AutomaticRepairs do Conjunto de Dimensionamento de VM:</span><span class="sxs-lookup"><span data-stu-id="89801-1177">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="89801-1178">Adição dos parâmetros EnableAutomaticRepair, AutomaticRepairGracePeriod e AutomaticRepairMaxInstanceRepairsPercent aos seguintes cmdlets:   New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="89801-1178">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="89801-1179">Suporte para imagens de galeria entre inquilinos para New-AzVM</span><span class="sxs-lookup"><span data-stu-id="89801-1179">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="89801-1180">Adição de "Spot" ao preenchedor de argumentos do parâmetro Priority nos cmdlets New-AzVM, New-AzVMConfig e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="89801-1180">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="89801-1181">Adição dos parâmetros DiskIOPSReadWrite e DiskMBpsReadWrite ao cmdlet Add-AzVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="89801-1181">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="89801-1182">Alteração do parâmetro SourceImageId do cmdlet New-AzGalleryImageVersion para opcional</span><span class="sxs-lookup"><span data-stu-id="89801-1182">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="89801-1183">Adição dos parâmetros OSDiskImage e DataDiskImage ao cmdlet New-AzGalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="89801-1183">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="89801-1184">Adição do parâmetro HyperVGeneration ao cmdlet New-AzGalleryImageDefinition</span><span class="sxs-lookup"><span data-stu-id="89801-1184">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="89801-1185">Adição dos parâmetros SkipExtensionsOnOverprovisionedVMs aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="89801-1185">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="89801-1186">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="89801-1186">Az.DataBoxEdge</span></span>
* <span data-ttu-id="89801-1187">Adição do cmdlet `Get-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="89801-1187">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="89801-1188">Obter a Encomenda</span><span class="sxs-lookup"><span data-stu-id="89801-1188">Get the Order</span></span>
* <span data-ttu-id="89801-1189">Adição do cmdlet `New-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="89801-1189">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="89801-1190">Criar nova Encomenda</span><span class="sxs-lookup"><span data-stu-id="89801-1190">Create new Order</span></span>
* <span data-ttu-id="89801-1191">Adição do cmdlet `Remove-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="89801-1191">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="89801-1192">Remover a Encomenda</span><span class="sxs-lookup"><span data-stu-id="89801-1192">Remove the Order</span></span>
* <span data-ttu-id="89801-1193">Alteração no cmdlet `New-AzDataBoxEdgeShare`</span><span class="sxs-lookup"><span data-stu-id="89801-1193">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="89801-1194">Agora cria uma Partilha Local</span><span class="sxs-lookup"><span data-stu-id="89801-1194">Now creates Local Share</span></span>
* <span data-ttu-id="89801-1195">Adição do cmdlet `Set-AzDataBoxEdgeRole`</span><span class="sxs-lookup"><span data-stu-id="89801-1195">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="89801-1196">Agora, o IotRole pode ser mapeado para a Partilha</span><span class="sxs-lookup"><span data-stu-id="89801-1196">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="89801-1197">Adição do cmdlet `Invoke-AzDataBoxEdgeDevice`</span><span class="sxs-lookup"><span data-stu-id="89801-1197">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="89801-1198">Invocar verificação da atualização, transferência da atualização, instalação das atualizações no dispositivo</span><span class="sxs-lookup"><span data-stu-id="89801-1198">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="89801-1199">Adição do cmdlet `Get-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="89801-1199">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="89801-1200">Obtém as informações sobre os Acionadores</span><span class="sxs-lookup"><span data-stu-id="89801-1200">Gets the information about Triggers</span></span>
* <span data-ttu-id="89801-1201">Adição do cmdlet `New-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="89801-1201">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="89801-1202">Criar novos Acionadores</span><span class="sxs-lookup"><span data-stu-id="89801-1202">Create new Triggers</span></span>
* <span data-ttu-id="89801-1203">Adição do cmdlet `Remove-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="89801-1203">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="89801-1204">Remover os Acionadores</span><span class="sxs-lookup"><span data-stu-id="89801-1204">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="89801-1205">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="89801-1205">Az.DataFactory</span></span>
* <span data-ttu-id="89801-1206">Atualização do SDK .NET do ADF para a versão 4.4.0</span><span class="sxs-lookup"><span data-stu-id="89801-1206">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="89801-1207">Adição do parâmetro "ExpressCustomSetup" para o cmdlet "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir configurações e componentes de terceiros sem scripts de configuração personalizados.</span><span class="sxs-lookup"><span data-stu-id="89801-1207">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="89801-1208">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="89801-1208">Az.DataLakeStore</span></span>
* <span data-ttu-id="89801-1209">Atualização da documentação de Get-AzDataLakeStoreDeletedItem e Restore-AzDataLakeStoreDeletedItem</span><span class="sxs-lookup"><span data-stu-id="89801-1209">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="89801-1210">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="89801-1210">Az.EventHub</span></span>
* <span data-ttu-id="89801-1211">Correção do problema 10301: Correção do formato de data do token de SAS</span><span class="sxs-lookup"><span data-stu-id="89801-1211">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="89801-1212">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="89801-1212">Az.FrontDoor</span></span>
* <span data-ttu-id="89801-1213">Adição do parâmetro MinimumTlsVersion a Enable-AzFrontDoorCustomDomainHttps e New-AzFrontDoorFrontendEndpointObject</span><span class="sxs-lookup"><span data-stu-id="89801-1213">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="89801-1214">Adição dos parâmetros HealthProbeMethod e EnabledState a New-AzFrontDoorHealthProbeSettingObject</span><span class="sxs-lookup"><span data-stu-id="89801-1214">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="89801-1215">Adição de um novo cmdlet para criar um objeto BackendPoolsSettings para passar para a criação/atualização do Front Door</span><span class="sxs-lookup"><span data-stu-id="89801-1215">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="89801-1216">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="89801-1216">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-1217">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-1217">Az.Network</span></span>
* <span data-ttu-id="89801-1218">Alteração dos exemplos de opções FilterData de "Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" e "Start-AzVirtualnetworkGatewayPacketCapture.md".</span><span class="sxs-lookup"><span data-stu-id="89801-1218">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="89801-1219">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="89801-1219">Az.PrivateDns</span></span>
* <span data-ttu-id="89801-1220">Atualização do SDK .NET do PrivateDns para a versão 1.0.0</span><span class="sxs-lookup"><span data-stu-id="89801-1220">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-1221">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-1221">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-1222">Suporte do Azure Site Recovery para selecionar o tipo de disco ao ativar a proteção.</span><span class="sxs-lookup"><span data-stu-id="89801-1222">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="89801-1223">Correção do Azure Site Recovery para a edição de ações do plano de recuperação.</span><span class="sxs-lookup"><span data-stu-id="89801-1223">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="89801-1224">Suporte de Restauro de SQL do Azure Backup para aceitar BDs de filestream.</span><span class="sxs-lookup"><span data-stu-id="89801-1224">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="89801-1225">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="89801-1225">Az.RedisCache</span></span>
* <span data-ttu-id="89801-1226">Adição do parâmetro "MinimumTlsVersion" nos cmdlets "New-AzRedisCache" e "Set-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="89801-1226">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="89801-1227">Adição, também, de "MinimumTlsVersion" na saída do cmdlet "Get-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="89801-1227">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="89801-1228">Adição da validação no parâmetro "-Size" para os cmdlets "Set-AzRedisCache" e "New-AzRedisCache"</span><span class="sxs-lookup"><span data-stu-id="89801-1228">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-1229">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-1229">Az.Resources</span></span>
- <span data-ttu-id="89801-1230">Atualização dos cmdlets de política no sentido de utilizar a nova versão de api 2019-06-01, a qual tem a nova propriedade EnforcementMode na atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="89801-1230">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="89801-1231">Atualização do exemplo de ajuda da definição da política de criação</span><span class="sxs-lookup"><span data-stu-id="89801-1231">Updated create policy definition help example</span></span>
- <span data-ttu-id="89801-1232">Correção do erro Remove-AZADServicePrincipal -ServicePrincipalName. Apresentação de uma referência nula quando o nome do principal do serviço não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="89801-1232">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="89801-1233">Correção do erro New-AZADServicePrincipal. Apresentação de uma referência nula quando o inquilino não tem uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="89801-1233">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="89801-1234">Alteração de New-AzAdServicePrincipal para adicionar credenciais apenas a aplicações associadas.</span><span class="sxs-lookup"><span data-stu-id="89801-1234">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-1235">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-1235">Az.Sql</span></span>
* <span data-ttu-id="89801-1236">Adição de suporte para a base de dados ReadReplicaCount.</span><span class="sxs-lookup"><span data-stu-id="89801-1236">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="89801-1237">Correção de Set-AzSqlDatabase quando a redundância de zona não está definida</span><span class="sxs-lookup"><span data-stu-id="89801-1237">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="89801-1238">3.0.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-1238">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="89801-1239">Geral</span><span class="sxs-lookup"><span data-stu-id="89801-1239">General</span></span>
* <span data-ttu-id="89801-1240">Disponibilização do Az.PrivateDns 1.0.0</span><span class="sxs-lookup"><span data-stu-id="89801-1240">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="89801-1241">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-1241">Az.Accounts</span></span>
* <span data-ttu-id="89801-1242">Adição de uma mensagem de descontinuação para o alias "Resolve-Error".</span><span class="sxs-lookup"><span data-stu-id="89801-1242">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="89801-1243">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="89801-1243">Az.Advisor</span></span>
* <span data-ttu-id="89801-1244">Adição da nova categoria "Excelência Operacional" ao cmdlet Get-AzAdvisorRecommendation.</span><span class="sxs-lookup"><span data-stu-id="89801-1244">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="89801-1245">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="89801-1245">Az.Batch</span></span>
* <span data-ttu-id="89801-1246">Mudança de nome de `CoreQuota` em `BatchAccountContext` para `DedicatedCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="89801-1246">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="89801-1247">Existe também um novo `LowPriorityCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="89801-1247">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="89801-1248">Isto afeta **Get-AzBatchAccount**.</span><span class="sxs-lookup"><span data-stu-id="89801-1248">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="89801-1249">O parâmetro **New-AzBatchTask** `-ResourceFile` assume agora uma coleção de objetos `PSResourceFile`, os quais podem ser construídos com o novo cmdlet **New-AzBatchResourceFile**.</span><span class="sxs-lookup"><span data-stu-id="89801-1249">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="89801-1250">Novo cmdlet **New-AzBatchResourceFile** para ajudar a criar objetos `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="89801-1250">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="89801-1251">Estes podem ser fornecidos a **New-AzBatchTask** no parâmetro `-ResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="89801-1251">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="89801-1252">Isto suporta dois novos tipos de ficheiro de recursos para além do caminho `HttpUrl` existente:</span><span class="sxs-lookup"><span data-stu-id="89801-1252">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="89801-1253">Os ficheiros de recursos baseados em `AutoStorageContainerName` transferem um contentor integral de armazenamento automático para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="89801-1253">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="89801-1254">Os ficheiros de recursos baseados em `StorageContainerUrl` transferem o contentor especificado no URL para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="89801-1254">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="89801-1255">Remoção da propriedade `ApplicationPackages` de `PSApplication` devolvida por **Get-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="89801-1255">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="89801-1256">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com **Get-AzBatchApplicationPackage**.</span><span class="sxs-lookup"><span data-stu-id="89801-1256">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="89801-1257">Por exemplo: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span><span class="sxs-lookup"><span data-stu-id="89801-1257">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="89801-1258">Mudança de nome de `ApplicationId` para `ApplicationName` em **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication** e **Set-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="89801-1258">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="89801-1259">`ApplicationId` é agora um alias de `ApplicationName`.</span><span class="sxs-lookup"><span data-stu-id="89801-1259">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="89801-1260">Adição da nova propriedade `PSWindowsUserConfiguration` a `PSUserAccount`.</span><span class="sxs-lookup"><span data-stu-id="89801-1260">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="89801-1261">Mudança de nome de `Version` para `Name` em `PSApplicationPackage`.</span><span class="sxs-lookup"><span data-stu-id="89801-1261">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="89801-1262">Mudança de nome de `BlobSource` para `HttpUrl` em `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="89801-1262">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="89801-1263">Remoção da propriedade `OSDisk` de `PSVirtualMachineConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="89801-1263">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="89801-1264">Remoção de **Set-AzBatchPoolOSVersion**.</span><span class="sxs-lookup"><span data-stu-id="89801-1264">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="89801-1265">Esta operação deixou de ser suportada.</span><span class="sxs-lookup"><span data-stu-id="89801-1265">This operation is no longer supported.</span></span>
* <span data-ttu-id="89801-1266">Remoção de `TargetOSVersion` de `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="89801-1266">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="89801-1267">Mudança de nome de `CurrentOSVersion` para `OSVersion` em `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="89801-1267">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="89801-1268">Remoção de `DataEgressGiB` e `DataIngressGiB` de `PSPoolUsageMetrics`.</span><span class="sxs-lookup"><span data-stu-id="89801-1268">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="89801-1269">Remoção de **Get-AzBatchNodeAgentSku** e substituição deste por **Get-AzBatchSupportedImage**.</span><span class="sxs-lookup"><span data-stu-id="89801-1269">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span>
  - <span data-ttu-id="89801-1270">**Get-AzBatchSupportedImage** devolve os mesmos dados de **Get-AzBatchNodeAgentSku**, mas num formato mais acessível.</span><span class="sxs-lookup"><span data-stu-id="89801-1270">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="89801-1271">As novas imagens não verificadas agora também são devolvidas.</span><span class="sxs-lookup"><span data-stu-id="89801-1271">New non-verified images are also now returned.</span></span> <span data-ttu-id="89801-1272">Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.</span><span class="sxs-lookup"><span data-stu-id="89801-1272">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="89801-1273">Adição da capacidade de montagem de sistemas de ficheiros remotos em cada nó de um conjunto através do novo parâmetro `MountConfiguration` de **New-AzBatchPool**.</span><span class="sxs-lookup"><span data-stu-id="89801-1273">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="89801-1274">Adição do suporte a regras de segurança de rede que bloqueiam o acesso de rede a um conjunto com base na porta de origem do tráfego.</span><span class="sxs-lookup"><span data-stu-id="89801-1274">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="89801-1275">Isto ocorre através da propriedade `SourcePortRanges` em `PSNetworkSecurityGroupRule`.</span><span class="sxs-lookup"><span data-stu-id="89801-1275">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="89801-1276">Ao executar um contentor, o Batch agora suporta a execução da tarefa no diretório de trabalho do contentor ou no diretório de trabalho da tarefa do Batch.</span><span class="sxs-lookup"><span data-stu-id="89801-1276">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="89801-1277">Isto é controlado pela propriedade `WorkingDirectory` em `PSTaskContainerSettings`.</span><span class="sxs-lookup"><span data-stu-id="89801-1277">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="89801-1278">Adição da capacidade de especificar uma coleção de IPs públicos em `PSNetworkConfiguration` através da nova propriedade `PublicIPs`.</span><span class="sxs-lookup"><span data-stu-id="89801-1278">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="89801-1279">Isto garante que os nós no Conjunto terão um IP da lista de IPs fornecidos pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="89801-1279">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="89801-1280">Quando não for especificado, o valor predefinido de `WaitForSuccess` em `PSSTartTask` é agora `$True` (era `$False`).</span><span class="sxs-lookup"><span data-stu-id="89801-1280">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="89801-1281">Quando não for especificado, o valor predefinido de `Scope` em `PSAutoUserSpecification` é agora `Pool` (era `Task` no Windows e `Pool` no Linux).</span><span class="sxs-lookup"><span data-stu-id="89801-1281">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="89801-1282">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="89801-1282">Az.Cdn</span></span>
* <span data-ttu-id="89801-1283">Introdução de UrlRewriteAction e CacheKeyQueryStringAction em RulesEngine.</span><span class="sxs-lookup"><span data-stu-id="89801-1283">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="89801-1284">Correção de vários erros como a falta da Entrada "Seletor" no cmdlet New-AzDeliveryRuleCondition.</span><span class="sxs-lookup"><span data-stu-id="89801-1284">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-1285">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-1285">Az.Compute</span></span>
* <span data-ttu-id="89801-1286">Funcionalidade Conjunto de Encriptação de Discos</span><span class="sxs-lookup"><span data-stu-id="89801-1286">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="89801-1287">Novos cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="89801-1287">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="89801-1288">Adição do parâmetro DiskEncryptionSetId aos seguintes cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="89801-1288">DiskEncryptionSetId parameter is added to the following cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="89801-1289">Adição dos parâmetros DiskEncryptionSetId e EncryptionType aos seguintes cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="89801-1289">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="89801-1290">Adição do parâmetro PublicIPAddressVersion a New-AzVmssIPConfig</span><span class="sxs-lookup"><span data-stu-id="89801-1290">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="89801-1291">Movimentação de FileUris da extensão de script personalizado da definição pública para a definição protegida</span><span class="sxs-lookup"><span data-stu-id="89801-1291">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="89801-1292">Adição de ScaleInPolicy aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="89801-1292">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="89801-1293">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="89801-1293">Breaking changes</span></span>
    - <span data-ttu-id="89801-1294">Utilização do parâmetro UploadSizeInBytes em vez de DiskSizeGB para New-AzDiskConfig quando CreateOption é Carregar</span><span class="sxs-lookup"><span data-stu-id="89801-1294">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="89801-1295">Substituição de PublishingProfile.Source.ManagedImage.Id por StorageProfile.Source.Id no objeto GalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="89801-1295">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="89801-1296">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="89801-1296">Az.DataFactory</span></span>
* <span data-ttu-id="89801-1297">Atualização da versão do SDK .Net do ADF para 4.3.0</span><span class="sxs-lookup"><span data-stu-id="89801-1297">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="89801-1298">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="89801-1298">Az.DataLakeStore</span></span>
* <span data-ttu-id="89801-1299">Atualização da versão do SDK ADLS (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) ) com as seguintes correções</span><span class="sxs-lookup"><span data-stu-id="89801-1299">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="89801-1300">Evita a apresentação de uma exceção ao mesmo tempo que não consegue anular a serialização do creationtime do lixo ou da entrada de diretório.</span><span class="sxs-lookup"><span data-stu-id="89801-1300">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="89801-1301">Expõe a definição por tempo limite do pedido em adlsclient</span><span class="sxs-lookup"><span data-stu-id="89801-1301">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="89801-1302">Correção da passagem do syncflag original para a recuperação de badoffset</span><span class="sxs-lookup"><span data-stu-id="89801-1302">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="89801-1303">Correção de EnumerateDirectory para obter o token de continuação após a verificação da resposta</span><span class="sxs-lookup"><span data-stu-id="89801-1303">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="89801-1304">Correção do Erro de Concatenação</span><span class="sxs-lookup"><span data-stu-id="89801-1304">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="89801-1305">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="89801-1305">Az.FrontDoor</span></span>
* <span data-ttu-id="89801-1306">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="89801-1306">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="89801-1307">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="89801-1307">Az.HDInsight</span></span>
* <span data-ttu-id="89801-1308">Correção do erro em que o cliente recebe o erro "Não é uma cadeia Base 64 válida" quando utiliza Get-AzHDInsightCluster para obter o cluster com o armazenamento ADLSGen1.</span><span class="sxs-lookup"><span data-stu-id="89801-1308">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="89801-1309">Adição de um parâmetro com o nome "ApplicationId" a três cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig e New-AzHDInsightCluster para que o cliente consiga fornecer o ID da aplicação do principal de serviço que permite aceder ao Azure Data Lake.</span><span class="sxs-lookup"><span data-stu-id="89801-1309">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="89801-1310">Alteração de Microsoft.Azure.Management.HDInsight da versão 2.1.0 para a 5.1.0</span><span class="sxs-lookup"><span data-stu-id="89801-1310">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="89801-1311">Remoção de cinco cmdlets:</span><span class="sxs-lookup"><span data-stu-id="89801-1311">Removed five cmdlets:</span></span>
    - <span data-ttu-id="89801-1312">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="89801-1312">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="89801-1313">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="89801-1313">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="89801-1314">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="89801-1314">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="89801-1315">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="89801-1315">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="89801-1316">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="89801-1316">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="89801-1317">Adição de três cmdlets:</span><span class="sxs-lookup"><span data-stu-id="89801-1317">Added three cmdlets:</span></span>
    - <span data-ttu-id="89801-1318">Get-AzHDInsightMonitoring para substituir Get-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="89801-1318">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="89801-1319">Enable-AzHDInsightMonitoring para substituir Enable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="89801-1319">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="89801-1320">Disable-AzHDInsightMonitoring para substituir Disable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="89801-1320">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="89801-1321">Correção do cmdlet Get-AzHDInsightProperties para suportar a obtenção de informações sobre capacidades de uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="89801-1321">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="89801-1322">Remoção de conjuntos de parâmetros("Spark1", "Spark2") de Add-AzHDInsightConfigValue.</span><span class="sxs-lookup"><span data-stu-id="89801-1322">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="89801-1323">Adição de exemplos aos documentos de ajuda do cmdlet Add-AzHDInsightSecurityProfile.</span><span class="sxs-lookup"><span data-stu-id="89801-1323">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="89801-1324">Alteração do tipo de saída dos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="89801-1324">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="89801-1325">Alteração do tipo de saída de Get-AzHDInsightProperties de CapabilitiesResponse para AzureHDInsightCapabilities.</span><span class="sxs-lookup"><span data-stu-id="89801-1325">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="89801-1326">Alteração do tipo de saída de Remove-AzHDInsightCluster de ClusterGetResponse para booleano.</span><span class="sxs-lookup"><span data-stu-id="89801-1326">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="89801-1327">Alteração do tipo de saída de Set-AzHDInsightGatewaySettings de HttpConnectivitySettings para GatewaySettings.</span><span class="sxs-lookup"><span data-stu-id="89801-1327">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="89801-1328">Adição de alguns casos de teste de cenários.</span><span class="sxs-lookup"><span data-stu-id="89801-1328">Added some scenario test cases.</span></span>
* <span data-ttu-id="89801-1329">Remoção de alguns alias: "Add-AzHDInsightConfigValues", "Get-AzHDInsightProperties".</span><span class="sxs-lookup"><span data-stu-id="89801-1329">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="89801-1330">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="89801-1330">Az.IotHub</span></span>
* <span data-ttu-id="89801-1331">Alterações interruptivas:</span><span class="sxs-lookup"><span data-stu-id="89801-1331">Breaking changes:</span></span>
    - <span data-ttu-id="89801-1332">O cmdlet "Add-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="89801-1332">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="89801-1333">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Add-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="89801-1333">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="89801-1334">O cmdlet "Get-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="89801-1334">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="89801-1335">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Get-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="89801-1335">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="89801-1336">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="89801-1336">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="89801-1337">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="89801-1337">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="89801-1338">O cmdlet "New-AzIotHubExportDevice" deixou de suportar o alias "New-AzIotHubExportDevices".</span><span class="sxs-lookup"><span data-stu-id="89801-1338">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="89801-1339">O cmdlet "New-AzIotHubImportDevice" deixou de suportar o alias "New-AzIotHubImportDevices".</span><span class="sxs-lookup"><span data-stu-id="89801-1339">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="89801-1340">O cmdlet "Remove-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="89801-1340">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="89801-1341">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Remove-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="89801-1341">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="89801-1342">O cmdlet "Set-AzIotHub" deixou de suportar o parâmetro "OperationsMonitoringProperties" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="89801-1342">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="89801-1343">O conjunto de parâmetros "UpdateOperationsMonitoringProperties" do cmdlet "Set-AzIotHub" foi removido.</span><span class="sxs-lookup"><span data-stu-id="89801-1343">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-1344">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-1344">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-1345">Suporte do Azure Site Recovery para configurar recursos de rede como NSG, IP público e balanceadores de carga internos do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-1345">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="89801-1346">Suporte do Azure Site Recovery para escrever para um disco gerido do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-1346">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="89801-1347">Suporte do Azure Site Recovery para redução de NIC do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-1347">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="89801-1348">Suporte do Azure Site Recovery para aceleração de rede do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-1348">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="89801-1349">Suporte do Azure Site Recovery para a atualização automática do agente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-1349">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="89801-1350">Suporte do Azure Site Recovery para SSD Standard do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-1350">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="89801-1351">Suporte do Azure Site Recovery para a codificação em dois passos do Azure Disk Encryption do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-1351">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="89801-1352">Suporte do Azure Site Recovery para a proteção de um disco adicionado recentemente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-1352">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="89801-1353">Adição da funcionalidade SoftDelete para VM e de testes para softdelete</span><span class="sxs-lookup"><span data-stu-id="89801-1353">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-1354">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-1354">Az.Resources</span></span>
* <span data-ttu-id="89801-1355">Atualização da assemblagem de dependências Microsoft.Extensions.Caching.Memory da versão 1.1.1 para a 2.2</span><span class="sxs-lookup"><span data-stu-id="89801-1355">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-1356">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-1356">Az.Network</span></span>
* <span data-ttu-id="89801-1357">Alteração de todos os cmdlets para PrivateEndpointConnection para suportar o fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="89801-1357">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="89801-1358">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="89801-1358">Updated cmdlet:</span></span>
        - <span data-ttu-id="89801-1359">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="89801-1359">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="89801-1360">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="89801-1360">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="89801-1361">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="89801-1361">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="89801-1362">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="89801-1362">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="89801-1363">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="89801-1363">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="89801-1364">Adição de novo cmdlet para PrivateLinkResource também com suporte de fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="89801-1364">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="89801-1365">Novo cmdlet:</span><span class="sxs-lookup"><span data-stu-id="89801-1365">New cmdlet:</span></span>
        - <span data-ttu-id="89801-1366">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="89801-1366">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="89801-1367">Adição de novos campos e parâmetro para a funcionalidade Protocolo de Proxy V2.</span><span class="sxs-lookup"><span data-stu-id="89801-1367">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="89801-1368">Adição da propriedade EnableProxyProtocol em PrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="89801-1368">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="89801-1369">Adição da propriedade LinkIdentifier em PrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="89801-1369">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="89801-1370">Atualização de New-AzPrivateLinkService para adicionar um novo parâmetro adicional EnableProxyProtocol.</span><span class="sxs-lookup"><span data-stu-id="89801-1370">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="89801-1371">Correção da descrição incorreta do parâmetro na documentação de referência "New-AzApplicationGatewaySku"</span><span class="sxs-lookup"><span data-stu-id="89801-1371">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="89801-1372">Novos cmdlets para suportar a política de firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="89801-1372">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="89801-1373">Adição de suporte para o recurso subordinado RouteTables de VirtualHub</span><span class="sxs-lookup"><span data-stu-id="89801-1373">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="89801-1374">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="89801-1374">New cmdlets added:</span></span>
        - <span data-ttu-id="89801-1375">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="89801-1375">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="89801-1376">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="89801-1376">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="89801-1377">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="89801-1377">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="89801-1378">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="89801-1378">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="89801-1379">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="89801-1379">Set-AzVirtualHub</span></span>
* <span data-ttu-id="89801-1380">Adição de suporte para o SKU de novas propriedades de VirtualHub e VirtualWANType de VirtualWan</span><span class="sxs-lookup"><span data-stu-id="89801-1380">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="89801-1381">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="89801-1381">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="89801-1382">New-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="89801-1382">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="89801-1383">Update-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="89801-1383">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="89801-1384">New-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="89801-1384">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="89801-1385">Update-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="89801-1385">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="89801-1386">Adição de suporte para a propriedade EnableInternetSecurity para HubVnetConnection, VpnConnection e ExpressRouteConnection</span><span class="sxs-lookup"><span data-stu-id="89801-1386">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="89801-1387">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="89801-1387">New cmdlets added:</span></span>
        - <span data-ttu-id="89801-1388">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="89801-1388">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="89801-1389">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="89801-1389">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="89801-1390">New-AzureRmVirtualHubVnetConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="89801-1390">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="89801-1391">New-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="89801-1391">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="89801-1392">Update-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="89801-1392">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="89801-1393">New-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="89801-1393">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="89801-1394">Set-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="89801-1394">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="89801-1395">Adição de suporte para Configurar a Política WebApplicationFirewall de Nível Superior</span><span class="sxs-lookup"><span data-stu-id="89801-1395">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="89801-1396">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="89801-1396">New cmdlets added:</span></span>
        - <span data-ttu-id="89801-1397">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="89801-1397">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="89801-1398">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="89801-1398">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="89801-1399">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="89801-1399">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="89801-1400">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="89801-1400">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="89801-1401">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="89801-1401">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="89801-1402">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="89801-1402">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="89801-1403">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="89801-1403">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="89801-1404">New-AzApplicationGatewayFirewallPolicy : adição do parâmetro PolicySetting, ManagedRule</span><span class="sxs-lookup"><span data-stu-id="89801-1404">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="89801-1405">Adição de suporte para o operador GeoMatch em CustomRule</span><span class="sxs-lookup"><span data-stu-id="89801-1405">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="89801-1406">Adição de GeoMatch ao operador em FirewallCondition</span><span class="sxs-lookup"><span data-stu-id="89801-1406">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="89801-1407">Adição de suporte para a Política de firewall perListener e perSite</span><span class="sxs-lookup"><span data-stu-id="89801-1407">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="89801-1408">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="89801-1408">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="89801-1409">New-AzApplicationGatewayHttpListener : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="89801-1409">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="89801-1410">New-AzApplicationGatewayPathRuleConfig : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="89801-1410">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="89801-1411">Correção da sub-rede necessária com o nome AzureBastionSubnet em "PSBastion" pode não ser sensível às maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="89801-1411">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="89801-1412">Suporte para FQDNs de Destino nas Regras de Rede e para FQDN Traduzido em Regras NAT para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="89801-1412">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="89801-1413">Adição de suporte para o recurso de nível superior RouteTables de IpGroup</span><span class="sxs-lookup"><span data-stu-id="89801-1413">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="89801-1414">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="89801-1414">New cmdlets added:</span></span>
        - <span data-ttu-id="89801-1415">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="89801-1415">New-AzIpGroup</span></span>
        - <span data-ttu-id="89801-1416">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="89801-1416">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="89801-1417">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="89801-1417">Get-AzIpGroup</span></span>
        - <span data-ttu-id="89801-1418">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="89801-1418">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="89801-1419">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="89801-1419">Az.ServiceFabric</span></span>
* <span data-ttu-id="89801-1420">Remoção do cmdlet Add-AzServiceFabricApplicationCertificate uma vez que este cenário é abrangido por Add-AzVmssSecret.</span><span class="sxs-lookup"><span data-stu-id="89801-1420">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-1421">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-1421">Az.Sql</span></span>
* <span data-ttu-id="89801-1422">Adição de suporte para o restauro de bases de dados removidas em Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="89801-1422">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="89801-1423">Descontinuação dos cmdlets de auditoria antigos do código.</span><span class="sxs-lookup"><span data-stu-id="89801-1423">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="89801-1424">Remoção de aliases descontinuados:</span><span class="sxs-lookup"><span data-stu-id="89801-1424">Removed deprecated aliases:</span></span>
* <span data-ttu-id="89801-1425">Get-AzSqlDatabaseIndexRecommendations (utilize antes Get-AzSqlDatabaseIndexRecommendation)</span><span class="sxs-lookup"><span data-stu-id="89801-1425">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="89801-1426">Get-AzSqlDatabaseRestorePoints (utilize antes Get-AzSqlDatabaseRestorePoint)</span><span class="sxs-lookup"><span data-stu-id="89801-1426">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="89801-1427">Remoção do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="89801-1427">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="89801-1428">Remoção dos aliases dos cmdlets descontinuados das Definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="89801-1428">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="89801-1429">Descontinuação dos cmdlets das Definições de Deteção Avançada de Ameaças</span><span class="sxs-lookup"><span data-stu-id="89801-1429">Deprecate Advanced Threat Detection Settings cmdlets</span></span>
* <span data-ttu-id="89801-1430">Adição de cmdlets para Desativar e Ativar as recomendações de sensibilidade nas colunas de uma base de dados.</span><span class="sxs-lookup"><span data-stu-id="89801-1430">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-1431">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-1431">Az.Storage</span></span>
* <span data-ttu-id="89801-1432">Suporte à ativação da partilha de Ficheiros de Grandes Dimensões ao criar ou atualizar uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="89801-1432">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="89801-1433">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="89801-1433">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="89801-1434">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="89801-1434">Set-AzStorageAccount</span></span>
* <span data-ttu-id="89801-1435">Ao fechar/obter o Identificador de ficheiro, ignorar a verificação do caminho de entrada corresponde a Diretório de ficheiros ou Ficheiro, de forma a evitar a falha com o objeto no estado DeletePending</span><span class="sxs-lookup"><span data-stu-id="89801-1435">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="89801-1436">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="89801-1436">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="89801-1437">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="89801-1437">Close-AzStorageFileHandle</span></span>

## <a name="280---october-2019"></a><span data-ttu-id="89801-1438">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-1438">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="89801-1439">Geral</span><span class="sxs-lookup"><span data-stu-id="89801-1439">General</span></span>
* <span data-ttu-id="89801-1440">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="89801-1440">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="89801-1441">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-1441">Az.Accounts</span></span>
* <span data-ttu-id="89801-1442">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="89801-1442">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="89801-1443">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="89801-1443">Az.ApiManagement</span></span>
* <span data-ttu-id="89801-1444">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="89801-1444">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="89801-1445">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="89801-1445">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="89801-1446">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="89801-1446">Az.Automation</span></span>
* <span data-ttu-id="89801-1447">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="89801-1447">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="89801-1448">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="89801-1448">Az.Batch</span></span>
* <span data-ttu-id="89801-1449">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="89801-1449">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-1450">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-1450">Az.Compute</span></span>
* <span data-ttu-id="89801-1451">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="89801-1451">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="89801-1452">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="89801-1452">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="89801-1453">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="89801-1453">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span>
* <span data-ttu-id="89801-1454">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="89801-1454">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="89801-1455">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="89801-1455">Az.DataFactory</span></span>
* <span data-ttu-id="89801-1456">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="89801-1456">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="89801-1457">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="89801-1457">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="89801-1458">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="89801-1458">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="89801-1459">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="89801-1459">Az.DataLakeStore</span></span>
* <span data-ttu-id="89801-1460">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="89801-1460">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="89801-1461">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="89801-1461">Az.HealthcareApis</span></span>
* <span data-ttu-id="89801-1462">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="89801-1462">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="89801-1463">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="89801-1463">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="89801-1464">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="89801-1464">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="89801-1465">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="89801-1465">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="89801-1466">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="89801-1466">Az.IotHub</span></span>
* <span data-ttu-id="89801-1467">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="89801-1467">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="89801-1468">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="89801-1468">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="89801-1469">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="89801-1469">Az.Monitor</span></span>
* <span data-ttu-id="89801-1470">Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="89801-1470">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="89801-1471">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="89801-1471">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="89801-1472">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="89801-1472">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="89801-1473">Os Webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="89801-1473">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-1474">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-1474">Az.Network</span></span>
* <span data-ttu-id="89801-1475">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="89801-1475">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="89801-1476">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="89801-1476">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="89801-1477">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="89801-1477">New cmdlets added:</span></span>
        - <span data-ttu-id="89801-1478">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="89801-1478">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="89801-1479">Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="89801-1479">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="89801-1480">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="89801-1480">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="89801-1481">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="89801-1481">Updated cmdlets:</span></span>
        - <span data-ttu-id="89801-1482">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="89801-1482">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="89801-1483">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="89801-1483">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="89801-1484">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="89801-1484">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="89801-1485">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="89801-1485">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="89801-1486">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="89801-1486">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="89801-1487">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="89801-1487">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="89801-1488">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="89801-1488">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="89801-1489">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="89801-1489">Az.RedisCache</span></span>
* <span data-ttu-id="89801-1490">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="89801-1490">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-1491">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-1491">Az.Sql</span></span>
* <span data-ttu-id="89801-1492">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="89801-1492">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-1493">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-1493">Az.Storage</span></span>
* <span data-ttu-id="89801-1494">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="89801-1494">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="89801-1495">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="89801-1495">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="89801-1496">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="89801-1496">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="89801-1497">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="89801-1497">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="89801-1498">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="89801-1498">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="89801-1499">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="89801-1499">Az.StorageSync</span></span>
* <span data-ttu-id="89801-1500">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="89801-1500">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="89801-1501">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-1501">Az.Websites</span></span>
* <span data-ttu-id="89801-1502">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="89801-1502">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="89801-1503">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-1503">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="89801-1504">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="89801-1504">Az.ApiManagement</span></span>
* <span data-ttu-id="89801-1505">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="89801-1505">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="89801-1506">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="89801-1506">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="89801-1507">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="89801-1507">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="89801-1508">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="89801-1508">Az.Automation</span></span>
* <span data-ttu-id="89801-1509">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="89801-1509">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="89801-1510">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="89801-1510">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="89801-1511">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="89801-1511">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-1512">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-1512">Az.Compute</span></span>
* <span data-ttu-id="89801-1513">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="89801-1513">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="89801-1514">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="89801-1514">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="89801-1515">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="89801-1515">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="89801-1516">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="89801-1516">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="89801-1517">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="89801-1517">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="89801-1518">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="89801-1518">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="89801-1519">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="89801-1519">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="89801-1520">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="89801-1520">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="89801-1521">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="89801-1521">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="89801-1522">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="89801-1522">Az.DataFactory</span></span>
* <span data-ttu-id="89801-1523">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="89801-1523">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="89801-1524">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="89801-1524">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="89801-1525">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="89801-1525">Az.HDInsight</span></span>
* <span data-ttu-id="89801-1526">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="89801-1526">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="89801-1527">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="89801-1527">Az.IotHub</span></span>
* <span data-ttu-id="89801-1528">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="89801-1528">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="89801-1529">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="89801-1529">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="89801-1530">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="89801-1530">New cmdlets are:</span></span>
    - <span data-ttu-id="89801-1531">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="89801-1531">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="89801-1532">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="89801-1532">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="89801-1533">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="89801-1533">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="89801-1534">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="89801-1534">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="89801-1535">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="89801-1535">Az.Monitor</span></span>
* <span data-ttu-id="89801-1536">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="89801-1536">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="89801-1537">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="89801-1537">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="89801-1538">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="89801-1538">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="89801-1539">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="89801-1539">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="89801-1540">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="89801-1540">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="89801-1541">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="89801-1541">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="89801-1542">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="89801-1542">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="89801-1543">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="89801-1543">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="89801-1544">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="89801-1544">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="89801-1545">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="89801-1545">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="89801-1546">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="89801-1546">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="89801-1547">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="89801-1547">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="89801-1548">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="89801-1548">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="89801-1549">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="89801-1549">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="89801-1550">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="89801-1550">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="89801-1551">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="89801-1551">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="89801-1552">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="89801-1552">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="89801-1553">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="89801-1553">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="89801-1554">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="89801-1554">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="89801-1555">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="89801-1555">Overall improved help files</span></span>
* <span data-ttu-id="89801-1556">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="89801-1556">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-1557">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-1557">Az.Network</span></span>
* <span data-ttu-id="89801-1558">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="89801-1558">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span>
* <span data-ttu-id="89801-1559">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="89801-1559">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="89801-1560">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="89801-1560">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="89801-1561">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="89801-1561">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="89801-1562">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="89801-1562">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="89801-1563">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="89801-1563">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="89801-1564">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="89801-1564">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="89801-1565">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="89801-1565">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="89801-1566">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="89801-1566">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="89801-1567">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="89801-1567">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="89801-1568">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="89801-1568">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="89801-1569">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="89801-1569">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="89801-1570">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="89801-1570">New cmdlets</span></span>
        - <span data-ttu-id="89801-1571">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="89801-1571">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="89801-1572">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="89801-1572">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="89801-1573">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="89801-1573">Updated cmdlet:</span></span>
        - <span data-ttu-id="89801-1574">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="89801-1574">New-VpnSite</span></span>
        - <span data-ttu-id="89801-1575">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="89801-1575">Update-VpnSite</span></span>
        - <span data-ttu-id="89801-1576">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="89801-1576">New-VpnConnection</span></span>
        - <span data-ttu-id="89801-1577">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="89801-1577">Update-VpnConnection</span></span>
* <span data-ttu-id="89801-1578">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="89801-1578">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-1579">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-1579">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-1580">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="89801-1580">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="89801-1581">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="89801-1581">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-1582">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-1582">Az.Resources</span></span>
* <span data-ttu-id="89801-1583">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="89801-1583">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="89801-1584">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="89801-1584">Az.ServiceFabric</span></span>
* <span data-ttu-id="89801-1585">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="89801-1585">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="89801-1586">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="89801-1586">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="89801-1587">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="89801-1587">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="89801-1588">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="89801-1588">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="89801-1589">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="89801-1589">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="89801-1590">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="89801-1590">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="89801-1591">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="89801-1591">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="89801-1592">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="89801-1592">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="89801-1593">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="89801-1593">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="89801-1594">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="89801-1594">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="89801-1595">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="89801-1595">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="89801-1596">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="89801-1596">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="89801-1597">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="89801-1597">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="89801-1598">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="89801-1598">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="89801-1599">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="89801-1599">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="89801-1600">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="89801-1600">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="89801-1601">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="89801-1601">Az.SignalR</span></span>
* <span data-ttu-id="89801-1602">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="89801-1602">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-1603">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-1603">Az.Sql</span></span>
* <span data-ttu-id="89801-1604">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="89801-1604">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="89801-1605">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="89801-1605">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="89801-1606">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="89801-1606">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="89801-1607">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="89801-1607">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="89801-1608">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="89801-1608">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-1609">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-1609">Az.Storage</span></span>
* <span data-ttu-id="89801-1610">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="89801-1610">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="89801-1611">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="89801-1611">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="89801-1612">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="89801-1612">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="89801-1613">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="89801-1613">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="89801-1614">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="89801-1614">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="89801-1615">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="89801-1615">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="89801-1616">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="89801-1616">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="89801-1617">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="89801-1617">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="89801-1618">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="89801-1618">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="89801-1619">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="89801-1619">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="89801-1620">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="89801-1620">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="89801-1621">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-1621">Az.Websites</span></span>
* <span data-ttu-id="89801-1622">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="89801-1622">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="89801-1623">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="89801-1623">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="89801-1624">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="89801-1624">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="89801-1625">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-1625">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="89801-1626">Geral</span><span class="sxs-lookup"><span data-stu-id="89801-1626">General</span></span>
* <span data-ttu-id="89801-1627">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="89801-1627">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="89801-1628">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-1628">Az.Accounts</span></span>
* <span data-ttu-id="89801-1629">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="89801-1629">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="89801-1630">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="89801-1630">Az.Aks</span></span>
* <span data-ttu-id="89801-1631">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="89801-1631">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="89801-1632">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="89801-1632">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="89801-1633">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="89801-1633">Az.ApiManagement</span></span>
* <span data-ttu-id="89801-1634">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="89801-1634">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="89801-1635">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="89801-1635">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="89801-1636">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="89801-1636">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="89801-1637">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="89801-1637">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="89801-1638">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="89801-1638">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="89801-1639">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="89801-1639">Az.Batch</span></span>
* <span data-ttu-id="89801-1640">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="89801-1640">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="89801-1641">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="89801-1641">Az.Cdn</span></span>
* <span data-ttu-id="89801-1642">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="89801-1642">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-1643">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-1643">Az.Compute</span></span>
* <span data-ttu-id="89801-1644">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="89801-1644">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="89801-1645">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="89801-1645">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="89801-1646">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="89801-1646">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="89801-1647">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="89801-1647">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="89801-1648">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="89801-1648">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="89801-1649">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="89801-1649">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="89801-1650">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="89801-1650">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="89801-1651">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="89801-1651">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="89801-1652">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="89801-1652">Az.DataFactory</span></span>
* <span data-ttu-id="89801-1653">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="89801-1653">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="89801-1654">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="89801-1654">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="89801-1655">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="89801-1655">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="89801-1656">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="89801-1656">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="89801-1657">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="89801-1657">Az.DataLakeStore</span></span>
* <span data-ttu-id="89801-1658">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="89801-1658">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="89801-1659">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="89801-1659">Az.EventHub</span></span>
* <span data-ttu-id="89801-1660">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="89801-1660">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="89801-1661">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="89801-1661">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="89801-1662">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="89801-1662">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="89801-1663">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="89801-1663">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="89801-1664">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="89801-1664">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="89801-1665">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="89801-1665">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="89801-1666">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="89801-1666">Az.Monitor</span></span>
* <span data-ttu-id="89801-1667">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="89801-1667">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-1668">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-1668">Az.Network</span></span>
* <span data-ttu-id="89801-1669">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="89801-1669">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="89801-1670">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="89801-1670">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="89801-1671">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="89801-1671">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="89801-1672">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="89801-1672">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="89801-1673">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="89801-1673">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span>
* <span data-ttu-id="89801-1674">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="89801-1674">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="89801-1675">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="89801-1675">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="89801-1676">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="89801-1676">Az.OperationalInsights</span></span>
* <span data-ttu-id="89801-1677">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="89801-1677">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="89801-1678">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="89801-1678">Added example</span></span>
    - <span data-ttu-id="89801-1679">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="89801-1679">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="89801-1680">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="89801-1680">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="89801-1681">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="89801-1681">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-1682">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-1682">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-1683">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="89801-1683">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-1684">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-1684">Az.Resources</span></span>
* <span data-ttu-id="89801-1685">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="89801-1685">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="89801-1686">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="89801-1686">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="89801-1687">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="89801-1687">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="89801-1688">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="89801-1688">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="89801-1689">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="89801-1689">Az.ServiceBus</span></span>
* <span data-ttu-id="89801-1690">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="89801-1690">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="89801-1691">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="89801-1691">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="89801-1692">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="89801-1692">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="89801-1693">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="89801-1693">Az.ServiceFabric</span></span>
* <span data-ttu-id="89801-1694">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="89801-1694">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="89801-1695">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="89801-1695">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="89801-1696">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="89801-1696">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="89801-1697">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="89801-1697">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="89801-1698">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="89801-1698">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="89801-1699">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="89801-1699">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-1700">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-1700">Az.Sql</span></span>
* <span data-ttu-id="89801-1701">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="89801-1701">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-1702">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-1702">Az.Storage</span></span>
* <span data-ttu-id="89801-1703">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="89801-1703">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="89801-1704">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="89801-1704">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="89801-1705">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="89801-1705">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="89801-1706">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="89801-1706">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="89801-1707">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="89801-1707">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="89801-1708">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="89801-1708">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="89801-1709">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-1709">Az.Websites</span></span>
* <span data-ttu-id="89801-1710">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="89801-1710">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="89801-1711">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-1711">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="89801-1712">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-1712">Az.Accounts</span></span>
* <span data-ttu-id="89801-1713">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="89801-1713">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="89801-1714">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="89801-1714">Az.ApplicationInsights</span></span>
* <span data-ttu-id="89801-1715">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="89801-1715">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span>

#### <a name="azautomation"></a><span data-ttu-id="89801-1716">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="89801-1716">Az.Automation</span></span>
* <span data-ttu-id="89801-1717">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="89801-1717">Fix typo in resource string</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="89801-1718">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="89801-1718">Az.CognitiveServices</span></span>
* <span data-ttu-id="89801-1719">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="89801-1719">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-1720">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-1720">Az.Compute</span></span>
* <span data-ttu-id="89801-1721">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="89801-1721">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="89801-1722">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="89801-1722">Az.ContainerRegistry</span></span>
* <span data-ttu-id="89801-1723">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="89801-1723">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="89801-1724">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="89801-1724">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="89801-1725">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="89801-1725">Az.DataFactory</span></span>
* <span data-ttu-id="89801-1726">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="89801-1726">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="89801-1727">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="89801-1727">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="89801-1728">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="89801-1728">Az.EventHub</span></span>
* <span data-ttu-id="89801-1729">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="89801-1729">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="89801-1730">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="89801-1730">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="89801-1731">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="89801-1731">Az.KeyVault</span></span>
* <span data-ttu-id="89801-1732">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="89801-1732">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="89801-1733">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="89801-1733">Az.LogicApp</span></span>
* <span data-ttu-id="89801-1734">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="89801-1734">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="89801-1735">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="89801-1735">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="89801-1736">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="89801-1736">Az.ManagedServices</span></span>
* <span data-ttu-id="89801-1737">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="89801-1737">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-1738">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-1738">Az.Network</span></span>
* <span data-ttu-id="89801-1739">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="89801-1739">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="89801-1740">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="89801-1740">New cmdlets</span></span>
        - <span data-ttu-id="89801-1741">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="89801-1741">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="89801-1742">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="89801-1742">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="89801-1743">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="89801-1743">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="89801-1744">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="89801-1744">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="89801-1745">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="89801-1745">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="89801-1746">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="89801-1746">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="89801-1747">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="89801-1747">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="89801-1748">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="89801-1748">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="89801-1749">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="89801-1749">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="89801-1750">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="89801-1750">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="89801-1751">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="89801-1751">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="89801-1752">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="89801-1752">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="89801-1753">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="89801-1753">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="89801-1754">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="89801-1754">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="89801-1755">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="89801-1755">Updated cmdlets</span></span>
        - <span data-ttu-id="89801-1756">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="89801-1756">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="89801-1757">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="89801-1757">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="89801-1758">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="89801-1758">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="89801-1759">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="89801-1759">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="89801-1760">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="89801-1760">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="89801-1761">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="89801-1761">Updated cmdlet:</span></span>
        - <span data-ttu-id="89801-1762">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="89801-1762">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="89801-1763">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="89801-1763">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="89801-1764">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="89801-1764">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="89801-1765">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="89801-1765">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="89801-1766">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="89801-1766">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="89801-1767">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="89801-1767">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="89801-1768">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="89801-1768">Az.OperationalInsights</span></span>
* <span data-ttu-id="89801-1769">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="89801-1769">Updated default version for saved searches to be 1.</span></span>
* <span data-ttu-id="89801-1770">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="89801-1770">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-1771">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-1771">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-1772">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="89801-1772">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="89801-1773">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="89801-1773">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="89801-1774">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="89801-1774">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="89801-1775">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="89801-1775">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="89801-1776">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="89801-1776">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="89801-1777">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="89801-1777">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="89801-1778">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="89801-1778">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="89801-1779">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="89801-1779">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="89801-1780">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="89801-1780">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="89801-1781">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="89801-1781">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-1782">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-1782">Az.Resources</span></span>
- <span data-ttu-id="89801-1783">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="89801-1783">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="89801-1784">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="89801-1784">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="89801-1785">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="89801-1785">Az.ServiceBus</span></span>
* <span data-ttu-id="89801-1786">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="89801-1786">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="89801-1787">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="89801-1787">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-1788">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-1788">Az.Sql</span></span>
* <span data-ttu-id="89801-1789">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="89801-1789">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="89801-1790">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="89801-1790">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="89801-1791">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="89801-1791">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-1792">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-1792">Az.Storage</span></span>
* <span data-ttu-id="89801-1793">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="89801-1793">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="89801-1794">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="89801-1794">Az.StorageSync</span></span>
* <span data-ttu-id="89801-1795">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="89801-1795">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="89801-1796">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="89801-1796">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="89801-1797">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-1797">Az.Websites</span></span>
* <span data-ttu-id="89801-1798">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="89801-1798">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="89801-1799">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="89801-1799">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="89801-1800">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="89801-1800">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="89801-1801">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-1801">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="89801-1802">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-1802">Az.Accounts</span></span>
* <span data-ttu-id="89801-1803">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="89801-1803">Add support for profile cmdlets</span></span>
* <span data-ttu-id="89801-1804">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="89801-1804">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="89801-1805">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="89801-1805">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="89801-1806">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="89801-1806">Az.Advisor</span></span>
* <span data-ttu-id="89801-1807">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="89801-1807">GA release of Az.Advisor</span></span>
* <span data-ttu-id="89801-1808">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="89801-1808">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="89801-1809">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="89801-1809">Az.ApiManagement</span></span>
* <span data-ttu-id="89801-1810">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="89801-1810">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="89801-1811">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="89801-1811">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="89801-1812">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="89801-1812">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="89801-1813">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="89801-1813">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="89801-1814">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="89801-1814">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="89801-1815">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="89801-1815">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="89801-1816">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="89801-1816">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="89801-1817">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="89801-1817">Az.Automation</span></span>
* <span data-ttu-id="89801-1818">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="89801-1818">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-1819">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-1819">Az.Compute</span></span>
* <span data-ttu-id="89801-1820">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="89801-1820">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="89801-1821">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="89801-1821">Az.DataFactory</span></span>
* <span data-ttu-id="89801-1822">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="89801-1822">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="89801-1823">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="89801-1823">Az.EventGrid</span></span>
* <span data-ttu-id="89801-1824">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="89801-1824">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="89801-1825">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="89801-1825">Az.IotHub</span></span>
* <span data-ttu-id="89801-1826">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="89801-1826">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-1827">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-1827">Az.Network</span></span>
* <span data-ttu-id="89801-1828">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="89801-1828">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="89801-1829">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="89801-1829">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="89801-1830">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="89801-1830">Az.PolicyInsights</span></span>
* <span data-ttu-id="89801-1831">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="89801-1831">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="89801-1832">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="89801-1832">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="89801-1833">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="89801-1833">Az.OperationalInsights</span></span>
* <span data-ttu-id="89801-1834">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="89801-1834">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-1835">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-1835">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-1836">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="89801-1836">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-1837">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-1837">Az.Resources</span></span>
    - <span data-ttu-id="89801-1838">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="89801-1838">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="89801-1839">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="89801-1839">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="89801-1840">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="89801-1840">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="89801-1841">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="89801-1841">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="89801-1842">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="89801-1842">Az.ServiceBus</span></span>
* <span data-ttu-id="89801-1843">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="89801-1843">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-1844">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-1844">Az.Sql</span></span>
* <span data-ttu-id="89801-1845">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="89801-1845">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="89801-1846">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="89801-1846">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="89801-1847">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="89801-1847">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="89801-1848">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="89801-1848">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="89801-1849">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="89801-1849">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="89801-1850">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="89801-1850">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="89801-1851">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="89801-1851">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="89801-1852">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="89801-1852">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="89801-1853">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="89801-1853">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-1854">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-1854">Az.Storage</span></span>
* <span data-ttu-id="89801-1855">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="89801-1855">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="89801-1856">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="89801-1856">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="89801-1857">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="89801-1857">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="89801-1858">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="89801-1858">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="89801-1859">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="89801-1859">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="89801-1860">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="89801-1860">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="89801-1861">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="89801-1861">Set-AzStorageAccount</span></span>
* <span data-ttu-id="89801-1862">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="89801-1862">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="89801-1863">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="89801-1863">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="89801-1864">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="89801-1864">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="89801-1865">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="89801-1865">Az.StorageSync</span></span>
* <span data-ttu-id="89801-1866">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="89801-1866">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="89801-1867">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-1867">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="89801-1868">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-1868">Az.Accounts</span></span>
* <span data-ttu-id="89801-1869">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="89801-1869">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="89801-1870">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="89801-1870">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="89801-1871">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="89801-1871">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="89801-1872">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="89801-1872">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="89801-1873">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="89801-1873">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-1874">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-1874">Az.Compute</span></span>
* <span data-ttu-id="89801-1875">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="89801-1875">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="89801-1876">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="89801-1876">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="89801-1877">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="89801-1877">Az.Dns</span></span>
* <span data-ttu-id="89801-1878">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="89801-1878">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="89801-1879">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="89801-1879">Az.EventGrid</span></span>
* <span data-ttu-id="89801-1880">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="89801-1880">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="89801-1881">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="89801-1881">New cmdlets:</span></span>
    - <span data-ttu-id="89801-1882">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="89801-1882">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="89801-1883">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="89801-1883">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="89801-1884">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="89801-1884">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="89801-1885">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-1885">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="89801-1886">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="89801-1886">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="89801-1887">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="89801-1887">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="89801-1888">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="89801-1888">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="89801-1889">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="89801-1889">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="89801-1890">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="89801-1890">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="89801-1891">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="89801-1891">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="89801-1892">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="89801-1892">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="89801-1893">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="89801-1893">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="89801-1894">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="89801-1894">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="89801-1895">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="89801-1895">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span>
    - <span data-ttu-id="89801-1896">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="89801-1896">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="89801-1897">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="89801-1897">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="89801-1898">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="89801-1898">Updated cmdlets:</span></span>
    - <span data-ttu-id="89801-1899">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="89801-1899">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="89801-1900">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="89801-1900">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="89801-1901">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="89801-1901">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="89801-1902">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="89801-1902">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="89801-1903">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="89801-1903">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="89801-1904">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="89801-1904">Event subscription expiration date,</span></span>
            - <span data-ttu-id="89801-1905">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="89801-1905">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="89801-1906">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="89801-1906">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="89801-1907">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="89801-1907">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span>
    - <span data-ttu-id="89801-1908">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="89801-1908">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="89801-1909">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="89801-1909">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="89801-1910">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="89801-1910">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="89801-1911">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="89801-1911">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="89801-1912">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="89801-1912">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="89801-1913">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="89801-1913">Az.FrontDoor</span></span>
* <span data-ttu-id="89801-1914">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="89801-1914">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="89801-1915">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="89801-1915">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="89801-1916">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="89801-1916">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="89801-1917">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="89801-1917">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-1918">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-1918">Az.Network</span></span>
* <span data-ttu-id="89801-1919">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="89801-1919">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="89801-1920">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="89801-1920">New cmdlets</span></span>
        - <span data-ttu-id="89801-1921">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="89801-1921">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="89801-1922">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="89801-1922">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="89801-1923">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="89801-1923">New cmdlets</span></span>
        - <span data-ttu-id="89801-1924">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="89801-1924">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="89801-1925">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="89801-1925">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="89801-1926">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="89801-1926">New cmdlets</span></span>
        - <span data-ttu-id="89801-1927">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="89801-1927">Get-AzPrivateLinkService</span></span>
        - <span data-ttu-id="89801-1928">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="89801-1928">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="89801-1929">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="89801-1929">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="89801-1930">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="89801-1930">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="89801-1931">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="89801-1931">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="89801-1932">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="89801-1932">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="89801-1933">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="89801-1933">New cmdlets</span></span>
        - <span data-ttu-id="89801-1934">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="89801-1934">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="89801-1935">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="89801-1935">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="89801-1936">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="89801-1936">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="89801-1937">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="89801-1937">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="89801-1938">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="89801-1938">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="89801-1939">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="89801-1939">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="89801-1940">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="89801-1940">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="89801-1941">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="89801-1941">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="89801-1942">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="89801-1942">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="89801-1943">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="89801-1943">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="89801-1944">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="89801-1944">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="89801-1945">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="89801-1945">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="89801-1946">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="89801-1946">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="89801-1947">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="89801-1947">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="89801-1948">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="89801-1948">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="89801-1949">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="89801-1949">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="89801-1950">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="89801-1950">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="89801-1951">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="89801-1951">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="89801-1952">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="89801-1952">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="89801-1953">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="89801-1953">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="89801-1954">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="89801-1954">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="89801-1955">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="89801-1955">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="89801-1956">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="89801-1956">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span>
* <span data-ttu-id="89801-1957">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="89801-1957">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span>
    - <span data-ttu-id="89801-1958">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="89801-1958">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="89801-1959">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="89801-1959">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="89801-1960">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="89801-1960">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="89801-1961">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="89801-1961">Az.OperationalInsights</span></span>
* <span data-ttu-id="89801-1962">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="89801-1962">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-1963">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-1963">Az.Resources</span></span>
* <span data-ttu-id="89801-1964">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="89801-1964">Support for additional Template Export options</span></span>
    - <span data-ttu-id="89801-1965">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="89801-1965">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="89801-1966">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="89801-1966">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="89801-1967">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="89801-1967">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="89801-1968">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="89801-1968">Az.ServiceFabric</span></span>
* <span data-ttu-id="89801-1969">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="89801-1969">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-1970">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-1970">Az.Sql</span></span>
* <span data-ttu-id="89801-1971">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="89801-1971">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="89801-1972">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="89801-1972">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="89801-1973">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="89801-1973">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="89801-1974">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="89801-1974">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="89801-1975">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="89801-1975">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="89801-1976">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="89801-1976">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="89801-1977">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="89801-1977">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="89801-1978">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="89801-1978">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-1979">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-1979">Az.Storage</span></span>
* <span data-ttu-id="89801-1980">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="89801-1980">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="89801-1981">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="89801-1981">New-AzStorageAccount</span></span>
* <span data-ttu-id="89801-1982">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="89801-1982">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="89801-1983">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="89801-1983">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="89801-1984">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-1984">Az.Websites</span></span>
* <span data-ttu-id="89801-1985">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="89801-1985">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="89801-1986">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="89801-1986">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="89801-1987">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-1987">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="89801-1988">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="89801-1988">Az.Cdn</span></span>
* <span data-ttu-id="89801-1989">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="89801-1989">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-1990">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-1990">Az.Compute</span></span>
* <span data-ttu-id="89801-1991">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="89801-1991">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="89801-1992">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="89801-1992">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="89801-1993">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="89801-1993">Az.EventHub</span></span>
* <span data-ttu-id="89801-1994">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="89801-1994">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="89801-1995">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="89801-1995">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-1996">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-1996">Az.Network</span></span>
* <span data-ttu-id="89801-1997">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="89801-1997">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="89801-1998">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="89801-1998">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="89801-1999">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="89801-1999">Az.PolicyInsights</span></span>
* <span data-ttu-id="89801-2000">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="89801-2000">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-2001">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-2001">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-2002">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="89801-2002">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="89801-2003">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="89801-2003">Az.ServiceBus</span></span>
* <span data-ttu-id="89801-2004">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="89801-2004">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="89801-2005">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="89801-2005">Az.ServiceFabric</span></span>
* <span data-ttu-id="89801-2006">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="89801-2006">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="89801-2007">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="89801-2007">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-2008">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-2008">Az.Sql</span></span>
* <span data-ttu-id="89801-2009">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="89801-2009">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="89801-2010">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="89801-2010">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="89801-2011">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="89801-2011">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="89801-2012">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="89801-2012">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="89801-2013">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-2013">Az.Websites</span></span>
* <span data-ttu-id="89801-2014">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="89801-2014">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="89801-2015">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-2015">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="89801-2016">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="89801-2016">Az.ApiManagement</span></span>
* <span data-ttu-id="89801-2017">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="89801-2017">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="89801-2018">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="89801-2018">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="89801-2019">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="89801-2019">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="89801-2020">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="89801-2020">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="89801-2021">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="89801-2021">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="89801-2022">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="89801-2022">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="89801-2023">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="89801-2023">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="89801-2024">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="89801-2024">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="89801-2025">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="89801-2025">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="89801-2026">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="89801-2026">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="89801-2027">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="89801-2027">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="89801-2028">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="89801-2028">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="89801-2029">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="89801-2029">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="89801-2030">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="89801-2030">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="89801-2031">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="89801-2031">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="89801-2032">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="89801-2032">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="89801-2033">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="89801-2033">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="89801-2034">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="89801-2034">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="89801-2035">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="89801-2035">Created new Cmdlet for generating a User Token.</span></span>
    - <span data-ttu-id="89801-2036">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="89801-2036">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="89801-2037">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="89801-2037">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="89801-2038">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="89801-2038">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="89801-2039">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="89801-2039">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="89801-2040">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="89801-2040">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span>
    - <span data-ttu-id="89801-2041">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="89801-2041">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="89801-2042">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="89801-2042">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="89801-2043">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="89801-2043">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="89801-2044">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="89801-2044">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="89801-2045">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="89801-2045">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="89801-2046">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="89801-2046">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="89801-2047">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="89801-2047">Updated the cmdlet to display Error Messages inline</span></span>
     > <span data-ttu-id="89801-2048">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="89801-2048">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="89801-2049">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="89801-2049">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="89801-2050">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="89801-2050">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="89801-2051">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="89801-2051">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="89801-2052">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="89801-2052">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="89801-2053">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="89801-2053">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="89801-2054">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="89801-2054">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="89801-2055">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="89801-2055">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="89801-2056">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="89801-2056">Updated cmdlet **New-AzApiManagementApi**</span></span>
    - <span data-ttu-id="89801-2057">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="89801-2057">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="89801-2058">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="89801-2058">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="89801-2059">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="89801-2059">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="89801-2060">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="89801-2060">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="89801-2061">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="89801-2061">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="89801-2062">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="89801-2062">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="89801-2063">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="89801-2063">To updated an API into an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="89801-2064">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="89801-2064">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="89801-2065">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="89801-2065">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="89801-2066">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="89801-2066">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="89801-2067">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="89801-2067">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="89801-2068">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="89801-2068">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="89801-2069">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="89801-2069">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="89801-2070">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="89801-2070">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="89801-2071">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="89801-2071">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="89801-2072">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="89801-2072">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="89801-2073">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="89801-2073">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="89801-2074">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="89801-2074">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="89801-2075">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="89801-2075">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="89801-2076">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="89801-2076">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="89801-2077">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="89801-2077">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="89801-2078">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="89801-2078">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="89801-2079">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="89801-2079">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="89801-2080">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="89801-2080">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="89801-2081">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="89801-2081">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="89801-2082">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="89801-2082">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="89801-2083">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="89801-2083">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="89801-2084">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="89801-2084">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="89801-2085">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="89801-2085">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="89801-2086">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="89801-2086">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="89801-2087">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="89801-2087">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="89801-2088">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="89801-2088">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="89801-2089">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="89801-2089">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="89801-2090">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="89801-2090">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="89801-2091">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="89801-2091">'Get-AzApiManagementCertificate'</span></span>
    - <span data-ttu-id="89801-2092">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="89801-2092">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="89801-2093">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="89801-2093">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="89801-2094">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="89801-2094">Az.Automation</span></span>
* <span data-ttu-id="89801-2095">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="89801-2095">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="89801-2096">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="89801-2096">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="89801-2097">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="89801-2097">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="89801-2098">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="89801-2098">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="89801-2099">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="89801-2099">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="89801-2100">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="89801-2100">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="89801-2101">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="89801-2101">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-2102">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-2102">Az.Compute</span></span>
* <span data-ttu-id="89801-2103">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="89801-2103">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="89801-2104">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="89801-2104">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="89801-2105">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="89801-2105">Az.DataLakeStore</span></span>
* <span data-ttu-id="89801-2106">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="89801-2106">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="89801-2107">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="89801-2107">Az.Monitor</span></span>
* <span data-ttu-id="89801-2108">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="89801-2108">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-2109">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-2109">Az.Network</span></span>
* <span data-ttu-id="89801-2110">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="89801-2110">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="89801-2111">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="89801-2111">Updated cmdlet:</span></span>
        - <span data-ttu-id="89801-2112">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="89801-2112">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="89801-2113">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="89801-2113">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-2114">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-2114">Az.Resources</span></span>
* <span data-ttu-id="89801-2115">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="89801-2115">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-2116">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-2116">Az.Sql</span></span>
* <span data-ttu-id="89801-2117">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="89801-2117">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="89801-2118">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-2118">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="89801-2119">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-2119">Az.Accounts</span></span>
* <span data-ttu-id="89801-2120">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="89801-2120">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="89801-2121">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="89801-2121">Az.CognitiveServices</span></span>
* <span data-ttu-id="89801-2122">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="89801-2122">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="89801-2123">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="89801-2123">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-2124">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-2124">Az.Compute</span></span>
* <span data-ttu-id="89801-2125">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="89801-2125">Proximity placement group feature.</span></span>
    - <span data-ttu-id="89801-2126">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="89801-2126">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="89801-2127">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="89801-2127">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="89801-2128">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="89801-2128">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="89801-2129">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="89801-2129">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="89801-2130">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="89801-2130">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>
* <span data-ttu-id="89801-2131">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="89801-2131">Breaking changes</span></span>
    - <span data-ttu-id="89801-2132">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="89801-2132">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="89801-2133">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="89801-2133">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="89801-2134">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="89801-2134">Az.DeploymentManager</span></span>
* <span data-ttu-id="89801-2135">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="89801-2135">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="89801-2136">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="89801-2136">Az.Dns</span></span>
* <span data-ttu-id="89801-2137">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="89801-2137">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="89801-2138">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="89801-2138">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="89801-2139">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="89801-2139">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="89801-2140">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="89801-2140">Az.FrontDoor</span></span>
* <span data-ttu-id="89801-2141">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="89801-2141">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="89801-2142">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="89801-2142">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="89801-2143">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="89801-2143">Az.HDInsight</span></span>
* <span data-ttu-id="89801-2144">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="89801-2144">Removed two cmdlets:</span></span>
    - <span data-ttu-id="89801-2145">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="89801-2145">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="89801-2146">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="89801-2146">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="89801-2147">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="89801-2147">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="89801-2148">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="89801-2148">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="89801-2149">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="89801-2149">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="89801-2150">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="89801-2150">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="89801-2151">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="89801-2151">Az.Monitor</span></span>
* <span data-ttu-id="89801-2152">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="89801-2152">New cmdlets for SQR API (Scheduled Query Rule)</span></span>
    - <span data-ttu-id="89801-2153">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="89801-2153">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="89801-2154">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="89801-2154">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="89801-2155">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="89801-2155">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="89801-2156">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="89801-2156">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="89801-2157">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="89801-2157">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="89801-2158">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="89801-2158">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="89801-2159">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="89801-2159">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="89801-2160">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="89801-2160">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="89801-2161">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="89801-2161">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="89801-2162">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="89801-2162">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="89801-2163">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="89801-2163">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="89801-2164">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="89801-2164">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="89801-2165">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="89801-2165">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-2166">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-2166">Az.Network</span></span>
* <span data-ttu-id="89801-2167">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="89801-2167">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="89801-2168">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="89801-2168">New cmdlets</span></span>
        - <span data-ttu-id="89801-2169">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="89801-2169">New-AzNatGateway</span></span>
        - <span data-ttu-id="89801-2170">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="89801-2170">Get-AzNatGateway</span></span>
        - <span data-ttu-id="89801-2171">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="89801-2171">Set-AzNatGateway</span></span>
        - <span data-ttu-id="89801-2172">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="89801-2172">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="89801-2173">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="89801-2173">Updated cmdlets</span></span>
        - <span data-ttu-id="89801-2174">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="89801-2174">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="89801-2175">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="89801-2175">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="89801-2176">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="89801-2176">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="89801-2177">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="89801-2177">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="89801-2178">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="89801-2178">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="89801-2179">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="89801-2179">Az.PolicyInsights</span></span>
* <span data-ttu-id="89801-2180">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="89801-2180">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="89801-2181">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="89801-2181">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="89801-2182">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="89801-2182">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-2183">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-2183">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-2184">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="89801-2184">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="89801-2185">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="89801-2185">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="89801-2186">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="89801-2186">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="89801-2187">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-2187">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="89801-2188">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="89801-2188">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="89801-2189">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="89801-2189">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="89801-2190">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="89801-2190">Az.Relay</span></span>
* <span data-ttu-id="89801-2191">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="89801-2191">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="89801-2192">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="89801-2192">Az.ServiceBus</span></span>
* <span data-ttu-id="89801-2193">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="89801-2193">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-2194">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-2194">Az.Storage</span></span>
* <span data-ttu-id="89801-2195">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="89801-2195">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="89801-2196">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="89801-2196">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="89801-2197">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="89801-2197">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="89801-2198">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="89801-2198">New-AzStorageAccount</span></span>
* <span data-ttu-id="89801-2199">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="89801-2199">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="89801-2200">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="89801-2200">New-AzStorageAccount</span></span>
    - <span data-ttu-id="89801-2201">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="89801-2201">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="89801-2202">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="89801-2202">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="89801-2203">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-2203">Az.Websites</span></span>
* <span data-ttu-id="89801-2204">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="89801-2204">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="89801-2205">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="89801-2205">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="89801-2206">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-2206">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="89801-2207">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="89801-2207">Highlights since the last major release</span></span>
* <span data-ttu-id="89801-2208">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="89801-2208">General availability of `Az` module</span></span>
* <span data-ttu-id="89801-2209">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="89801-2209">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="89801-2210">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="89801-2210">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="89801-2211">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-2211">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="89801-2212">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="89801-2212">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="89801-2213">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="89801-2213">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="89801-2214">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="89801-2214">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="89801-2215">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-2215">Az.Accounts</span></span>
* <span data-ttu-id="89801-2216">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="89801-2216">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="89801-2217">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="89801-2217">Az.Batch</span></span>
* <span data-ttu-id="89801-2218">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="89801-2218">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="89801-2219">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="89801-2219">Az.Cdn</span></span>
* <span data-ttu-id="89801-2220">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="89801-2220">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="89801-2221">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="89801-2221">Az.CognitiveServices</span></span>
* <span data-ttu-id="89801-2222">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="89801-2222">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-2223">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-2223">Az.Compute</span></span>
* <span data-ttu-id="89801-2224">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="89801-2224">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="89801-2225">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="89801-2225">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="89801-2226">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="89801-2226">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="89801-2227">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="89801-2227">Az.DataFactory</span></span>
* <span data-ttu-id="89801-2228">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="89801-2228">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="89801-2229">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="89801-2229">Az.DataLakeStore</span></span>
* <span data-ttu-id="89801-2230">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="89801-2230">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="89801-2231">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="89801-2231">Az.EventGrid</span></span>
* <span data-ttu-id="89801-2232">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="89801-2232">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="89801-2233">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="89801-2233">Az.EventHub</span></span>
* <span data-ttu-id="89801-2234">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="89801-2234">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="89801-2235">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="89801-2235">Az.HDInsight</span></span>
* <span data-ttu-id="89801-2236">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="89801-2236">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="89801-2237">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="89801-2237">Az.IotHub</span></span>
* <span data-ttu-id="89801-2238">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="89801-2238">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="89801-2239">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="89801-2239">Az.KeyVault</span></span>
* <span data-ttu-id="89801-2240">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="89801-2240">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="89801-2241">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="89801-2241">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="89801-2242">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="89801-2242">Az.MachineLearning</span></span>
* <span data-ttu-id="89801-2243">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="89801-2243">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="89801-2244">Az.Media</span><span class="sxs-lookup"><span data-stu-id="89801-2244">Az.Media</span></span>
* <span data-ttu-id="89801-2245">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="89801-2245">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="89801-2246">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="89801-2246">Az.Monitor</span></span>
  * <span data-ttu-id="89801-2247">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="89801-2247">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="89801-2248">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="89801-2248">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="89801-2249">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="89801-2249">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="89801-2250">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="89801-2250">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="89801-2251">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="89801-2251">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="89801-2252">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="89801-2252">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="89801-2253">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="89801-2253">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-2254">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-2254">Az.Network</span></span>
* <span data-ttu-id="89801-2255">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="89801-2255">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="89801-2256">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="89801-2256">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="89801-2257">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="89801-2257">Az.NotificationHubs</span></span>
* <span data-ttu-id="89801-2258">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="89801-2258">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="89801-2259">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="89801-2259">Az.OperationalInsights</span></span>
* <span data-ttu-id="89801-2260">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="89801-2260">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="89801-2261">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="89801-2261">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="89801-2262">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="89801-2262">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-2263">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-2263">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-2264">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="89801-2264">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="89801-2265">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="89801-2265">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="89801-2266">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="89801-2266">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="89801-2267">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="89801-2267">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="89801-2268">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="89801-2268">Az.RedisCache</span></span>
* <span data-ttu-id="89801-2269">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="89801-2269">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-2270">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-2270">Az.Resources</span></span>
* <span data-ttu-id="89801-2271">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="89801-2271">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-2272">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-2272">Az.Sql</span></span>
* <span data-ttu-id="89801-2273">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="89801-2273">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="89801-2274">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="89801-2274">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="89801-2275">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="89801-2275">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="89801-2276">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="89801-2276">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="89801-2277">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="89801-2277">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="89801-2278">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="89801-2278">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="89801-2279">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="89801-2279">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="89801-2280">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-2280">Az.Websites</span></span>
* <span data-ttu-id="89801-2281">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="89801-2281">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="89801-2282">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="89801-2282">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="89801-2283">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="89801-2283">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="89801-2284">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="89801-2284">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="89801-2285">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-2285">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="89801-2286">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="89801-2286">Highlights since the last major release</span></span>
* <span data-ttu-id="89801-2287">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="89801-2287">General availability of `Az` module</span></span>
* <span data-ttu-id="89801-2288">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="89801-2288">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="89801-2289">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="89801-2289">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="89801-2290">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-2290">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="89801-2291">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="89801-2291">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="89801-2292">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="89801-2292">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="89801-2293">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="89801-2293">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="89801-2294">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-2294">Az.Accounts</span></span>
* <span data-ttu-id="89801-2295">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="89801-2295">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="89801-2296">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="89801-2296">Az.AnalysisServices</span></span>
* <span data-ttu-id="89801-2297">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="89801-2297">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="89801-2298">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="89801-2298">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="89801-2299">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="89801-2299">Az.Automation</span></span>
* <span data-ttu-id="89801-2300">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="89801-2300">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="89801-2301">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="89801-2301">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="89801-2302">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="89801-2302">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-2303">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-2303">Az.Compute</span></span>
* <span data-ttu-id="89801-2304">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="89801-2304">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="89801-2305">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="89801-2305">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="89801-2306">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="89801-2306">Az.ContainerInstance</span></span>
* <span data-ttu-id="89801-2307">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="89801-2307">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="89801-2308">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="89801-2308">Az.DataFactory</span></span>
* <span data-ttu-id="89801-2309">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="89801-2309">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="89801-2310">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="89801-2310">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-2311">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-2311">Az.Resources</span></span>
* <span data-ttu-id="89801-2312">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="89801-2312">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="89801-2313">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="89801-2313">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="89801-2314">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="89801-2314">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="89801-2315">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="89801-2315">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="89801-2316">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="89801-2316">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="89801-2317">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="89801-2317">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-2318">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-2318">Az.Sql</span></span>
* <span data-ttu-id="89801-2319">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="89801-2319">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-2320">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-2320">Az.Storage</span></span>
* <span data-ttu-id="89801-2321">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="89801-2321">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="89801-2322">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="89801-2322">New-AzStorageContext</span></span>
* <span data-ttu-id="89801-2323">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="89801-2323">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="89801-2324">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="89801-2324">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="89801-2325">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="89801-2325">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="89801-2326">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="89801-2326">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="89801-2327">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="89801-2327">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="89801-2328">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="89801-2328">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="89801-2329">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="89801-2329">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="89801-2330">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="89801-2330">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="89801-2331">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="89801-2331">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="89801-2332">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="89801-2332">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="89801-2333">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-2333">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="89801-2334">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="89801-2334">Highlights since the last major release</span></span>
* <span data-ttu-id="89801-2335">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="89801-2335">General availability of `Az` module</span></span>
* <span data-ttu-id="89801-2336">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="89801-2336">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="89801-2337">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="89801-2337">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="89801-2338">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-2338">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="89801-2339">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="89801-2339">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="89801-2340">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="89801-2340">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="89801-2341">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="89801-2341">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="89801-2342">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="89801-2342">Az.Automation</span></span>
* <span data-ttu-id="89801-2343">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="89801-2343">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="89801-2344">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="89801-2344">Dynamic grouping</span></span>
    * <span data-ttu-id="89801-2345">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="89801-2345">Pre-Post script</span></span>
    * <span data-ttu-id="89801-2346">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="89801-2346">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-2347">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-2347">Az.Compute</span></span>
* <span data-ttu-id="89801-2348">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="89801-2348">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="89801-2349">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="89801-2349">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="89801-2350">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="89801-2350">Az.KeyVault</span></span>
* <span data-ttu-id="89801-2351">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="89801-2351">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-2352">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-2352">Az.Network</span></span>
* <span data-ttu-id="89801-2353">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="89801-2353">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="89801-2354">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="89801-2354">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-2355">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-2355">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-2356">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="89801-2356">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="89801-2357">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="89801-2357">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-2358">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-2358">Az.Resources</span></span>
* <span data-ttu-id="89801-2359">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="89801-2359">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="89801-2360">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="89801-2360">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-2361">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-2361">Az.Sql</span></span>
* <span data-ttu-id="89801-2362">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="89801-2362">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-2363">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-2363">Az.Storage</span></span>
* <span data-ttu-id="89801-2364">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="89801-2364">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="89801-2365">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="89801-2365">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="89801-2366">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="89801-2366">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="89801-2367">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="89801-2367">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="89801-2368">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="89801-2368">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="89801-2369">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="89801-2369">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="89801-2370">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="89801-2370">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="89801-2371">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-2371">Az.Websites</span></span>
* <span data-ttu-id="89801-2372">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="89801-2372">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="89801-2373">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-2373">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="89801-2374">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-2374">Az.Accounts</span></span>
* <span data-ttu-id="89801-2375">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="89801-2375">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="89801-2376">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="89801-2376">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="89801-2377">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="89801-2377">Az.Automation</span></span>
* <span data-ttu-id="89801-2378">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="89801-2378">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="89801-2379">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="89801-2379">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="89801-2380">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="89801-2380">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="89801-2381">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="89801-2381">Az.Cdn</span></span>
* <span data-ttu-id="89801-2382">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="89801-2382">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-2383">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-2383">Az.Compute</span></span>
* <span data-ttu-id="89801-2384">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="89801-2384">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="89801-2385">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="89801-2385">Az.DataFactory</span></span>
* <span data-ttu-id="89801-2386">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="89801-2386">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="89801-2387">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="89801-2387">Az.LogicApp</span></span>
* <span data-ttu-id="89801-2388">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="89801-2388">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-2389">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-2389">Az.Network</span></span>
* <span data-ttu-id="89801-2390">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="89801-2390">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-2391">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-2391">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-2392">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="89801-2392">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="89801-2393">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="89801-2393">SDK Update</span></span>
* <span data-ttu-id="89801-2394">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="89801-2394">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="89801-2395">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="89801-2395">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-2396">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-2396">Az.Resources</span></span>
* <span data-ttu-id="89801-2397">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="89801-2397">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="89801-2398">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="89801-2398">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="89801-2399">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="89801-2399">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="89801-2400">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="89801-2400">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="89801-2401">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="89801-2401">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="89801-2402">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="89801-2402">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-2403">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-2403">Az.Sql</span></span>
* <span data-ttu-id="89801-2404">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="89801-2404">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="89801-2405">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="89801-2405">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-2406">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-2406">Az.Storage</span></span>
* <span data-ttu-id="89801-2407">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="89801-2407">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="89801-2408">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-2408">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="89801-2409">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="89801-2409">Az.AnalysisServices</span></span>
* <span data-ttu-id="89801-2410">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="89801-2410">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="89801-2411">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="89801-2411">Az.Automation</span></span>
* <span data-ttu-id="89801-2412">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="89801-2412">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="89801-2413">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="89801-2413">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="89801-2414">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="89801-2414">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="89801-2415">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="89801-2415">Az.CognitiveServices</span></span>
* <span data-ttu-id="89801-2416">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="89801-2416">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-2417">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-2417">Az.Compute</span></span>
* <span data-ttu-id="89801-2418">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="89801-2418">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="89801-2419">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="89801-2419">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="89801-2420">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="89801-2420">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="89801-2421">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="89801-2421">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="89801-2422">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="89801-2422">Az.DataLakeStore</span></span>
* <span data-ttu-id="89801-2423">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="89801-2423">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="89801-2424">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="89801-2424">Az.EventHub</span></span>
* <span data-ttu-id="89801-2425">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="89801-2425">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="89801-2426">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="89801-2426">Az.KeyVault</span></span>
* <span data-ttu-id="89801-2427">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="89801-2427">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="89801-2428">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="89801-2428">Az.LogicApp</span></span>
* <span data-ttu-id="89801-2429">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="89801-2429">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="89801-2430">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="89801-2430">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="89801-2431">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="89801-2431">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="89801-2432">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="89801-2432">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="89801-2433">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="89801-2433">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="89801-2434">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="89801-2434">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="89801-2435">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="89801-2435">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="89801-2436">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="89801-2436">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="89801-2437">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="89801-2437">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="89801-2438">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="89801-2438">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="89801-2439">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="89801-2439">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="89801-2440">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="89801-2440">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="89801-2441">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="89801-2441">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="89801-2442">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="89801-2442">Az.Monitor</span></span>
* <span data-ttu-id="89801-2443">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="89801-2443">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-2444">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-2444">Az.Network</span></span>
* <span data-ttu-id="89801-2445">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="89801-2445">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="89801-2446">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="89801-2446">Az.OperationalInsights</span></span>
* <span data-ttu-id="89801-2447">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="89801-2447">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="89801-2448">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="89801-2448">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="89801-2449">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="89801-2449">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-2450">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-2450">Az.Resources</span></span>
* <span data-ttu-id="89801-2451">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="89801-2451">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="89801-2452">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="89801-2452">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="89801-2453">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="89801-2453">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="89801-2454">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="89801-2454">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-2455">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-2455">Az.Sql</span></span>
* <span data-ttu-id="89801-2456">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="89801-2456">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="89801-2457">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="89801-2457">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="89801-2458">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-2458">Az.Websites</span></span>
* <span data-ttu-id="89801-2459">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="89801-2459">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="89801-2460">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-2460">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="89801-2461">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-2461">Az.Accounts</span></span>
* <span data-ttu-id="89801-2462">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="89801-2462">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="89801-2463">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="89801-2463">Az.AnalysisServices</span></span>
<span data-ttu-id="89801-2464">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="89801-2464">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-2465">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-2465">Az.Compute</span></span>
* <span data-ttu-id="89801-2466">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="89801-2466">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="89801-2467">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="89801-2467">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="89801-2468">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="89801-2468">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-2469">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-2469">Az.RecoveryServices</span></span>
<span data-ttu-id="89801-2470">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="89801-2470">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-2471">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-2471">Az.Resources</span></span>
* <span data-ttu-id="89801-2472">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="89801-2472">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="89801-2473">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="89801-2473">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="89801-2474">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="89801-2474">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="89801-2475">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="89801-2475">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-2476">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-2476">Az.Sql</span></span>
* <span data-ttu-id="89801-2477">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="89801-2477">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="89801-2478">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="89801-2478">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="89801-2479">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="89801-2479">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="89801-2480">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-2480">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="89801-2481">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-2481">Az.Accounts</span></span>
* <span data-ttu-id="89801-2482">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="89801-2482">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="89801-2483">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="89801-2483">Az.AnalysisServices</span></span>
* <span data-ttu-id="89801-2484">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="89801-2484">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="89801-2485">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-2485">Az.RecoveryServices</span></span>
* <span data-ttu-id="89801-2486">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="89801-2486">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="89801-2487">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-2487">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="89801-2488">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-2488">Az.Accounts</span></span>
* <span data-ttu-id="89801-2489">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="89801-2489">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="89801-2490">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="89801-2490">Update incorrect online help URLs</span></span>
* <span data-ttu-id="89801-2491">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="89801-2491">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="89801-2492">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="89801-2492">Az.Aks</span></span>
* <span data-ttu-id="89801-2493">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="89801-2493">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="89801-2494">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="89801-2494">Az.Automation</span></span>
* <span data-ttu-id="89801-2495">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="89801-2495">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="89801-2496">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="89801-2496">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="89801-2497">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="89801-2497">Az.Cdn</span></span>
* <span data-ttu-id="89801-2498">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="89801-2498">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-2499">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-2499">Az.Compute</span></span>
* <span data-ttu-id="89801-2500">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="89801-2500">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="89801-2501">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="89801-2501">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="89801-2502">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="89801-2502">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="89801-2503">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="89801-2503">Az.ContainerRegistry</span></span>
* <span data-ttu-id="89801-2504">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="89801-2504">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="89801-2505">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="89801-2505">Az.DataFactory</span></span>
* <span data-ttu-id="89801-2506">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="89801-2506">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="89801-2507">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="89801-2507">Az.DataLakeStore</span></span>
* <span data-ttu-id="89801-2508">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="89801-2508">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="89801-2509">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="89801-2509">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="89801-2510">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="89801-2510">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="89801-2511">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="89801-2511">Az.IotHub</span></span>
* <span data-ttu-id="89801-2512">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="89801-2512">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="89801-2513">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="89801-2513">Az.KeyVault</span></span>
* <span data-ttu-id="89801-2514">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="89801-2514">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-2515">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-2515">Az.Network</span></span>
* <span data-ttu-id="89801-2516">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="89801-2516">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-2517">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-2517">Az.Resources</span></span>
* <span data-ttu-id="89801-2518">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="89801-2518">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="89801-2519">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="89801-2519">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="89801-2520">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="89801-2520">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="89801-2521">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="89801-2521">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="89801-2522">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="89801-2522">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="89801-2523">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="89801-2523">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="89801-2524">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="89801-2524">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="89801-2525">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="89801-2525">Az.ServiceFabric</span></span>
* <span data-ttu-id="89801-2526">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="89801-2526">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="89801-2527">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="89801-2527">Fix some error messages.</span></span>
* <span data-ttu-id="89801-2528">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="89801-2528">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="89801-2529">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="89801-2529">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="89801-2530">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="89801-2530">Az.SignalR</span></span>
* <span data-ttu-id="89801-2531">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="89801-2531">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-2532">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-2532">Az.Sql</span></span>
* <span data-ttu-id="89801-2533">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="89801-2533">Update incorrect online help URLs</span></span>
* <span data-ttu-id="89801-2534">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="89801-2534">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="89801-2535">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="89801-2535">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="89801-2536">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="89801-2536">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-2537">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-2537">Az.Storage</span></span>
* <span data-ttu-id="89801-2538">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="89801-2538">Update incorrect online help URLs</span></span>
* <span data-ttu-id="89801-2539">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="89801-2539">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="89801-2540">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="89801-2540">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="89801-2541">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="89801-2541">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="89801-2542">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="89801-2542">Az.TrafficManager</span></span>
* <span data-ttu-id="89801-2543">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="89801-2543">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="89801-2544">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-2544">Az.Websites</span></span>
* <span data-ttu-id="89801-2545">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="89801-2545">Update incorrect online help URLs</span></span>
* <span data-ttu-id="89801-2546">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="89801-2546">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="89801-2547">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="89801-2547">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="89801-2548">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="89801-2548">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="89801-2549">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-2549">Az.Accounts</span></span>
* <span data-ttu-id="89801-2550">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="89801-2550">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-2551">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-2551">Az.Compute</span></span>
* <span data-ttu-id="89801-2552">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="89801-2552">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="89801-2553">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="89801-2553">Updated the description of ID in help files</span></span>
* <span data-ttu-id="89801-2554">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-2554">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="89801-2555">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="89801-2555">Az.DataLakeStore</span></span>
* <span data-ttu-id="89801-2556">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="89801-2556">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="89801-2557">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="89801-2557">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="89801-2558">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="89801-2558">Az.EventGrid</span></span>
* <span data-ttu-id="89801-2559">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="89801-2559">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="89801-2560">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="89801-2560">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="89801-2561">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="89801-2561">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="89801-2562">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="89801-2562">Event Time-To-Live,</span></span>
        - <span data-ttu-id="89801-2563">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="89801-2563">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="89801-2564">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="89801-2564">Dead letter endpoint.</span></span>
    - <span data-ttu-id="89801-2565">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="89801-2565">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="89801-2566">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="89801-2566">Event Time-To-Live,</span></span>
        - <span data-ttu-id="89801-2567">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="89801-2567">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="89801-2568">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="89801-2568">Dead letter endpoint.</span></span>
* <span data-ttu-id="89801-2569">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="89801-2569">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="89801-2570">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="89801-2570">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="89801-2571">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="89801-2571">Az.IotHub</span></span>
* <span data-ttu-id="89801-2572">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="89801-2572">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="89801-2573">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="89801-2573">Az.LogicApp</span></span>
* <span data-ttu-id="89801-2574">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="89801-2574">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-2575">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-2575">Az.Resources</span></span>
* <span data-ttu-id="89801-2576">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="89801-2576">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="89801-2577">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="89801-2577">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="89801-2578">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="89801-2578">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="89801-2579">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="89801-2579">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="89801-2580">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="89801-2580">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="89801-2581">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="89801-2581">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="89801-2582">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="89801-2582">Az.SignalR</span></span>
* <span data-ttu-id="89801-2583">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-2583">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-2584">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-2584">Az.Sql</span></span>
* <span data-ttu-id="89801-2585">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="89801-2585">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="89801-2586">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-2586">Az.Storage</span></span>
* <span data-ttu-id="89801-2587">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="89801-2587">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="89801-2588">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="89801-2588">New-AzStorageContext</span></span>
* <span data-ttu-id="89801-2589">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="89801-2589">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="89801-2590">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="89801-2590">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="89801-2591">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-2591">Az.Websites</span></span>
* <span data-ttu-id="89801-2592">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="89801-2592">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="89801-2593">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-2593">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="89801-2594">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="89801-2594">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="89801-2595">Geral</span><span class="sxs-lookup"><span data-stu-id="89801-2595">General</span></span>

- <span data-ttu-id="89801-2596">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="89801-2596">General Availability of Az Module</span></span>
- <span data-ttu-id="89801-2597">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="89801-2597">Online help for each module</span></span>
- <span data-ttu-id="89801-2598">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="89801-2598">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="89801-2599">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="89801-2599">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="89801-2600">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-2600">Az.Accounts</span></span>
- <span data-ttu-id="89801-2601">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="89801-2601">Changed from Az.Profile</span></span>
- <span data-ttu-id="89801-2602">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="89801-2602">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="89801-2603">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="89801-2603">Az.ApiManagement</span></span>
- <span data-ttu-id="89801-2604">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="89801-2604">Fixes for #7002</span></span>
- <span data-ttu-id="89801-2605">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="89801-2605">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="89801-2606">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="89801-2606">Az.Batch</span></span>
- <span data-ttu-id="89801-2607">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="89801-2607">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="89801-2608">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="89801-2608">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="89801-2609">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="89801-2609">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="89801-2610">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="89801-2610">Az.Billing</span></span>
- <span data-ttu-id="89801-2611">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="89801-2611">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="89801-2612">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="89801-2612">Az.CognitivServices</span></span>
- <span data-ttu-id="89801-2613">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="89801-2613">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="89801-2614">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="89801-2614">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="89801-2615">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="89801-2615">Az.ContainerInstance</span></span>
- <span data-ttu-id="89801-2616">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="89801-2616">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="89801-2617">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="89801-2617">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="89801-2618">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="89801-2618">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="89801-2619">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="89801-2619">Az.DataLakeStore</span></span>
- <span data-ttu-id="89801-2620">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="89801-2620">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="89801-2621">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="89801-2621">Az.Monitor</span></span>
- <span data-ttu-id="89801-2622">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="89801-2622">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="89801-2623">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="89801-2623">Az.KeyVault</span></span>
- <span data-ttu-id="89801-2624">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="89801-2624">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="89801-2625">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="89801-2625">Az.MachineLearning</span></span>
- <span data-ttu-id="89801-2626">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="89801-2626">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="89801-2627">Az.Media</span><span class="sxs-lookup"><span data-stu-id="89801-2627">Az.Media</span></span>
- <span data-ttu-id="89801-2628">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="89801-2628">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="89801-2629">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-2629">Az.Network</span></span>
<span data-ttu-id="89801-2630">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="89801-2630">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="89801-2631">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="89801-2631">New cmdlets added:</span></span>
        - <span data-ttu-id="89801-2632">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="89801-2632">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="89801-2633">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="89801-2633">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="89801-2634">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="89801-2634">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="89801-2635">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="89801-2635">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="89801-2636">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="89801-2636">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="89801-2637">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="89801-2637">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="89801-2638">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="89801-2638">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="89801-2639">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="89801-2639">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="89801-2640">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="89801-2640">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="89801-2641">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="89801-2641">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="89801-2642">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="89801-2642">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="89801-2643">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="89801-2643">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="89801-2644">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="89801-2644">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="89801-2645">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="89801-2645">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="89801-2646">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="89801-2646">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="89801-2647">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="89801-2647">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="89801-2648">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="89801-2648">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="89801-2649">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="89801-2649">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="89801-2650">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="89801-2650">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="89801-2651">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="89801-2651">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="89801-2652">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="89801-2652">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="89801-2653">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="89801-2653">Az.OperationalInsights</span></span>
- <span data-ttu-id="89801-2654">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="89801-2654">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="89801-2655">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="89801-2655">Az.Profile</span></span>
- <span data-ttu-id="89801-2656">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="89801-2656">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="89801-2657">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-2657">Az.RecoveryServices</span></span>
- <span data-ttu-id="89801-2658">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="89801-2658">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="89801-2659">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-2659">Az.Resources</span></span>
- <span data-ttu-id="89801-2660">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="89801-2660">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="89801-2661">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="89801-2661">Az.ServiceFabric</span></span>
- <span data-ttu-id="89801-2662">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="89801-2662">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="89801-2663">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="89801-2663">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="89801-2664">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="89801-2664">Az.SIgnalR</span></span>
- <span data-ttu-id="89801-2665">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="89801-2665">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="89801-2666">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-2666">Az.Sql</span></span>
- <span data-ttu-id="89801-2667">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="89801-2667">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="89801-2668">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="89801-2668">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="89801-2669">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="89801-2669">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="89801-2670">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-2670">Az.Storage</span></span>
- <span data-ttu-id="89801-2671">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="89801-2671">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="89801-2672">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-2672">Az.Websites</span></span>
- <span data-ttu-id="89801-2673">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="89801-2673">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="89801-2674">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="89801-2674">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="89801-2675">Geral</span><span class="sxs-lookup"><span data-stu-id="89801-2675">General</span></span>

* <span data-ttu-id="89801-2676">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="89801-2676">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="89801-2677">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-2677">Az.Compute</span></span>

* <span data-ttu-id="89801-2678">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="89801-2678">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="89801-2679">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="89801-2679">Az.DataLakeStore</span></span>

* <span data-ttu-id="89801-2680">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="89801-2680">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="89801-2681">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="89801-2681">Az.FrontDoor</span></span>

* <span data-ttu-id="89801-2682">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="89801-2682">Fixed some broken links</span></span>
    - <span data-ttu-id="89801-2683">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="89801-2683">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="89801-2684">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="89801-2684">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="89801-2685">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="89801-2685">Az.RecoveryServices</span></span>

* <span data-ttu-id="89801-2686">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-2686">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="89801-2687">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="89801-2687">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="89801-2688">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-2688">Az.Resources</span></span>

* <span data-ttu-id="89801-2689">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="89801-2689">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="89801-2690">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="89801-2690">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="89801-2691">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-2691">Az.Sql</span></span>

* <span data-ttu-id="89801-2692">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="89801-2692">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="89801-2693">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="89801-2693">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="89801-2694">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="89801-2694">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="89801-2695">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-2695">Az.Storage</span></span>

* <span data-ttu-id="89801-2696">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="89801-2696">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="89801-2697">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="89801-2697">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="89801-2698">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="89801-2698">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="89801-2699">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="89801-2699">Support Static Website configuration</span></span>
    - <span data-ttu-id="89801-2700">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="89801-2700">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="89801-2701">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="89801-2701">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="89801-2702">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-2702">Az.Websites</span></span>

* <span data-ttu-id="89801-2703">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="89801-2703">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="89801-2704">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="89801-2704">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="89801-2705">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-2705">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="89801-2706">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="89801-2706">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="89801-2707">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="89801-2707">Az.ApiManagement</span></span>
* <span data-ttu-id="89801-2708">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="89801-2708">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="89801-2709">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="89801-2709">Az.Automation</span></span>
* <span data-ttu-id="89801-2710">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="89801-2710">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="89801-2711">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="89801-2711">Added Update Management cmdlets</span></span>
* <span data-ttu-id="89801-2712">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="89801-2712">Added Source Control cmdlets</span></span>
* <span data-ttu-id="89801-2713">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="89801-2713">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="89801-2714">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="89801-2714">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="89801-2715">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-2715">Az.Compute</span></span>
* <span data-ttu-id="89801-2716">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="89801-2716">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="89801-2717">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="89801-2717">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="89801-2718">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="89801-2718">Az.ContainerInstance</span></span>
* <span data-ttu-id="89801-2719">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="89801-2719">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="89801-2720">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="89801-2720">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="89801-2721">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="89801-2721">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="89801-2722">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-2722">Az.Network</span></span>
* <span data-ttu-id="89801-2723">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="89801-2723">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="89801-2724">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="89801-2724">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="89801-2725">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="89801-2725">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="89801-2726">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="89801-2726">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="89801-2727">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="89801-2727">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="89801-2728">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="89801-2728">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="89801-2729">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="89801-2729">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="89801-2730">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="89801-2730">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="89801-2731">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="89801-2731">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="89801-2732">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="89801-2732">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="89801-2733">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="89801-2733">Az.Relay</span></span>
* <span data-ttu-id="89801-2734">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="89801-2734">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="89801-2735">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-2735">Az.Resources</span></span>
* <span data-ttu-id="89801-2736">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="89801-2736">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="89801-2737">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="89801-2737">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="89801-2738">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="89801-2738">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="89801-2739">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="89801-2739">Az.ServiceFabric</span></span>
* <span data-ttu-id="89801-2740">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="89801-2740">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="89801-2741">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-2741">Az.Sql</span></span>
* <span data-ttu-id="89801-2742">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="89801-2742">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="89801-2743">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="89801-2743">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="89801-2744">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="89801-2744">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="89801-2745">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="89801-2745">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="89801-2746">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="89801-2746">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="89801-2747">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="89801-2747">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="89801-2748">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="89801-2748">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="89801-2749">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="89801-2749">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="89801-2750">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="89801-2750">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="89801-2751">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="89801-2751">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="89801-2752">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="89801-2752">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="89801-2753">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="89801-2753">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="89801-2754">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="89801-2754">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="89801-2755">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="89801-2755">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="89801-2756">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="89801-2756">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="89801-2757">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="89801-2757">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="89801-2758">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="89801-2758">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="89801-2759">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="89801-2759">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="89801-2760">Geral</span><span class="sxs-lookup"><span data-stu-id="89801-2760">General</span></span>
* <span data-ttu-id="89801-2761">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="89801-2761">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="89801-2762">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="89801-2762">Az.Profile</span></span>
* <span data-ttu-id="89801-2763">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="89801-2763">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="89801-2764">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="89801-2764">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="89801-2765">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="89801-2765">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="89801-2766">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="89801-2766">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="89801-2767">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="89801-2767">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="89801-2768">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="89801-2768">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="89801-2769">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="89801-2769">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="89801-2770">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="89801-2770">Az.CognitiveServices</span></span>
* <span data-ttu-id="89801-2771">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="89801-2771">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-2772">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-2772">Az.Compute</span></span>
* <span data-ttu-id="89801-2773">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="89801-2773">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="89801-2774">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="89801-2774">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="89801-2775">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="89801-2775">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="89801-2776">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="89801-2776">Az.DataLakeStore</span></span>
* <span data-ttu-id="89801-2777">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="89801-2777">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="89801-2778">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="89801-2778">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="89801-2779">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="89801-2779">Az.Insights</span></span>
* <span data-ttu-id="89801-2780">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="89801-2780">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="89801-2781">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="89801-2781">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="89801-2782">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="89801-2782">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="89801-2783">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="89801-2783">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-2784">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-2784">Az.Network</span></span>
* <span data-ttu-id="89801-2785">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="89801-2785">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="89801-2786">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="89801-2786">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="89801-2787">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="89801-2787">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="89801-2788">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="89801-2788">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="89801-2789">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="89801-2789">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="89801-2790">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="89801-2790">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="89801-2791">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="89801-2791">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="89801-2792">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="89801-2792">Az.PolicyInsights</span></span>
* <span data-ttu-id="89801-2793">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="89801-2793">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-2794">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-2794">Az.Resources</span></span>
* <span data-ttu-id="89801-2795">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="89801-2795">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="89801-2796">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="89801-2796">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="89801-2797">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="89801-2797">Az.ServiceBus</span></span>
* <span data-ttu-id="89801-2798">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="89801-2798">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="89801-2799">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="89801-2799">Az.ServiceFabric</span></span>
* <span data-ttu-id="89801-2800">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="89801-2800">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="89801-2801">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="89801-2801">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="89801-2802">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="89801-2802">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="89801-2803">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="89801-2803">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="89801-2804">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="89801-2804">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="89801-2805">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="89801-2805">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="89801-2806">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="89801-2806">Az.Profile</span></span>
* <span data-ttu-id="89801-2807">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="89801-2807">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="89801-2808">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="89801-2808">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-2809">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-2809">Az.Compute</span></span>
* <span data-ttu-id="89801-2810">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="89801-2810">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="89801-2811">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="89801-2811">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="89801-2812">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="89801-2812">Az.DataLakeStore</span></span>
* <span data-ttu-id="89801-2813">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="89801-2813">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="89801-2814">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-2814">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="89801-2815">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="89801-2815">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="89801-2816">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="89801-2816">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="89801-2817">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="89801-2817">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-2818">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-2818">Az.Network</span></span>
* <span data-ttu-id="89801-2819">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="89801-2819">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="89801-2820">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="89801-2820">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-2821">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-2821">Az.Resources</span></span>
* <span data-ttu-id="89801-2822">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="89801-2822">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="89801-2823">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="89801-2823">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="89801-2824">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="89801-2824">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="89801-2825">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="89801-2825">Azure.Storage</span></span>
* <span data-ttu-id="89801-2826">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="89801-2826">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="89801-2827">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="89801-2827">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="89801-2828">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="89801-2828">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="89801-2829">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="89801-2829">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="89801-2830">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="89801-2830">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="89801-2831">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="89801-2831">Az.CognitiveServices</span></span>
* <span data-ttu-id="89801-2832">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="89801-2832">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="89801-2833">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="89801-2833">Az.Compute</span></span>
* <span data-ttu-id="89801-2834">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="89801-2834">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="89801-2835">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="89801-2835">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="89801-2836">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="89801-2836">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="89801-2837">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="89801-2837">Az.DataFactoryV2</span></span>
* <span data-ttu-id="89801-2838">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="89801-2838">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="89801-2839">Az.Network</span><span class="sxs-lookup"><span data-stu-id="89801-2839">Az.Network</span></span>
* <span data-ttu-id="89801-2840">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="89801-2840">Added NetworkProfile functionality.</span></span> <span data-ttu-id="89801-2841">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="89801-2841">new cmdlets added</span></span>
    - <span data-ttu-id="89801-2842">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="89801-2842">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="89801-2843">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="89801-2843">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="89801-2844">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="89801-2844">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="89801-2845">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="89801-2845">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="89801-2846">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="89801-2846">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="89801-2847">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="89801-2847">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="89801-2848">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="89801-2848">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="89801-2849">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="89801-2849">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="89801-2850">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="89801-2850">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="89801-2851">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="89801-2851">Az.RedisCache</span></span>
* <span data-ttu-id="89801-2852">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="89801-2852">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="89801-2853">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="89801-2853">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="89801-2854">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="89801-2854">Az.Resources</span></span>
* <span data-ttu-id="89801-2855">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="89801-2855">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="89801-2856">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="89801-2856">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="89801-2857">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="89801-2857">Az.Sql</span></span>
* <span data-ttu-id="89801-2858">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="89801-2858">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="89801-2859">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="89801-2859">Az.Websites</span></span>
* <span data-ttu-id="89801-2860">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="89801-2860">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="89801-2861">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="89801-2861">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="89801-2862">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="89801-2862">0.2.0 - September 2018</span></span>
 <span data-ttu-id="89801-2863">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="89801-2863">Initial Release</span></span>
