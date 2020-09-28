---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: 52129f31202a8ae04bf80988b5aa07b12fe081b8
ms.sourcegitcommit: 15f21c40dcb7610e2fbaaabf264ad925e4224500
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/22/2020
ms.locfileid: "90913395"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="c0450-103">Notas de versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c0450-103">Azure PowerShell release notes</span></span>

## <a name="460---august-2020"></a><span data-ttu-id="c0450-104">4.6.0 - Agosto de 2020</span><span class="sxs-lookup"><span data-stu-id="c0450-104">4.6.0 - August 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c0450-105">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-105">Az.Accounts</span></span>
* <span data-ttu-id="c0450-106">São carregados todos os ambientes de cloud pública quando o ponto final de deteção não devolve o AzureCloud predefinido ou outros ambientes públicos [#12633]</span><span class="sxs-lookup"><span data-stu-id="c0450-106">Loaded all public cloud environments when discovery endpoint doesn't return default AzureCloud or other public environments [#12633]</span></span>
* <span data-ttu-id="c0450-107">Exposição de SubscriptionPolicies em "Get-AzSubscription" [#12551]</span><span class="sxs-lookup"><span data-stu-id="c0450-107">Exposed SubscriptionPolicies in 'Get-AzSubscription' [#12551]</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c0450-108">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c0450-108">Az.Automation</span></span>
* <span data-ttu-id="c0450-109">Adição de parâmetros "-RunOn" a "Set-AzAutomationWebhook" para especificar um Grupo de Função de Trabalho Híbrida</span><span class="sxs-lookup"><span data-stu-id="c0450-109">Added '-RunOn' parameters to 'Set-AzAutomationWebhook' to specify a Hybrid Worker Group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-110">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-110">Az.Compute</span></span>
* <span data-ttu-id="c0450-111">Adição do parâmetro "-EncryptionAtHost" a "New-AzVm", "New-AzVmss", "New-AzVMConfig", "New-AzVmssConfig", "Update-AzVM" e "Update-AzVmss"</span><span class="sxs-lookup"><span data-stu-id="c0450-111">Added '-EncryptionAtHost' parameter to 'New-AzVm', 'New-AzVmss', 'New-AzVMConfig', 'New-AzVmssConfig', 'Update-AzVM', and 'Update-AzVmss'</span></span>
* <span data-ttu-id="c0450-112">Adição de "SecurityProfile" ao objeto de retorno "Get-AzVM" e "Get-AzVmss"</span><span class="sxs-lookup"><span data-stu-id="c0450-112">Added 'SecurityProfile' to 'Get-AzVM' and 'Get-AzVmss' return object</span></span>
* <span data-ttu-id="c0450-113">Adição do comutador "-InstanceView" como parâmetro opcional a "Get-AzHostGroup"</span><span class="sxs-lookup"><span data-stu-id="c0450-113">Added '-InstanceView' switch as optional parameter to 'Get-AzHostGroup'</span></span>
* <span data-ttu-id="c0450-114">Adição do novo cmdlet "Invoke-AzVmPatchAssessment"</span><span class="sxs-lookup"><span data-stu-id="c0450-114">Added new cmdlet 'Invoke-AzVmPatchAssessment'</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c0450-115">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c0450-115">Az.DataFactory</span></span>
* <span data-ttu-id="c0450-116">Adição das propriedades em falta à classe PSPipelineRun.</span><span class="sxs-lookup"><span data-stu-id="c0450-116">Added missing properties to PSPipelineRun class.</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c0450-117">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c0450-117">Az.HDInsight</span></span>
* <span data-ttu-id="c0450-118">É suportada a criação de clusters com encriptação na funcionalidade de anfitrião.</span><span class="sxs-lookup"><span data-stu-id="c0450-118">Supported creating cluster with encryption at host feature.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c0450-119">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0450-119">Az.KeyVault</span></span>
* <span data-ttu-id="c0450-120">Adição de mensagens de aviso para planear a desativação da eliminação recuperável</span><span class="sxs-lookup"><span data-stu-id="c0450-120">Added warning messages for planning to disable soft delete</span></span>
* <span data-ttu-id="c0450-121">Adição de mensagens de aviso para planear a remoção do atributo SecretValueText</span><span class="sxs-lookup"><span data-stu-id="c0450-121">Added warning messages for planning to remove attribute SecretValueText</span></span>

#### <a name="azmaintenance"></a><span data-ttu-id="c0450-122">Az.Maintenance</span><span class="sxs-lookup"><span data-stu-id="c0450-122">Az.Maintenance</span></span>
* <span data-ttu-id="c0450-123">Adição de campos relacionados com agendamento opcionais a "New-AzMaintenanceConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c0450-123">Added optional schedule related fields to 'New-AzMaintenanceConfiguration'</span></span>
* <span data-ttu-id="c0450-124">Adição do novo cmdlet para "Get-AzMaintenancePublicConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c0450-124">Added new cmdlet for 'Get-AzMaintenancePublicConfiguration'</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="c0450-125">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="c0450-125">Az.ManagedServices</span></span>
* <span data-ttu-id="c0450-126">Adição de avisos de alteração interruptiva nos cmdlets de atribuição e definição de serviços geridos</span><span class="sxs-lookup"><span data-stu-id="c0450-126">Added breaking change warnings on cmdlets of managed services assignment and definition</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c0450-127">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c0450-127">Az.Monitor</span></span>
* <span data-ttu-id="c0450-128">Expansão do parâmetro definido em "Set-AzDiagnosticSetting" para a separação da ativação de Registos e Métricas [#12482]</span><span class="sxs-lookup"><span data-stu-id="c0450-128">Extended the parameter set in 'Set-AzDiagnosticSetting' for separation of Logs and Metrics enablement [#12482]</span></span>
* <span data-ttu-id="c0450-129">Correção do erro de "Add-AzMetricAlertRuleV2" ao obter o alerta de métrica do pipeline</span><span class="sxs-lookup"><span data-stu-id="c0450-129">Fixed bug for 'Add-AzMetricAlertRuleV2' when getting metric alert from pipeline</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-130">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-130">Az.Resources</span></span>
* <span data-ttu-id="c0450-131">Atualização da resposta "Get-AzPolicyAlias" no sentido de incluir informações que indicam se o alias pode ser modificado pelo Azure Policy.</span><span class="sxs-lookup"><span data-stu-id="c0450-131">Updated 'Get-AzPolicyAlias' response to include information indicating whether the alias is modifiable by Azure Policy.</span></span>
* <span data-ttu-id="c0450-132">Criação do novo cmdlet "Set-AzRoleAssignment"</span><span class="sxs-lookup"><span data-stu-id="c0450-132">Created new cmdlet 'Set-AzRoleAssignment'</span></span>
* <span data-ttu-id="c0450-133">Adição de "Get-AzDeploymentManagementGroupWhatIfResult" para obter os resultados de Hipóteses do modelo do ARM no âmbito do Grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="c0450-133">Added 'Get-AzDeploymentManagementGroupWhatIfResult' for getting ARM template What-If results at management Group scope</span></span>
* <span data-ttu-id="c0450-134">Adição do novo cmdlet "Get-AzTenantWhatIfResult" para obter os resultados de Hipóteses do modelo do ARM no âmbito do inquilino</span><span class="sxs-lookup"><span data-stu-id="c0450-134">Added 'Get-AzTenantWhatIfResult' new cmdlet for getting ARM template What-If results at tenant scope</span></span>
* <span data-ttu-id="c0450-135">Substituição de "-WhatIf" e "-Confirm" por "New-AzManagementGroupDeployment" e "New-AzTenantDeployment" no sentido de utilizar os resultados de Hipóteses do modelo do ARM</span><span class="sxs-lookup"><span data-stu-id="c0450-135">Overrode '-WhatIf' and '-Confirm' for 'New-AzManagementGroupDeployment' and 'New-AzTenantDeployment' to use ARM template What-If results</span></span>
* <span data-ttu-id="c0450-136">Correção dos comportamentos de "-WhatIf" e "-Confirm" para os novos cmdlets de implementação para que estejam em conformidade com $WhatIfPreference e $ConfirmPreference.</span><span class="sxs-lookup"><span data-stu-id="c0450-136">Fixed the behaviors of '-WhatIf' and '-Confirm' for new deployment cmdlets so they comply with $WhatIfPreference and $ConfirmPreference.</span></span>
* <span data-ttu-id="c0450-137">Correção do erro de serialização de "-TemplateObject" e "TemplateParameterObject" [#1528] [#6292]</span><span class="sxs-lookup"><span data-stu-id="c0450-137">Fixed serialization error for '-TemplateObject' and 'TemplateParameterObject' [#1528] [#6292]</span></span>
* <span data-ttu-id="c0450-138">Adição do atributo de alteração interruptiva a "Get-AzResourceGroupDeploymentOperation" para a próxima alteração do tipo de saída</span><span class="sxs-lookup"><span data-stu-id="c0450-138">Added breaking change attribute to 'Get-AzResourceGroupDeploymentOperation' for the upcoming output type change</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="c0450-139">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="c0450-139">Az.SignalR</span></span>
* <span data-ttu-id="c0450-140">Correção dos erros dos ficheiros de ajuda "Restart-AzSignalR" e "Update-AzSignalR"</span><span class="sxs-lookup"><span data-stu-id="c0450-140">Fixed 'Restart-AzSignalR' and 'Update-AzSignalR' help files errors</span></span>
* <span data-ttu-id="c0450-141">Adição dos cmdlets "Update-AzSignalRNetworkAcl" e "Set-AzSignalRUpstream"</span><span class="sxs-lookup"><span data-stu-id="c0450-141">Added cmdlets 'Update-AzSignalRNetworkAcl', 'Set-AzSignalRUpstream'</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-142">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-142">Az.Storage</span></span>
* <span data-ttu-id="c0450-143">É suportada a aceleração da consulta de blobs</span><span class="sxs-lookup"><span data-stu-id="c0450-143">Supported blob query acceleration</span></span>
    -  <span data-ttu-id="c0450-144">"Get-AzStorageBlobQueryResult"</span><span class="sxs-lookup"><span data-stu-id="c0450-144">'Get-AzStorageBlobQueryResult'</span></span>
    -  <span data-ttu-id="c0450-145">"New-AzStorageBlobQueryConfig"</span><span class="sxs-lookup"><span data-stu-id="c0450-145">'New-AzStorageBlobQueryConfig'</span></span>
* <span data-ttu-id="c0450-146">Atualização do ficheiro de ajuda, com a adição de mais descrições e a correção de erros de digitação</span><span class="sxs-lookup"><span data-stu-id="c0450-146">Updated help file, added more description, and fixed typo</span></span>
    -  <span data-ttu-id="c0450-147">"Start-AzStorageBlobCopy"</span><span class="sxs-lookup"><span data-stu-id="c0450-147">'Start-AzStorageBlobCopy'</span></span>
    -  <span data-ttu-id="c0450-148">"Get-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="c0450-148">'Get-AzDataLakeGen2Item'</span></span>
* <span data-ttu-id="c0450-149">Correção da falha de transferência de blobs quando o subdiretório relacionado não existe [#12592]</span><span class="sxs-lookup"><span data-stu-id="c0450-149">Fixed download blob fail when related sub directory not exist [#12592]</span></span>
    -  <span data-ttu-id="c0450-150">"Get-AzStorageBlobContent"</span><span class="sxs-lookup"><span data-stu-id="c0450-150">'Get-AzStorageBlobContent'</span></span>
* <span data-ttu-id="c0450-151">É suportada a Política de Replicação Definir/Obter/Remover Objeto nas Contas de armazenamento</span><span class="sxs-lookup"><span data-stu-id="c0450-151">Supported Set/Get/Remove Object Replication Policy on Storage accounts</span></span>
    - <span data-ttu-id="c0450-152">"New-AzStorageObjectReplicationPolicyRule"</span><span class="sxs-lookup"><span data-stu-id="c0450-152">'New-AzStorageObjectReplicationPolicyRule'</span></span>
    - <span data-ttu-id="c0450-153">"Set-AzStorageObjectReplicationPolicy"</span><span class="sxs-lookup"><span data-stu-id="c0450-153">'Set-AzStorageObjectReplicationPolicy'</span></span>
    - <span data-ttu-id="c0450-154">"Get-AzStorageObjectReplicationPolicy"</span><span class="sxs-lookup"><span data-stu-id="c0450-154">'Get-AzStorageObjectReplicationPolicy'</span></span>
    - <span data-ttu-id="c0450-155">"Remove-AzStorageObjectReplicationPolicy"</span><span class="sxs-lookup"><span data-stu-id="c0450-155">'Remove-AzStorageObjectReplicationPolicy'</span></span>
* <span data-ttu-id="c0450-156">Suporte para ativar/desativar o ChangeFeed no Serviço Blob de uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="c0450-156">Supported enable/disable ChangeFeed on Blob Service of a Storage account</span></span>
    - <span data-ttu-id="c0450-157">"Update-AzStorageBlobServiceProperty"</span><span class="sxs-lookup"><span data-stu-id="c0450-157">'Update-AzStorageBlobServiceProperty'</span></span>

## <a name="450---august-2020"></a><span data-ttu-id="c0450-158">4.5.0 - Agosto de 2020</span><span class="sxs-lookup"><span data-stu-id="c0450-158">4.5.0 - August 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c0450-159">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-159">Az.Accounts</span></span>
* <span data-ttu-id="c0450-160">"Connect-AzAccount" atualizado para aceitar o parâmetro "MaxContextPopulation" [#9865]</span><span class="sxs-lookup"><span data-stu-id="c0450-160">Updated 'Connect-AzAccount' to accept parameter 'MaxContextPopulation' [#9865]</span></span>
* <span data-ttu-id="c0450-161">Versão de SubscriptionClient atualizada para a de 2019-06-01 e apresentação de domínios de inquilino [#9838]</span><span class="sxs-lookup"><span data-stu-id="c0450-161">Updated SubscriptionClient version to 2019-06-01 and display tenant domains [#9838]</span></span>
* <span data-ttu-id="c0450-162">Inquilino principal suportado e informações do inquilino managedBy da subscrição</span><span class="sxs-lookup"><span data-stu-id="c0450-162">Supported home tenant and managedBy tenant information of subscription</span></span>
* <span data-ttu-id="c0450-163">Nome do módulo corrigido, informações da versão nos dados telemétricos</span><span class="sxs-lookup"><span data-stu-id="c0450-163">Corrected module name, version info in telemetry data</span></span>
* <span data-ttu-id="c0450-164">SqlDatabaseDnsSuffix e ServiceManagementUrl ajustados se o ponto final dos metadados do ambiente devolverem valores incompatíveis</span><span class="sxs-lookup"><span data-stu-id="c0450-164">Adjusted SqlDatabaseDnsSuffix and ServiceManagementUrl if environment metadata endpoint returns incompatible value</span></span>

#### <a name="azaks"></a><span data-ttu-id="c0450-165">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="c0450-165">Az.Aks</span></span>
* <span data-ttu-id="c0450-166">"ClientIdAndSecret" removido para "ServicePrincipalIdAndSecret" e "ClientIdAndSecret" definido como um alias [#12381].</span><span class="sxs-lookup"><span data-stu-id="c0450-166">Removed 'ClientIdAndSecret' to 'ServicePrincipalIdAndSecret' and set 'ClientIdAndSecret' as an alias [#12381].</span></span>
* <span data-ttu-id="c0450-167">"Get-AzAks"/"New-AzAks"/"Remove-AzAks"/"Set-AzAks" removidos para "Get-AzAksCluster"/"New-AzAksCluster"/"Remove-AzAksCluster"/"Set-AzAksCluster" e definição dos valores originais como alias [#12373].</span><span class="sxs-lookup"><span data-stu-id="c0450-167">Removed 'Get-AzAks'/'New-AzAks'/'Remove-AzAks'/'Set-AzAks' to 'Get-AzAksCluster'/'New-AzAksCluster'/'Remove-AzAksCluster'/'Set-AzAksCluster' and set the original ones as alias [#12373].</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c0450-168">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c0450-168">Az.ApiManagement</span></span>
* <span data-ttu-id="c0450-169">Novo cmdlet "Add-AzApiManagementApiToGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="c0450-169">Added new 'Add-AzApiManagementApiToGateway' cmdlet.</span></span>
* <span data-ttu-id="c0450-170">Novo cmdlet "Get-AzApiManagementGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="c0450-170">Added new 'Get-AzApiManagementGateway' cmdlet.</span></span>
* <span data-ttu-id="c0450-171">Novo cmdlet "Get-AzApiManagementGatewayHostnameConfiguration" adicionado.</span><span class="sxs-lookup"><span data-stu-id="c0450-171">Added new 'Get-AzApiManagementGatewayHostnameConfiguration' cmdlet.</span></span>
* <span data-ttu-id="c0450-172">Novo cmdlet "Get-AzApiManagementGatewayKey" adicionado.</span><span class="sxs-lookup"><span data-stu-id="c0450-172">Added new 'Get-AzApiManagementGatewayKey' cmdlet.</span></span>
* <span data-ttu-id="c0450-173">Novo cmdlet "New-AzApiManagementGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="c0450-173">Added new 'New-AzApiManagementGateway' cmdlet.</span></span>
* <span data-ttu-id="c0450-174">Novo cmdlet "New-AzApiManagementGatewayHostnameConfiguration" adicionado.</span><span class="sxs-lookup"><span data-stu-id="c0450-174">Added new 'New-AzApiManagementGatewayHostnameConfiguration' cmdlet.</span></span>
* <span data-ttu-id="c0450-175">Novo cmdlet "New-AzApiManagementResourceLocationObject" adicionado.</span><span class="sxs-lookup"><span data-stu-id="c0450-175">Added new 'New-AzApiManagementResourceLocationObject' cmdlet.</span></span>
* <span data-ttu-id="c0450-176">Novo cmdlet "Remove-AzApiManagementApiFromGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="c0450-176">Added new 'Remove-AzApiManagementApiFromGateway' cmdlet.</span></span>
* <span data-ttu-id="c0450-177">Novo cmdlet "Remove-AzApiManagementGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="c0450-177">Added new 'Remove-AzApiManagementGateway' cmdlet.</span></span>
* <span data-ttu-id="c0450-178">Novo cmdlet "Remove-AzApiManagementGatewayHostnameConfiguration" adicionado.</span><span class="sxs-lookup"><span data-stu-id="c0450-178">Added new 'Remove-AzApiManagementGatewayHostnameConfiguration' cmdlet.</span></span>
* <span data-ttu-id="c0450-179">Novo cmdlet "Update-AzApiManagementGateway" adicionado.</span><span class="sxs-lookup"><span data-stu-id="c0450-179">Added new 'Update-AzApiManagementGateway' cmdlet.</span></span>
* <span data-ttu-id="c0450-180">Foi adicionado um novo parâmetro [-GatewayId] opcional ao cmdlet "Get-AzApiManagementApi".</span><span class="sxs-lookup"><span data-stu-id="c0450-180">Added new optional [-GatewayId] parameter to the 'Get-AzApiManagementApi' cmdlet.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c0450-181">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c0450-181">Az.CognitiveServices</span></span>
* <span data-ttu-id="c0450-182">Utilizado "Deny" especificamente como ação NetworkRules predefinida.</span><span class="sxs-lookup"><span data-stu-id="c0450-182">Used 'Deny' specifically as NetworkRules default action.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c0450-183">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c0450-183">Az.FrontDoor</span></span>
* <span data-ttu-id="c0450-184">Foi resolvido um problema em que é gerada uma exceção quando Enum.Parse tenta limitar um valor nulo a um valor de enumeração Enabled ou Disabled [#12344]</span><span class="sxs-lookup"><span data-stu-id="c0450-184">Fixed an issue where an exception is being thrown when Enum.Parse tries to coerce a null value to an Enabled or Disabled enum values [#12344]</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c0450-185">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c0450-185">Az.HDInsight</span></span>
* <span data-ttu-id="c0450-186">É suportada a criação de clusters com encriptação na funcionalidade de trânsito.</span><span class="sxs-lookup"><span data-stu-id="c0450-186">Supported creating cluster with encryption in transit feature.</span></span>
    - <span data-ttu-id="c0450-187">Foi adicionado o novo parâmetro "EncryptionInTransit" ao cmdlet "New-AzHDInsightCluster"</span><span class="sxs-lookup"><span data-stu-id="c0450-187">Add new parameter 'EncryptionInTransit' to the cmdlet 'New-AzHDInsightCluster'</span></span>
    - <span data-ttu-id="c0450-188">Foi adicionado o novo parâmetro "EncryptionInTransit" ao cmdlet "New-AzHDInsightClusterConfig"</span><span class="sxs-lookup"><span data-stu-id="c0450-188">Add new parameter 'EncryptionInTransit' to the cmdlet 'New-AzHDInsightClusterConfig'</span></span>
* <span data-ttu-id="c0450-189">É suportada a criação de clusters com a funcionalidade de ligação privada:</span><span class="sxs-lookup"><span data-stu-id="c0450-189">Supported creating cluster with private link feature:</span></span>
    - <span data-ttu-id="c0450-190">Novos parâmetros "PublicNetworkAccessType" e "OutboundPublicNetworkAccessType" adicionados ao cmdlet "New-AzHDInsightCluster"</span><span class="sxs-lookup"><span data-stu-id="c0450-190">Add new parameter 'PublicNetworkAccessType' and 'OutboundPublicNetworkAccessType' to the cmdlet 'New-AzHDInsightCluster'</span></span>
    - <span data-ttu-id="c0450-191">Novos parâmetros "PublicNetworkAccessType" e "OutboundPublicNetworkAccessType" adicionados ao cmdlet "New-AzHDInsightClusterConfig"</span><span class="sxs-lookup"><span data-stu-id="c0450-191">Add new parameter 'PublicNetworkAccessType' and 'OutboundPublicNetworkAccessType' to the cmdlet 'New-AzHDInsightClusterConfig'</span></span>
* <span data-ttu-id="c0450-192">Informações de rede virtual devolvidas ao chamar "New-AzHDInsightCluster" ou "Get-AzHDInsightCluster"</span><span class="sxs-lookup"><span data-stu-id="c0450-192">Returned virtual network information when calling 'New-AzHDInsightCluster' or 'Get-AzHDInsightCluster'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-193">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-193">Az.Network</span></span>
* <span data-ttu-id="c0450-194">Adição de suporte para o parâmetro AddressPrefixType a "Remove-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="c0450-194">Added support for AddressPrefixType parameter to 'Remove-AzExpressRouteCircuitConnectionConfig'</span></span>
* <span data-ttu-id="c0450-195">Alterações não interruptivas adicionadas: Funcionalidade PeerAddressType para Peering Privado em "Remove-AzExpressRouteCircutPeeringConfig".</span><span class="sxs-lookup"><span data-stu-id="c0450-195">Added non-breaking changes: PeerAddressType functionality for Private Peering in 'Remove-AzExpressRouteCircutPeeringConfig'.</span></span>
* <span data-ttu-id="c0450-196">Código alterado para ignorar caso dos parâmetros AddressPrefixType e PeerAddressType.</span><span class="sxs-lookup"><span data-stu-id="c0450-196">Code changed to ignore case for AddressPrefixType and PeerAddressType parameter.</span></span>
* <span data-ttu-id="c0450-197">Foi modificada a mensagem de aviso de "New-AzLoadBalancerFrontendIpConfig", "New-AzPublicIpAddress" e "New-AzPublicIpPrefix".</span><span class="sxs-lookup"><span data-stu-id="c0450-197">Modified the warning message for 'New-AzLoadBalancerFrontendIpConfig', 'New-AzPublicIpAddress' and 'New-AzPublicIpPrefix'.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c0450-198">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-198">Az.OperationalInsights</span></span>
* <span data-ttu-id="c0450-199">Opção "-ForceDelete" adicionada para "Remove-AzOperationalInsightsworkspace"</span><span class="sxs-lookup"><span data-stu-id="c0450-199">Added '-ForceDelete' option for 'Remove-AzOperationalInsightsworkspace'</span></span>
* <span data-ttu-id="c0450-200">Novo cmdlet "Get-AzOperationalInsightsDeletedWorkspace" adicionado</span><span class="sxs-lookup"><span data-stu-id="c0450-200">Added new cmdlet 'Get-AzOperationalInsightsDeletedWorkspace'</span></span>
* <span data-ttu-id="c0450-201">Novo cmdlet "Restore-AzOperationalInsightsWorkspace" adicionado</span><span class="sxs-lookup"><span data-stu-id="c0450-201">Added new cmdlet 'Restore-AzOperationalInsightsWorkspace'</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-202">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-202">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-203">Experiência de deteção de contentores/itens do Azure Backup melhorada.</span><span class="sxs-lookup"><span data-stu-id="c0450-203">Improved the Azure Backup container/item discovery experience.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-204">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-204">Az.Resources</span></span>
* <span data-ttu-id="c0450-205">Propriedades "Condition", "ConditionVersion" e "Description" adicionadas a "New-AzRoleAssignment"</span><span class="sxs-lookup"><span data-stu-id="c0450-205">Added properties 'Condition', 'ConditionVersion' and 'Description' to 'New-AzRoleAssignment'</span></span>
    - <span data-ttu-id="c0450-206">Isto incluiu todas as alterações relevantes aos modelos de dados</span><span class="sxs-lookup"><span data-stu-id="c0450-206">This included all the relevant changes to the data models</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-207">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-207">Az.Sql</span></span>
* <span data-ttu-id="c0450-208">Foi corrigido o potencial erro de nome do servidor não sensível a maiúsculas e minúsculas em "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="c0450-208">Fixed potential server name case insensitive error in 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="c0450-209">Foi corrigido o erro em que era devolvido um nome de base de dados incorreto numa base de dados existente em "New-AzSqlDatabaseSecondary"</span><span class="sxs-lookup"><span data-stu-id="c0450-209">Fixed wrong database name returned on existing database error in 'New-AzSqlDatabaseSecondary'</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-210">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-210">Az.Storage</span></span>
* <span data-ttu-id="c0450-211">Criação de tokens de SAS de contentores/blobs suportada com nova permissão x,t</span><span class="sxs-lookup"><span data-stu-id="c0450-211">Supported create container/blob Sas token with new permission x,t</span></span>
    -  <span data-ttu-id="c0450-212">"New-AzStorageBlobSASToken"</span><span class="sxs-lookup"><span data-stu-id="c0450-212">'New-AzStorageBlobSASToken'</span></span>
    -  <span data-ttu-id="c0450-213">"New-AzStorageContainerSASToken"</span><span class="sxs-lookup"><span data-stu-id="c0450-213">'New-AzStorageContainerSASToken'</span></span>
* <span data-ttu-id="c0450-214">Criação de tokens de SAS de contas suportada com nova permissão x,t,f</span><span class="sxs-lookup"><span data-stu-id="c0450-214">Supported create account Sas token with new permission x,t,f</span></span>
    -  <span data-ttu-id="c0450-215">"New-AzStorageAccountSASToken"</span><span class="sxs-lookup"><span data-stu-id="c0450-215">'New-AzStorageAccountSASToken'</span></span>
* <span data-ttu-id="c0450-216">Obtenção da utilização de partilha de ficheiros única suportada</span><span class="sxs-lookup"><span data-stu-id="c0450-216">Supported get single file share usage</span></span>
    - <span data-ttu-id="c0450-217">"Get-AzRmStorageShare"</span><span class="sxs-lookup"><span data-stu-id="c0450-217">'Get-AzRmStorageShare'</span></span>

## <a name="440---july-2020"></a><span data-ttu-id="c0450-218">4.4.0 - Julho de 2020</span><span class="sxs-lookup"><span data-stu-id="c0450-218">4.4.0 - July 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c0450-219">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-219">Az.Accounts</span></span>
* <span data-ttu-id="c0450-220">Adição do novo cmdlet "Invoke-AzRestMethod"</span><span class="sxs-lookup"><span data-stu-id="c0450-220">Added new cmdlet 'Invoke-AzRestMethod'</span></span>
* <span data-ttu-id="c0450-221">Correção de um problema que pode causar erros de autenticação em cenários de vários processos, tais como executar vários cmdlets do Azure PowerShell utilizando "Start-Job" [#9448]</span><span class="sxs-lookup"><span data-stu-id="c0450-221">Fixed an issue that may cause authentication errors in multi-process scenarios such as running multiple Azure PowerShell cmdlets using 'Start-Job' [#9448]</span></span>

#### <a name="azaks"></a><span data-ttu-id="c0450-222">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="c0450-222">Az.Aks</span></span>
* <span data-ttu-id="c0450-223">Correção do erro "Get-AzAks" uma vez que não recebe todos os clusters [#12296]</span><span class="sxs-lookup"><span data-stu-id="c0450-223">Fixed bug 'Get-AzAks' doesn't get all clusters [#12296]</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="c0450-224">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c0450-224">Az.AnalysisServices</span></span>
* <span data-ttu-id="c0450-225">Remoção da referência do projeto para Autenticação</span><span class="sxs-lookup"><span data-stu-id="c0450-225">Removed project reference to Authentication</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c0450-226">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c0450-226">Az.Automation</span></span>
* <span data-ttu-id="c0450-227">Correção do problema em que a cadeia com chars de fuga não pode ser convertida num objeto json.</span><span class="sxs-lookup"><span data-stu-id="c0450-227">Fixed the issue that string with escape chars cannot be converted into json object.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-228">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-228">Az.Compute</span></span>
* <span data-ttu-id="c0450-229">Adição do aviso ao utilizar "New-AzVmss" sem a versão de imagem "mais recente"</span><span class="sxs-lookup"><span data-stu-id="c0450-229">Added warning when using 'New-AzVmss' without 'latest' image version</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c0450-230">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c0450-230">Az.DataFactory</span></span>
* <span data-ttu-id="c0450-231">Adição de parâmetros globais ao Data Factory.</span><span class="sxs-lookup"><span data-stu-id="c0450-231">Added global parameters to Data Factory.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="c0450-232">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c0450-232">Az.EventGrid</span></span>
* <span data-ttu-id="c0450-233">Atualização para utilizar a versão de API 2020-06-01.</span><span class="sxs-lookup"><span data-stu-id="c0450-233">Updated to use the 2020-06-01 API version.</span></span>
* <span data-ttu-id="c0450-234">Novas funcionalidades adicionadas:</span><span class="sxs-lookup"><span data-stu-id="c0450-234">Added new features:</span></span>
    - <span data-ttu-id="c0450-235">Mapeamento de entrada</span><span class="sxs-lookup"><span data-stu-id="c0450-235">Input mapping</span></span>
    - <span data-ttu-id="c0450-236">Esquema de Entrega de Eventos</span><span class="sxs-lookup"><span data-stu-id="c0450-236">Event Delivery Schema</span></span>
    - <span data-ttu-id="c0450-237">Ligação Privada</span><span class="sxs-lookup"><span data-stu-id="c0450-237">Private Link</span></span>
    - <span data-ttu-id="c0450-238">Esquema de Eventos na Cloud V10</span><span class="sxs-lookup"><span data-stu-id="c0450-238">Cloud Event V10 Schema</span></span>
    - <span data-ttu-id="c0450-239">Tópico do Service Bus como Destino</span><span class="sxs-lookup"><span data-stu-id="c0450-239">Service Bus Topic As Destination</span></span>
    - <span data-ttu-id="c0450-240">Função do Azure como Destino</span><span class="sxs-lookup"><span data-stu-id="c0450-240">Azure Function As Destination</span></span>
    - <span data-ttu-id="c0450-241">Criação de batches do WebHook</span><span class="sxs-lookup"><span data-stu-id="c0450-241">WebHook Batching</span></span>
    - <span data-ttu-id="c0450-242">Webhook seguro (suporte de AAD)</span><span class="sxs-lookup"><span data-stu-id="c0450-242">Secure webhook (AAD support)</span></span>
    - <span data-ttu-id="c0450-243">IpFiltering</span><span class="sxs-lookup"><span data-stu-id="c0450-243">IpFiltering</span></span>
* <span data-ttu-id="c0450-244">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="c0450-244">Updated cmdlets:</span></span>
    - <span data-ttu-id="c0450-245">"New-AzEventGridSubscription"/"Update-AzEventGridSubscription":</span><span class="sxs-lookup"><span data-stu-id="c0450-245">'New-AzEventGridSubscription'/'Update-AzEventGridSubscription':</span></span>
        - <span data-ttu-id="c0450-246">Adicionar novos parâmetros opcionais para suportar a criação de batches do webhook.</span><span class="sxs-lookup"><span data-stu-id="c0450-246">Add new optional parameters to support webhook batching.</span></span>
        - <span data-ttu-id="c0450-247">Adicionar novos parâmetros opcionais para suportar o webhook seguro através do AAD.</span><span class="sxs-lookup"><span data-stu-id="c0450-247">Add new optional parameters to support secured webhook using AAD.</span></span>
        - <span data-ttu-id="c0450-248">Adicionar uma nova enumeração para o parâmetro EndpointType para suportar a função do Azure e o tópico do Service Bus enquanto novos destinos.</span><span class="sxs-lookup"><span data-stu-id="c0450-248">Add new enum for EndpointType parameter to support azure function and service bus topic as new destinations.</span></span>
        - <span data-ttu-id="c0450-249">Adicionar novo parâmetro opcional para o esquema de entrega.</span><span class="sxs-lookup"><span data-stu-id="c0450-249">Add new optional parameter for delivery schema.</span></span>
    - <span data-ttu-id="c0450-250">"New-AzEventGridTopic"/"Update-AzEventGridTopic" e "New-AzEventGridDomain"/"Update-AzEventGridDomain":</span><span class="sxs-lookup"><span data-stu-id="c0450-250">'New-AzEventGridTopic'/'Update-AzEventGridTopic' and 'New-AzEventGridDomain'/'Update-AzEventGridDomain':</span></span>
        - <span data-ttu-id="c0450-251">Adicionar novos parâmetros opcionais para suportar IpFiltering.</span><span class="sxs-lookup"><span data-stu-id="c0450-251">Add new optional parameters to support IpFiltering.</span></span>
    - <span data-ttu-id="c0450-252">"New-AzEventGridTopic"/"New-AzEventGridDomain":</span><span class="sxs-lookup"><span data-stu-id="c0450-252">'New-AzEventGridTopic'/'New-AzEventGridDomain':</span></span>
        - <span data-ttu-id="c0450-253">Adicionar novos parâmetros opcionais para suportar o Mapeamento de entrada.</span><span class="sxs-lookup"><span data-stu-id="c0450-253">Add new optional parameters to support Input mapping.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c0450-254">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c0450-254">Az.FrontDoor</span></span>
* <span data-ttu-id="c0450-255">Módulo atualizado para utilizar a API 2020-05-01</span><span class="sxs-lookup"><span data-stu-id="c0450-255">Updated module to use API 2020-05-01</span></span>
* <span data-ttu-id="c0450-256">Adição de suporte do Private Link para recursos de Armazenamento, Cofre de chaves e Serviço de Aplicações Web</span><span class="sxs-lookup"><span data-stu-id="c0450-256">Added Private link support for Storage, Keyvault and Web App Service resources</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c0450-257">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c0450-257">Az.HDInsight</span></span>
* <span data-ttu-id="c0450-258">Suporte para a criação de cluster com armazenamento ADLSGen1/2 em clouds nacionais.</span><span class="sxs-lookup"><span data-stu-id="c0450-258">Supported creating cluster with ADLSGen1/2 storage in national clouds.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c0450-259">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c0450-259">Az.Monitor</span></span>
* <span data-ttu-id="c0450-260">Correção do erro em "Get-AzDiagnosticSetting" quando as métricas ou registos são nulos [#12272]</span><span class="sxs-lookup"><span data-stu-id="c0450-260">Fixed bug for 'Get-AzDiagnosticSetting' when metrics or logs are null [#12272]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-261">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-261">Az.Network</span></span>
* <span data-ttu-id="c0450-262">Correção da troca de parâmetros na ligação VWan HubVnet</span><span class="sxs-lookup"><span data-stu-id="c0450-262">Fixed parameters swap in VWan HubVnet connection</span></span>
* <span data-ttu-id="c0450-263">Adição de novos cmdlets para Sites de Aplicações Virtuais da Rede Azure</span><span class="sxs-lookup"><span data-stu-id="c0450-263">Added new cmdlets for Azure Network Virtual Appliance Sites</span></span>
    - <span data-ttu-id="c0450-264">"Get-AzVirtualApplianceSite"</span><span class="sxs-lookup"><span data-stu-id="c0450-264">'Get-AzVirtualApplianceSite'</span></span>
    - <span data-ttu-id="c0450-265">"New-AzVirtualApplianceSite"</span><span class="sxs-lookup"><span data-stu-id="c0450-265">'New-AzVirtualApplianceSite'</span></span>
    - <span data-ttu-id="c0450-266">"Remove-AzVirtualApplianceSite"</span><span class="sxs-lookup"><span data-stu-id="c0450-266">'Remove-AzVirtualApplianceSite'</span></span>
    - <span data-ttu-id="c0450-267">"Update-AzVirtualApplianceSite"</span><span class="sxs-lookup"><span data-stu-id="c0450-267">'Update-AzVirtualApplianceSite'</span></span>
    - <span data-ttu-id="c0450-268">"New-AzOffice365PolicyProperty"</span><span class="sxs-lookup"><span data-stu-id="c0450-268">'New-AzOffice365PolicyProperty'</span></span>
* <span data-ttu-id="c0450-269">Adição de novos cmdlets para Aplicações Virtuais da Rede Azure</span><span class="sxs-lookup"><span data-stu-id="c0450-269">Added new cmdlets for Azure Network Virtual Appliance</span></span>
    - <span data-ttu-id="c0450-270">"Get-AzNetworkVirtualAppliance"</span><span class="sxs-lookup"><span data-stu-id="c0450-270">'Get-AzNetworkVirtualAppliance'</span></span>
    - <span data-ttu-id="c0450-271">"New-AzNetworkVirtualAppliance"</span><span class="sxs-lookup"><span data-stu-id="c0450-271">'New-AzNetworkVirtualAppliance'</span></span>
    - <span data-ttu-id="c0450-272">"Remove-AzNetworkVirtualAppliance"</span><span class="sxs-lookup"><span data-stu-id="c0450-272">'Remove-AzNetworkVirtualAppliance'</span></span>
    - <span data-ttu-id="c0450-273">"Update-AzNetworkVirtualAppliance"</span><span class="sxs-lookup"><span data-stu-id="c0450-273">'Update-AzNetworkVirtualAppliance'</span></span>
    - <span data-ttu-id="c0450-274">"Get-AzNetworkVirtualApplianceSku"</span><span class="sxs-lookup"><span data-stu-id="c0450-274">'Get-AzNetworkVirtualApplianceSku'</span></span>
    - <span data-ttu-id="c0450-275">"New-AzVirtualApplianceSkuProperty"</span><span class="sxs-lookup"><span data-stu-id="c0450-275">'New-AzVirtualApplianceSkuProperty'</span></span>
* <span data-ttu-id="c0450-276">Gateway de Aplicação integrado para Cmdlets Comuns do Private Link</span><span class="sxs-lookup"><span data-stu-id="c0450-276">Onboarded Application Gateway to Private Link Common Cmdlets</span></span>
* <span data-ttu-id="c0450-277">StorageSync integrado para Cmdlets Comuns do Private Link</span><span class="sxs-lookup"><span data-stu-id="c0450-277">Onboarded StorageSync to Private Link Common Cmdlets</span></span>
* <span data-ttu-id="c0450-278">SignalR integrado para Cmdlets Comuns do Private Link</span><span class="sxs-lookup"><span data-stu-id="c0450-278">Onboarded SignalR to Private Link Common Cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-279">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-279">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-280">Remoção da referência do projeto para Autenticação</span><span class="sxs-lookup"><span data-stu-id="c0450-280">Removed project reference to Authentication</span></span>
* <span data-ttu-id="c0450-281">Os cmdlets afinados do Azure Backup ajudam o texto a ser mais preciso.</span><span class="sxs-lookup"><span data-stu-id="c0450-281">Azure Backup tuned cmdlets help text to be more accurate.</span></span>
* <span data-ttu-id="c0450-282">O Azure Backup adicionou suporte para obter tarefas de agentes MAB através do cmdlet "Get-AzRecoveryServicesBackupJob".</span><span class="sxs-lookup"><span data-stu-id="c0450-282">Azure Backup added support for fetching MAB agent jobs using 'Get-AzRecoveryServicesBackupJob' cmdlet.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-283">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-283">Az.Resources</span></span>
* <span data-ttu-id="c0450-284">Atualização de "Save-AzResourceGroupDeploymentTemplate" para utilizar o SDK.</span><span class="sxs-lookup"><span data-stu-id="c0450-284">Updated 'Save-AzResourceGroupDeploymentTemplate' to use the SDK.</span></span>
* <span data-ttu-id="c0450-285">Adição do cmdlet "Unregister-AzResourceProvider".</span><span class="sxs-lookup"><span data-stu-id="c0450-285">Added 'Unregister-AzResourceProvider' cmdlet.</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-286">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-286">Az.Sql</span></span>
* <span data-ttu-id="c0450-287">Adição de suporte para o Principal de serviço e utilizadores convidados no cmdlet Set-AzSqlInstanceActiveDirectoryAdministrator</span><span class="sxs-lookup"><span data-stu-id="c0450-287">Added support for Service principal and guest users in Set-AzSqlInstanceActiveDirectoryAdministrator cmdlet'</span></span>
* <span data-ttu-id="c0450-288">Correção de um erro em cmdlets de Classificação de Dados.</span><span class="sxs-lookup"><span data-stu-id="c0450-288">Fixed a bug in Data Classification cmdlets.'</span></span>
* <span data-ttu-id="c0450-289">Adição de suporte para a ativação pós-falha do Azure SQL Managed Instance: "Invoke-AzSqlInstanceFailover"</span><span class="sxs-lookup"><span data-stu-id="c0450-289">Added support for Azure SQL Managed Instance failover: 'Invoke-AzSqlInstanceFailover'</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-290">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-290">Az.Storage</span></span>
* <span data-ttu-id="c0450-291">Correção do erro de que o UserAgent não é adicionado para alguns cmdlets do plano de dados.</span><span class="sxs-lookup"><span data-stu-id="c0450-291">Fixed the issue that UserAgent is not added for some data plane cmdlets.</span></span>
* <span data-ttu-id="c0450-292">Suporte para a criação/atualização da Conta de armazenamento com MinimumTlsVersion e AllowBlobPublicAccess</span><span class="sxs-lookup"><span data-stu-id="c0450-292">Supported create/update Storage account with MinimumTlsVersion and AllowBlobPublicAccess</span></span>
    -  <span data-ttu-id="c0450-293">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c0450-293">'New-AzStorageAccount'</span></span>
    -  <span data-ttu-id="c0450-294">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c0450-294">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="c0450-295">Suporte para Permitir/desativar o controlo de versões no Serviço Blob de uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="c0450-295">Support enable/disable versioning on Blob Service of a Storage account</span></span>
    - <span data-ttu-id="c0450-296">"Update-AzStorageBlobServiceProperty"</span><span class="sxs-lookup"><span data-stu-id="c0450-296">'Update-AzStorageBlobServiceProperty'</span></span>
* <span data-ttu-id="c0450-297">Suporte para a lista de blobs com versões de blobs</span><span class="sxs-lookup"><span data-stu-id="c0450-297">Support list blobs with blob versions</span></span>
    - <span data-ttu-id="c0450-298">"Get-AzStorageBlob"</span><span class="sxs-lookup"><span data-stu-id="c0450-298">'Get-AzStorageBlob'</span></span>
* <span data-ttu-id="c0450-299">Suporte para obter/remover instantâneo de blob único ou versão do blob</span><span class="sxs-lookup"><span data-stu-id="c0450-299">Support get/remove single blob snapshot or blob version</span></span>
    - <span data-ttu-id="c0450-300">"Get-AzStorageBlob"</span><span class="sxs-lookup"><span data-stu-id="c0450-300">'Get-AzStorageBlob'</span></span>
    - <span data-ttu-id="c0450-301">"Remove-AzStorageBlob"</span><span class="sxs-lookup"><span data-stu-id="c0450-301">'Remove-AzStorageBlob'</span></span>
* <span data-ttu-id="c0450-302">Suporte para pipeline a partir do objeto de blob gerado a partir de Azure.Storage.Blobs V12</span><span class="sxs-lookup"><span data-stu-id="c0450-302">Support pipeline from blob object generated from Azure.Storage.Blobs V12</span></span>
    - <span data-ttu-id="c0450-303">"Get-AzStorageBlobContent"</span><span class="sxs-lookup"><span data-stu-id="c0450-303">'Get-AzStorageBlobContent'</span></span>
    - <span data-ttu-id="c0450-304">"New-AzStorageBlobSASToken"</span><span class="sxs-lookup"><span data-stu-id="c0450-304">'New-AzStorageBlobSASToken'</span></span>
    - <span data-ttu-id="c0450-305">"Remove-AzStorageBlob"</span><span class="sxs-lookup"><span data-stu-id="c0450-305">'Remove-AzStorageBlob'</span></span>
    - <span data-ttu-id="c0450-306">"Set-AzStorageBlobContent"</span><span class="sxs-lookup"><span data-stu-id="c0450-306">'Set-AzStorageBlobContent'</span></span>
    - <span data-ttu-id="c0450-307">"Start-AzStorageBlobCopy"</span><span class="sxs-lookup"><span data-stu-id="c0450-307">'Start-AzStorageBlobCopy'</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="c0450-308">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="c0450-308">Az.StorageSync</span></span>
* <span data-ttu-id="c0450-309">Adição de uma nova versão StorageSync SDK para ApiVersion 2020-03-01</span><span class="sxs-lookup"><span data-stu-id="c0450-309">Added a new version StorageSync SDK targeting ApiVersion 2020-03-01</span></span>
* <span data-ttu-id="c0450-310">Adição de cmdlet do Serviço de Sincronização de Armazenamento de Atualização</span><span class="sxs-lookup"><span data-stu-id="c0450-310">Added Update Storage Sync Service cmdlet</span></span>
    - <span data-ttu-id="c0450-311">"Set-AzStorageSyncService"</span><span class="sxs-lookup"><span data-stu-id="c0450-311">'Set-AzStorageSyncService'</span></span>
* <span data-ttu-id="c0450-312">Adição de IncomingTrafficPolicy e PrivateEndpointConnections para cmdlets StorageSyncService.</span><span class="sxs-lookup"><span data-stu-id="c0450-312">Added IncomingTrafficPolicy and PrivateEndpointConnections to StorageSyncService cmdlets.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c0450-313">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-313">Az.Websites</span></span>
* <span data-ttu-id="c0450-314">Adição de suporte para a realização de operações para Slots em grupos de recursos diferentes do Plano do Serviço de Aplicações</span><span class="sxs-lookup"><span data-stu-id="c0450-314">Added support to perform operations for Slots not in the same resource group as the App Service Plan</span></span>

## <a name="430---june-2020"></a><span data-ttu-id="c0450-315">4.3.0 - Junho de 2020</span><span class="sxs-lookup"><span data-stu-id="c0450-315">4.3.0 - June 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c0450-316">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-316">Az.Accounts</span></span>
* <span data-ttu-id="c0450-317">Suporte para a deteção da definição do ambiente por predefinição e adição de ambiente através de "Add-AzEnvironment"</span><span class="sxs-lookup"><span data-stu-id="c0450-317">Supported discovering environment setting by default and adding environment via 'Add-AzEnvironment'</span></span>
* <span data-ttu-id="c0450-318">Atualizar assemblagens pré-carregadas [#12024], [#11976]</span><span class="sxs-lookup"><span data-stu-id="c0450-318">Update preloaded assemblies [#12024], [#11976]</span></span>
* <span data-ttu-id="c0450-319">Atualização da assemblagem Azure.Core</span><span class="sxs-lookup"><span data-stu-id="c0450-319">Updated Azure.Core assembly</span></span>
* <span data-ttu-id="c0450-320">Correção de um problema que pode provocar a falha de "Connect-AzAccount" numa execução de múltiplos threads [#11201]</span><span class="sxs-lookup"><span data-stu-id="c0450-320">Fixed an issue that may cause 'Connect-AzAccount' to fail in multi-threaded execution [#11201]</span></span>

#### <a name="azaks"></a><span data-ttu-id="c0450-321">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="c0450-321">Az.Aks</span></span>
* <span data-ttu-id="c0450-322">Substituição da utilização da [API AccessProfile](https://docs.microsoft.com/rest/api/aks/managedclusters/getaccessprofile) antiga por chamadas para as APIs [ListClusterAdmin](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusteradmincredentials) e [ListClusterUser](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusterusercredentials)</span><span class="sxs-lookup"><span data-stu-id="c0450-322">Replaced usage of old [AccessProfile API](https://docs.microsoft.com/rest/api/aks/managedclusters/getaccessprofile) with calls to [ListClusterAdmin](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusteradmincredentials) and [ListClusterUser](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusterusercredentials) APIs</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c0450-323">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c0450-323">Az.Batch</span></span>
* <span data-ttu-id="c0450-324">Atualização da versão do SDK de Az.Batch para utilizar "Microsoft.Azure.Management.Batch" para 11.0.0</span><span class="sxs-lookup"><span data-stu-id="c0450-324">Updated Az.Batch to use 'Microsoft.Azure.Management.Batch' SDK version to 11.0.0</span></span>
* <span data-ttu-id="c0450-325">Adição da capacidade de definir a Identidade BatchAccount no cmdlet "New-AzBatchAccount"</span><span class="sxs-lookup"><span data-stu-id="c0450-325">Added the ability to set the BatchAccount Identity in the 'New-AzBatchAccount' cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c0450-326">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c0450-326">Az.CognitiveServices</span></span>
* <span data-ttu-id="c0450-327">Suporte para a apresentação das capacidades da conta.</span><span class="sxs-lookup"><span data-stu-id="c0450-327">Supported displaying account capabilities.</span></span>
* <span data-ttu-id="c0450-328">Suporte para a modificação de PublicNetworkAccess.</span><span class="sxs-lookup"><span data-stu-id="c0450-328">Supported modifying PublicNetworkAccess.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-329">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-329">Az.Compute</span></span>
* <span data-ttu-id="c0450-330">Adição do parâmetro SimulateEviction aos cmdlets Set-AzVM e Set-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="c0450-330">Added SimulateEviction parameter to Set-AzVM and Set-AzVmssVM cmdlets.</span></span>
* <span data-ttu-id="c0450-331">Adição de "Premium_LRS" ao mecanismo de preenchimento de argumentos do parâmetro StorageAccountType para o cmdlet New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="c0450-331">Added 'Premium_LRS' to the argument completer of StorageAccountType parameter for New-AzGalleryImageVersion cmdlet.</span></span>
* <span data-ttu-id="c0450-332">Adição de subestados a VMCustomScriptExtension [#11297]</span><span class="sxs-lookup"><span data-stu-id="c0450-332">Added Substatuses to VMCustomScriptExtension [#11297]</span></span>
* <span data-ttu-id="c0450-333">Adição de "Delete" ao mecanismo de preenchimento de argumentos do parâmetro EvictionPolicy para os cmdlets New-AzVM e New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="c0450-333">Added 'Delete' to the argument completer of EvictionPolicy parameter for New-AzVM and New-AzVMConfig cmdlets.</span></span>
* <span data-ttu-id="c0450-334">Correção do nome da nova Extensão de VM para SAP</span><span class="sxs-lookup"><span data-stu-id="c0450-334">Fixed name of new VM Extension for SAP</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c0450-335">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c0450-335">Az.DataFactory</span></span>
* <span data-ttu-id="c0450-336">Atualização da versão do SDK de .Net do ADF para 4.9.0</span><span class="sxs-lookup"><span data-stu-id="c0450-336">Updated ADF .Net SDK version to 4.9.0</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c0450-337">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c0450-337">Az.EventHub</span></span>
* <span data-ttu-id="c0450-338">Adição de parâmetros de Identidade Gerida aos cmdlets "New-AzEventHubNamespace" e "Set-AzEventHubNamespace"</span><span class="sxs-lookup"><span data-stu-id="c0450-338">Added Managed Identity parameters to 'New-AzEventHubNamespace' and 'Set-AzEventHubNamespace' cmdlets</span></span>

#### <a name="azfunctions"></a><span data-ttu-id="c0450-339">Az.Functions</span><span class="sxs-lookup"><span data-stu-id="c0450-339">Az.Functions</span></span>
* <span data-ttu-id="c0450-340">Adição de suporte para a criação de aplicações de funções do PowerShell 7.0 e de Java 11</span><span class="sxs-lookup"><span data-stu-id="c0450-340">Added support to create PowerShell 7.0 and Java 11 function apps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c0450-341">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c0450-341">Az.HDInsight</span></span>
* <span data-ttu-id="c0450-342">Suporte para listagem de anfitriões e reinício de anfitriões específicos do cluster HDInsight.</span><span class="sxs-lookup"><span data-stu-id="c0450-342">Supported listing hosts and restart specific hosts of the HDInsight cluster.</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="c0450-343">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="c0450-343">Az.HealthcareApis</span></span>
* <span data-ttu-id="c0450-344">Atualização da versão do SDK para 1.1.0</span><span class="sxs-lookup"><span data-stu-id="c0450-344">Updated the SDK version to 1.1.0</span></span>
* <span data-ttu-id="c0450-345">Adição de suporte para as definições de Exportação e a Identidade Gerida</span><span class="sxs-lookup"><span data-stu-id="c0450-345">Added support for Export settings and Managed Identity</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c0450-346">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c0450-346">Az.Monitor</span></span>
* <span data-ttu-id="c0450-347">Correção do parâmetro de objeto de entrada para "Set-AzActivityLogAlert"</span><span class="sxs-lookup"><span data-stu-id="c0450-347">Fixed input object parameter for 'Set-AzActivityLogAlert'</span></span>
* <span data-ttu-id="c0450-348">Correção do parâmetro "InputObject" para "Set-AzActionGroup" [#10868]</span><span class="sxs-lookup"><span data-stu-id="c0450-348">Fixed 'InputObject' parameter for 'Set-AzActionGroup' [#10868]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-349">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-349">Az.Network</span></span>
* <span data-ttu-id="c0450-350">Adição de suporte para o parâmetro AddressPrefixType a "Remove-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="c0450-350">Added support for AddressPrefixType parameter to 'Remove-AzExpressRouteCircuitConnectionConfig'</span></span>
* <span data-ttu-id="c0450-351">Adição de novos cmdlets para a Política de Firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="c0450-351">Added new cmdlets for Azure FirewallPolicy</span></span>
    - <span data-ttu-id="c0450-352">"New-AzFirewallPolicyDnsSetting"</span><span class="sxs-lookup"><span data-stu-id="c0450-352">'New-AzFirewallPolicyDnsSetting'</span></span>
    - <span data-ttu-id="c0450-353">Suporte para FQDN de Destino nas Regras de Rede para a Política de Firewall</span><span class="sxs-lookup"><span data-stu-id="c0450-353">Support for Destination FQDN in Network Rules for Firewall Policy</span></span>
* <span data-ttu-id="c0450-354">Adição de suporte para operações de conjuntos de endereços back-end</span><span class="sxs-lookup"><span data-stu-id="c0450-354">Added support for backend address pool operations</span></span>
    - <span data-ttu-id="c0450-355">"New-AzLoadBalancerBackendAddressConfig"</span><span class="sxs-lookup"><span data-stu-id="c0450-355">'New-AzLoadBalancerBackendAddressConfig'</span></span>
    - <span data-ttu-id="c0450-356">"New-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="c0450-356">'New-AzLoadBalancerBackendAddressPool'</span></span>
    - <span data-ttu-id="c0450-357">"Set-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="c0450-357">'Set-AzLoadBalancerBackendAddressPool'</span></span>
    - <span data-ttu-id="c0450-358">"Remove-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="c0450-358">'Remove-AzLoadBalancerBackendAddressPool'</span></span>
    - <span data-ttu-id="c0450-359">"Get-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="c0450-359">'Get-AzLoadBalancerBackendAddressPool'</span></span>
* <span data-ttu-id="c0450-360">Adição de validação de nomes para "New-AzIpGroup"</span><span class="sxs-lookup"><span data-stu-id="c0450-360">Added name validation for 'New-AzIpGroup'</span></span>
* <span data-ttu-id="c0450-361">Adição de novos cmdlets para a Política de Firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="c0450-361">Added new cmdlets for Azure FirewallPolicy</span></span>
    - <span data-ttu-id="c0450-362">"New-AzFirewallPolicyThreatIntelWhitelist"</span><span class="sxs-lookup"><span data-stu-id="c0450-362">'New-AzFirewallPolicyThreatIntelWhitelist'</span></span>
* <span data-ttu-id="c0450-363">Foram atualizados os seguintes comandos para a funcionalidade: Definição/remoção de servidores DNS personalizados no P2SVpnGateway de VirtualWan.</span><span class="sxs-lookup"><span data-stu-id="c0450-363">Updated below commands for feature: Custom dns servers set/remove on VirtualWan P2SVpnGateway.</span></span>
    - <span data-ttu-id="c0450-364">Atualização de New-AzP2sVpnGateway: Adição do parâmetro opcional "-CustomDnsServer" para os clientes especificarem os respetivos servidores DNS a definir no P2SVpnGateway, o qual pode ser utilizado por clientes do tipo Ponto a site.</span><span class="sxs-lookup"><span data-stu-id="c0450-364">Updated New-AzP2sVpnGateway: Added optional parameter '-CustomDnsServer' for customers to specify their dns servers to set on P2SVpnGateway, which can be used by Point to site clients.</span></span>
    - <span data-ttu-id="c0450-365">Atualização de Update-AzP2sVpnGateway: Adição do parâmetro opcional "-CustomDnsServer" para os clientes especificarem os respetivos servidores DNS a definir no P2SVpnGateway, o qual pode ser utilizado por clientes do tipo Ponto a site.</span><span class="sxs-lookup"><span data-stu-id="c0450-365">Updated Update-AzP2sVpnGateway: Added optional parameter '-CustomDnsServer' for customers to specify their dns servers to set on P2SVpnGateway, which can be used by Point to site clients.</span></span>
* <span data-ttu-id="c0450-366">Atualização de "Update-AzVpnGateway"</span><span class="sxs-lookup"><span data-stu-id="c0450-366">Updated 'Update-AzVpnGateway'</span></span>
    - <span data-ttu-id="c0450-367">Adição do parâmetro opcional "-BgpPeeringAddress" para os clientes especificarem os respetivos bgps personalizados a definir no VpnGateway.</span><span class="sxs-lookup"><span data-stu-id="c0450-367">Added optional parameter '-BgpPeeringAddress' for customers to specify their custom bgps to set on VpnGateway.</span></span>
* <span data-ttu-id="c0450-368">Adição de novo cmdlet para suportar a reposição do estado de encaminhamento de um recurso VirtualHub:</span><span class="sxs-lookup"><span data-stu-id="c0450-368">Added new cmdlet to support resetting the routing state of a VirtualHub resource:</span></span>
    - <span data-ttu-id="c0450-369">"Reset-AzHubRouter"</span><span class="sxs-lookup"><span data-stu-id="c0450-369">'Reset-AzHubRouter'</span></span>
* <span data-ttu-id="c0450-370">Atualização dos elementos indicados abaixo com base na alteração recente de Swagger para a Política de Firewall</span><span class="sxs-lookup"><span data-stu-id="c0450-370">Updated below things based on recent swagger change for Firewall Policy</span></span>
    - <span data-ttu-id="c0450-371">Alteração de nomes para RuleGroup, RuleCollectionGroup e RuleType</span><span class="sxs-lookup"><span data-stu-id="c0450-371">Changes names for RuleGroup, RuleCollectionGroup and RuleType</span></span>
    - <span data-ttu-id="c0450-372">Adição de suporte para Coleções de Regras de NAT da Política de Firewall para suportar várias Coleções de Regras de NAT</span><span class="sxs-lookup"><span data-stu-id="c0450-372">Added support for Firewall Policy NAT Rule Collections to support multiple NAT Rule Collection</span></span>
* <span data-ttu-id="c0450-373">[Alteração Interruptiva] Adição do parâmetro obrigatório "SourceIpGroup" para "New-AzFirewallPolicyApplicationRule" e "New-AzFirewallPolicyNetworkRule".</span><span class="sxs-lookup"><span data-stu-id="c0450-373">[Breaking Change] Added mandatory parameter 'SourceIpGroup' for 'New-AzFirewallPolicyApplicationRule' and 'New-AzFirewallPolicyNetworkRule'.</span></span>
* <span data-ttu-id="c0450-374">[Alteração Interruptiva] Correção do parâmetro "SourceAddress" de "New-AzFirewallPolicyApplicationRule" de modo a ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0450-374">[Breaking Change] Fixed 'New-AzFirewallPolicyApplicationRule', parameter 'SourceAddress' to be mandatory.</span></span>
* <span data-ttu-id="c0450-375">[Alteração Interruptiva] Correção do parâmetro "SourceAddress" de "New-AzFirewallPolicyApplicationRule" de modo a ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0450-375">[Breaking Change] Fixed 'New-AzFirewallPolicyApplicationRule', parameter 'SourceAddress' to be mandatory.</span></span>
* <span data-ttu-id="c0450-376">[Alteração Interruptiva] Remoção de parâmetros obrigatórios: "TranslatedAddress", "TranslatedPort" para "New-AzFirewallPolicyNatRuleCollection".</span><span class="sxs-lookup"><span data-stu-id="c0450-376">[Breaking Change] Removed mandatory parameters: 'TranslatedAddress', 'TranslatedPort' for 'New-AzFirewallPolicyNatRuleCollection'.</span></span>
* <span data-ttu-id="c0450-377">Adição de novos cmdlets para suportar PrivateLink no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="c0450-377">Added new cmdlets to support PrivateLink On Application Gateway</span></span>
    - <span data-ttu-id="c0450-378">"New-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c0450-378">'New-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="c0450-379">"Get-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c0450-379">'Get-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="c0450-380">"New-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c0450-380">'New-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="c0450-381">"Set-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c0450-381">'Set-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="c0450-382">"Remove-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c0450-382">'Remove-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="c0450-383">"New-AzApplicationGatewayPrivateLinkIpConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c0450-383">'New-AzApplicationGatewayPrivateLinkIpConfiguration'</span></span>
* <span data-ttu-id="c0450-384">Adição de novos cmdlets para o recurso subordinado HubRouteTables de VirtualHub.</span><span class="sxs-lookup"><span data-stu-id="c0450-384">Added new cmdlets for HubRouteTables child resource of VirtualHub.</span></span>
    - <span data-ttu-id="c0450-385">"New-AzVHubRoute"</span><span class="sxs-lookup"><span data-stu-id="c0450-385">'New-AzVHubRoute'</span></span>
    - <span data-ttu-id="c0450-386">"New-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="c0450-386">'New-AzVHubRouteTable'</span></span>
    - <span data-ttu-id="c0450-387">"Get-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="c0450-387">'Get-AzVHubRouteTable'</span></span>
    - <span data-ttu-id="c0450-388">"Update-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="c0450-388">'Update-AzVHubRouteTable'</span></span>
    - <span data-ttu-id="c0450-389">"Remove-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="c0450-389">'Remove-AzVHubRouteTable'</span></span>
* <span data-ttu-id="c0450-390">Atualização dos cmdlets existentes para suportar o parâmetro de entrada opcional RoutingConfiguration para encaminhamento personalizado em VirtualWan.</span><span class="sxs-lookup"><span data-stu-id="c0450-390">Updated existing cmdlets to support optional RoutingConfiguration input parameter for custom routing in VirtualWan.</span></span>
    - <span data-ttu-id="c0450-391">"New-AzExpressRouteConnection"</span><span class="sxs-lookup"><span data-stu-id="c0450-391">'New-AzExpressRouteConnection'</span></span>
    - <span data-ttu-id="c0450-392">"Set-AzExpressRouteConnection"</span><span class="sxs-lookup"><span data-stu-id="c0450-392">'Set-AzExpressRouteConnection'</span></span>
    - <span data-ttu-id="c0450-393">"New-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="c0450-393">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="c0450-394">"Update-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="c0450-394">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="c0450-395">"New-AzVpnConnection"</span><span class="sxs-lookup"><span data-stu-id="c0450-395">'New-AzVpnConnection'</span></span>
    - <span data-ttu-id="c0450-396">"Update-AzVpnConnection"</span><span class="sxs-lookup"><span data-stu-id="c0450-396">'Update-AzVpnConnection'</span></span>
    - <span data-ttu-id="c0450-397">"New-AzP2sVpnGateway"</span><span class="sxs-lookup"><span data-stu-id="c0450-397">'New-AzP2sVpnGateway'</span></span>
    - <span data-ttu-id="c0450-398">"Update-AzP2sVpnGateway"</span><span class="sxs-lookup"><span data-stu-id="c0450-398">'Update-AzP2sVpnGateway'</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c0450-399">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-399">Az.OperationalInsights</span></span>
* <span data-ttu-id="c0450-400">Correção do erro PSWorkspace não implementa IOperationalInsightsWorkspace [#12135]</span><span class="sxs-lookup"><span data-stu-id="c0450-400">Fixed bug PSWorkspace doesn't implement IOperationalInsightsWorkspace [#12135]</span></span>
* <span data-ttu-id="c0450-401">Adição de "pergb2018" ao conjunto de valores válidos do parâmetro "Sku" em "Set-AzOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="c0450-401">Added 'pergb2018' to valid value set of parameter 'Sku' in 'Set-AzOperationalInsightsWorkspace'</span></span> 
* <span data-ttu-id="c0450-402">Adição do alias "FunctionParameters" para o parâmetro "FunctionParameter" a</span><span class="sxs-lookup"><span data-stu-id="c0450-402">Added alias 'FunctionParameters' for parameter 'FunctionParameter' to</span></span>
    - <span data-ttu-id="c0450-403">"New-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="c0450-403">'New-AzOperationalInsightsSavedSearch'</span></span>
    - <span data-ttu-id="c0450-404">"Set-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="c0450-404">'Set-AzOperationalInsightsSavedSearch'</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-405">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-405">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-406">Adição de suporte no Azure Backup para a obtenção de itens de MAB.</span><span class="sxs-lookup"><span data-stu-id="c0450-406">Azure Backup added support for fetching MAB items.</span></span>
* <span data-ttu-id="c0450-407">Suporte do Azure Site Recovery para o tipo de disco "StandardSSD_LRS"</span><span class="sxs-lookup"><span data-stu-id="c0450-407">Azure Site Recovery supports disk type 'StandardSSD_LRS'</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-408">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-408">Az.Resources</span></span>
* <span data-ttu-id="c0450-409">Adição de "UsageLocation", "GivenName", "Surname", "AccountEnabled", "MailNickname", "Mail" em "PSADUser" [#10526] [#10497]</span><span class="sxs-lookup"><span data-stu-id="c0450-409">Added 'UsageLocation', 'GivenName', 'Surname', 'AccountEnabled', 'MailNickname', 'Mail' on 'PSADUser' [#10526] [#10497]</span></span>
* <span data-ttu-id="c0450-410">Correção do problema em que "-Mail" não funciona em "Get-AzADUser" [#11981]</span><span class="sxs-lookup"><span data-stu-id="c0450-410">Fixed issue that '-Mail' doesn't work on 'Get-AzADUser' [#11981]</span></span>
* <span data-ttu-id="c0450-411">Adição do parâmetro "-ExcludeChangeType" a "Get-AzDeploymentWhatIfResult" e "Get-AzResourceGroupDeploymentWhatIfResult"</span><span class="sxs-lookup"><span data-stu-id="c0450-411">Added '-ExcludeChangeType' parameter to 'Get-AzDeploymentWhatIfResult' and 'Get-AzResourceGroupDeploymentWhatIfResult'</span></span>
* <span data-ttu-id="c0450-412">Adição do parâmetro "-WhatIfExcludeChangeType" a "New-AzDeployment" e "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="c0450-412">Added '-WhatIfExcludeChangeType' parameter to 'New-AzDeployment' and 'New-AzResourceGroupDeployment'</span></span>
* <span data-ttu-id="c0450-413">Atualização de cmdlets "Test-Az\*Deployment" para apresentação de mensagens de erro melhores</span><span class="sxs-lookup"><span data-stu-id="c0450-413">Updated 'Test-Az\*Deployment' cmdlets to show better error messages</span></span>
* <span data-ttu-id="c0450-414">Correção da mensagem de ajuda para o parâmetro "-Name" de criação de implementação e cmdlets What-If</span><span class="sxs-lookup"><span data-stu-id="c0450-414">Fixed help message for '-Name' parameter of deployment create and What-If cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-415">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-415">Az.Sql</span></span>
* <span data-ttu-id="c0450-416">Adição de suporte para o principal de serviço para o cmdlet Set SQL Server Azure Active Directory Admin</span><span class="sxs-lookup"><span data-stu-id="c0450-416">Added support for service principal for Set SQL Server Azure Active Directory Admin cmdlet</span></span>
* <span data-ttu-id="c0450-417">Correção de problema de sincronização em cmdlets de Classificação de Dados.</span><span class="sxs-lookup"><span data-stu-id="c0450-417">Fixed sync issue in Data Classification cmdlets.</span></span>
* <span data-ttu-id="c0450-418">Suporte para a pesquisa de utilizador por correio em "Set-AzSqlServerActiveDirectoryAdministrator" [#12192]</span><span class="sxs-lookup"><span data-stu-id="c0450-418">Supported searching user by mail on 'Set-AzSqlServerActiveDirectoryAdministrator' [#12192]</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-419">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-419">Az.Storage</span></span>
* <span data-ttu-id="c0450-420">Suporte para a criação de Conta de armazenamento com RequireInfrastructureEncryption</span><span class="sxs-lookup"><span data-stu-id="c0450-420">Supported create Storage account with RequireInfrastructureEncryption</span></span>
    -  <span data-ttu-id="c0450-421">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c0450-421">'New-AzStorageAccount'</span></span>
* <span data-ttu-id="c0450-422">Mudança da lógica de carregamento de Azure.Core para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-422">Moved the logic of loading Azure.Core to Az.Accounts</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c0450-423">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-423">Az.Websites</span></span>
* <span data-ttu-id="c0450-424">Adição de salvaguarda para eliminar a aplicação Web criada em caso de falha do restauro em "Restore-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="c0450-424">Added safeguard to delete created webapp if restore failed in 'Restore-AzDeletedWebApp'</span></span>
* <span data-ttu-id="c0450-425">Adição de "SourceWebApp.Location" para "New-AzWebApp" e "New-AzWebAppSlot"</span><span class="sxs-lookup"><span data-stu-id="c0450-425">Added 'SourceWebApp.Location' for 'New-AzWebApp' and 'New-AzWebAppSlot'</span></span>
* <span data-ttu-id="c0450-426">Correção do erro que impedia a alteração de definições de Contentor em "Set-AzWebApp" e "Set-AzWebAppSlot"</span><span class="sxs-lookup"><span data-stu-id="c0450-426">Fixed bug that prevented changing Container settings in 'Set-AzWebApp' and 'Set-AzWebAppSlot'</span></span>
* <span data-ttu-id="c0450-427">Correção do erro para obter SiteConfig quando -Name não é fornecido para Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="c0450-427">Fixed bug to get SiteConfig when -Name is not given for Get-AzWebApp</span></span>
* <span data-ttu-id="c0450-428">Adição de suporte para a criação de ASP para Aplicações Linux</span><span class="sxs-lookup"><span data-stu-id="c0450-428">Added a support to create ASP for Linux Apps</span></span>
* <span data-ttu-id="c0450-429">Adição de exceções para clonagem entre grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="c0450-429">Added exceptions for clone across resource groups</span></span>

## <a name="420---june-2020"></a><span data-ttu-id="c0450-430">4.2.0 - Junho de 2020</span><span class="sxs-lookup"><span data-stu-id="c0450-430">4.2.0 - June 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c0450-431">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-431">Az.Accounts</span></span>
* <span data-ttu-id="c0450-432">Correção de um problema que fazia com que o Az ignorasse registos nas tarefas da Automatização do Azure ou do PowerShell [#11492]</span><span class="sxs-lookup"><span data-stu-id="c0450-432">Fixed an issue that may cause Az to skip logs in Azure Automation or PowerShell jobs [#11492]</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="c0450-433">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c0450-433">Az.AnalysisServices</span></span>
* <span data-ttu-id="c0450-434">Atualização da versão de assemblagem dos cmdlets de plano de dados</span><span class="sxs-lookup"><span data-stu-id="c0450-434">Updated assembly version of data plane cmdlets</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c0450-435">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c0450-435">Az.ApiManagement</span></span>
* <span data-ttu-id="c0450-436">Atualização da versão de assemblagem dos cmdlets de gestão de serviços</span><span class="sxs-lookup"><span data-stu-id="c0450-436">Updated assembly version of service management cmdlets</span></span>

#### <a name="azbilling"></a><span data-ttu-id="c0450-437">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="c0450-437">Az.Billing</span></span>
* <span data-ttu-id="c0450-438">Atualização da versão de assemblagem dos cmdlets de consumo</span><span class="sxs-lookup"><span data-stu-id="c0450-438">Updated assembly version of consumption cmdlets</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c0450-439">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c0450-439">Az.CognitiveServices</span></span>
* <span data-ttu-id="c0450-440">Suporte para o controlo de PrivateEndpoint e PublicNetworkAccess.</span><span class="sxs-lookup"><span data-stu-id="c0450-440">Support PrivateEndpoint and PublicNetworkAccess control.</span></span> 

#### <a name="azdatafactory"></a><span data-ttu-id="c0450-441">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c0450-441">Az.DataFactory</span></span>
* <span data-ttu-id="c0450-442">Atualização da versão de assemblagem dos cmdlets V2 de fábrica de dados</span><span class="sxs-lookup"><span data-stu-id="c0450-442">Updated assembly version of data factory V2 cmdlets</span></span>

#### <a name="azdatashare"></a><span data-ttu-id="c0450-443">Az.DataShare</span><span class="sxs-lookup"><span data-stu-id="c0450-443">Az.DataShare</span></span>
* <span data-ttu-id="c0450-444">Disponibilidade geral do módulo "Az.DataShare"</span><span class="sxs-lookup"><span data-stu-id="c0450-444">General availability of ''Az.DataShare'' module</span></span>

#### <a name="azdesktopvirtualization"></a><span data-ttu-id="c0450-445">Az.DesktopVirtualization</span><span class="sxs-lookup"><span data-stu-id="c0450-445">Az.DesktopVirtualization</span></span>
* <span data-ttu-id="c0450-446">Disponibilidade geral do módulo "Az.DesktopVirtualization"</span><span class="sxs-lookup"><span data-stu-id="c0450-446">General availability of ''Az.DesktopVirtualization'' module</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c0450-447">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-447">Az.OperationalInsights</span></span>
* <span data-ttu-id="c0450-448">Atualização do SDK para a versão 0.21.0</span><span class="sxs-lookup"><span data-stu-id="c0450-448">Upgraded SDK to 0.21.0</span></span>
* <span data-ttu-id="c0450-449">Adição de parâmetros opcionais a</span><span class="sxs-lookup"><span data-stu-id="c0450-449">Added optional parameters to</span></span> 
    - <span data-ttu-id="c0450-450">"New-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="c0450-450">'New-AzOperationalInsightsSavedSearch'</span></span>
    - <span data-ttu-id="c0450-451">"Set-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="c0450-451">'Set-AzOperationalInsightsSavedSearch'</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c0450-452">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-452">Az.PolicyInsights</span></span>
* <span data-ttu-id="c0450-453">Correção do exemplo 3 de "Start-AzPolicyComplianceScan"</span><span class="sxs-lookup"><span data-stu-id="c0450-453">Corrected example 3 for 'Start-AzPolicyComplianceScan'</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="c0450-454">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="c0450-454">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="c0450-455">Atualização da versão de assemblagem dos cmdlets do PowerBI</span><span class="sxs-lookup"><span data-stu-id="c0450-455">Updated assembly version of PowerBI cmdlets</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="c0450-456">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="c0450-456">Az.PrivateDns</span></span>
* <span data-ttu-id="c0450-457">Correção da formatação da cadeia de saída verbosa de Remove-AzPrivateDnsRecordSet</span><span class="sxs-lookup"><span data-stu-id="c0450-457">Corrected verbose output string formatting for Remove-AzPrivateDnsRecordSet</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-458">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-458">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-459">Suporte do Azure Site Recovery para a criação de um plano de recuperação para replicação zona a zona a partir de uma entrada xml.</span><span class="sxs-lookup"><span data-stu-id="c0450-459">Azure Site Recovery support for creating recovery plan for zone to zone replication from xml input.</span></span>
* <span data-ttu-id="c0450-460">Atualização da versão de assemblagem dos cmdlets do SiteRecovery e Backup</span><span class="sxs-lookup"><span data-stu-id="c0450-460">Updated assembly version of SiteRecovery and Backup cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-461">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-461">Az.Resources</span></span>
* <span data-ttu-id="c0450-462">Adição do parâmetro Tail aos cmdlets Get-AzDeploymentScriptLog e Save-AzDeploymentScriptLog</span><span class="sxs-lookup"><span data-stu-id="c0450-462">Added Tail parameter to Get-AzDeploymentScriptLog and Save-AzDeploymentScriptLog cmdlets</span></span>
* <span data-ttu-id="c0450-463">Formatação da propriedade Output e apresentação da mesma na saída do cmdlet Get-AzDeploymentScript</span><span class="sxs-lookup"><span data-stu-id="c0450-463">Formatted Output property and show it on the Get-AzDeploymentScript cmdlet output</span></span>
* <span data-ttu-id="c0450-464">Mudança de nome do parâmetro -DeploymentScriptInputObject para -DeploymentScriptObject</span><span class="sxs-lookup"><span data-stu-id="c0450-464">Renamed -DeploymentScriptInputObject parameter to -DeploymentScriptObject</span></span>
* <span data-ttu-id="c0450-465">Correção do nome em falta do ficheiro/destino nas mensagens de cmdlet.</span><span class="sxs-lookup"><span data-stu-id="c0450-465">Fixed missing file/target name in cmdlet messages.</span></span>
* <span data-ttu-id="c0450-466">Atualização da versão de assemblagem dos cmdlets de gestor de recursos e de etiquetas</span><span class="sxs-lookup"><span data-stu-id="c0450-466">Updated assembly version of resource manager and tags cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-467">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-467">Az.Sql</span></span>
* <span data-ttu-id="c0450-468">Adição de UsePrivateLinkConnection a "New-AzSqlSyncGroup", "Update-AzSqlSyncGroup", "New-AzSqlSyncMember" e "Update-AzSqlSyncMember"</span><span class="sxs-lookup"><span data-stu-id="c0450-468">Added UsePrivateLinkConnection to 'New-AzSqlSyncGroup', 'Update-AzSqlSyncGroup', 'New-AzSqlSyncMember' and 'Update-AzSqlSyncMember'</span></span>
* <span data-ttu-id="c0450-469">Adição de SyncMemberAzureDatabaseResourceId a "New-AzSqlSyncMember" e "Update-AzSqlSyncMember"</span><span class="sxs-lookup"><span data-stu-id="c0450-469">Added SyncMemberAzureDatabaseResourceId to 'New-AzSqlSyncMember' and 'Update-AzSqlSyncMember'</span></span>
* <span data-ttu-id="c0450-470">Adição do suporte de pesquisa de Utilizador convidado ao cmdlet Set SQL Server Azure Active Directory Admin</span><span class="sxs-lookup"><span data-stu-id="c0450-470">Added Guest user lookup support to Set SQL Server Azure Active Directory Admin cmdlet</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-471">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-471">Az.Storage</span></span>
* <span data-ttu-id="c0450-472">Atualização da versão de assemblagem dos cmdlets de plano de dados</span><span class="sxs-lookup"><span data-stu-id="c0450-472">Updated assembly version of data plane cmdlets</span></span>

## <a name="410---may-2020"></a><span data-ttu-id="c0450-473">4.1.0 - Maio de 2020</span><span class="sxs-lookup"><span data-stu-id="c0450-473">4.1.0 - May 2020</span></span>
### <a name="highlights-since-the-last-release"></a><span data-ttu-id="c0450-474">Destaques desde a última versão</span><span class="sxs-lookup"><span data-stu-id="c0450-474">Highlights since the last release</span></span>
* <span data-ttu-id="c0450-475">Versões do PowerShell suportadas: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span><span class="sxs-lookup"><span data-stu-id="c0450-475">Supported PowerShell versions: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span></span>
* <span data-ttu-id="c0450-476">Disponibilidade geral de Az.Functions</span><span class="sxs-lookup"><span data-stu-id="c0450-476">General availability of Az.Functions</span></span> 
* <span data-ttu-id="c0450-477">Az.ApiManagement, Az.Batch, Az.Compute, Az.KeyVault, Az.Monitor, Az.Network, Az.OperationalInsights, Az.Resources e Az.Storage são alvo de grandes versões</span><span class="sxs-lookup"><span data-stu-id="c0450-477">Az.ApiManagement, Az.Batch, Az.Compute, Az.KeyVault, Az.Monitor, Az.Network, Az.OperationalInsights, Az.Resources, and Az.Storage have major release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c0450-478">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-478">Az.Accounts</span></span>
* <span data-ttu-id="c0450-479">"Add-AzEnvironment" e "Set-AzEnvironment" foram atualizados para aceitar os parâmetros "AzureSynapseAnalyticsEndpointResourceId" e "AzureSynapseAnalyticsEndpointSuffix"</span><span class="sxs-lookup"><span data-stu-id="c0450-479">Updated 'Add-AzEnvironment' and 'Set-AzEnvironment' to accept parameters 'AzureSynapseAnalyticsEndpointResourceId' and 'AzureSynapseAnalyticsEndpointSuffix'</span></span>
* <span data-ttu-id="c0450-480">Foram adicionadas assemblagens relacionadas ao Azure.Core em Az.Accounts; as plataformas suportadas do PowerShell incluem Windows PowerShell 5.1, PowerShell Core 6.2.4, PowerShell 7+</span><span class="sxs-lookup"><span data-stu-id="c0450-480">Added Azure.Core related assemblies into Az.Accounts, supported PowerShell platforms include Windows PowerShell 5.1, PowerShell Core 6.2.4, PowerShell 7+</span></span>

#### <a name="azaks"></a><span data-ttu-id="c0450-481">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="c0450-481">Az.Aks</span></span>
* <span data-ttu-id="c0450-482">Versão da API atualizada para 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="c0450-482">Upgraded API Version to 2019-10-01</span></span>
* <span data-ttu-id="c0450-483">Suportado para criar o AKS com contentores do Windows</span><span class="sxs-lookup"><span data-stu-id="c0450-483">Supported to create AKS using Windows container</span></span>
* <span data-ttu-id="c0450-484">Novos cmdlets fornecidos: "New-AzAksNodePool", "Update-AzAksNodePool", "Remove-AzAksNodePool",        "Get-AzAksNodePool", "Install-AzAksKubectl", "Get-AzAksVersion"</span><span class="sxs-lookup"><span data-stu-id="c0450-484">Provided new cmdlets: 'New-AzAksNodePool', 'Update-AzAksNodePool', 'Remove-AzAksNodePool',        'Get-AzAksNodePool', 'Install-AzAksKubectl', 'Get-AzAksVersion'</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c0450-485">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c0450-485">Az.ApiManagement</span></span>
* <span data-ttu-id="c0450-486">"New-AzApiManagement" e "Set-AzApiManagement": o nome do parâmetro [-AssignIdentity] foi mudado para [-SystemAssignedIdentity]</span><span class="sxs-lookup"><span data-stu-id="c0450-486">'New-AzApiManagement' and 'Set-AzApiManagement': [-AssignIdentity] parameter renamed as [-SystemAssignedIdentity]</span></span>
* <span data-ttu-id="c0450-487">"New-AzApiManagement" e "Set-AzApiManagement": Novo parâmetro adicionado: [-UserAssignedIdentity <String[]>]</span><span class="sxs-lookup"><span data-stu-id="c0450-487">'New-AzApiManagement' and 'Set-AzApiManagement': New parameter added: [-UserAssignedIdentity <String[]>]</span></span>
* <span data-ttu-id="c0450-488">"Get-AzApiManagementProperty": o nome foi mudado para "Get-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="c0450-488">'Get-AzApiManagementProperty': renamed as 'Get-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="c0450-489">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="c0450-489">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="c0450-490">"New-AzApiManagementProperty": o nome foi mudado para "New-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="c0450-490">'New-AzApiManagementProperty': renamed as 'New-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="c0450-491">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="c0450-491">PropertyId parameter renamed as NamedValueId.</span></span> 
* <span data-ttu-id="c0450-492">"Set-AzApiManagementProperty": o nome foi mudado para "Set-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="c0450-492">'Set-AzApiManagementProperty': renamed as 'Set-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="c0450-493">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="c0450-493">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="c0450-494">"Remove-AzApiManagementProperty": o nome foi mudado para "Remove-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="c0450-494">'Remove-AzApiManagementProperty': renamed as 'Remove-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="c0450-495">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="c0450-495">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="c0450-496">Foi adicionado o cmdlet novo "Get-AzApiManagementAuthorizationServerClientSecret" e "Get-AzApiManagementAuthorizationServer" vai deixar de devolver o segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="c0450-496">Added new 'Get-AzApiManagementAuthorizationServerClientSecret' cmdlet and 'Get-AzApiManagementAuthorizationServer' will not return client secret anymore.</span></span>
* <span data-ttu-id="c0450-497">Foi adicionado o cmdlet novo "Get-AzApiManagementNamedValueSecretValue" e "Get-AzApiManagementNamedValue" vai deixar de devolver o valor do segredo.</span><span class="sxs-lookup"><span data-stu-id="c0450-497">Added new 'Get-AzApiManagementNamedValueSecretValue' cmdlet and 'Get-AzApiManagementNamedValue' will not return secret value.</span></span>
* <span data-ttu-id="c0450-498">Foi adicionado o cmdlet novo "Get-AzApiManagementOpenIdConnectProviderClientSecret" e "Get-AzApiManagementOpenIdConnectProvider" vai deixar de devolver o segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="c0450-498">Added new 'Get-AzApiManagementOpenIdConnectProviderClientSecret' cmdlet and 'Get-AzApiManagementOpenIdConnectProvider' will not return client secret anymore.</span></span>
* <span data-ttu-id="c0450-499">Foi adicionado o cmdlet "Get-AzApiManagementSubscriptionKey" e "Get-AzApiManagementSubscription" vai deixar de devolver chaves de subscrições.</span><span class="sxs-lookup"><span data-stu-id="c0450-499">Added new 'Get-AzApiManagementSubscriptionKey' cmdlet and 'Get-AzApiManagementSubscription' will not return subscription keys anymore.</span></span>
* <span data-ttu-id="c0450-500">Foi adicionado o cmdlet novo "Get-AzApiManagementTenantAccessSecret" e "Get-AzApiManagementTenantAccess" vai deixar de devolver chaves.</span><span class="sxs-lookup"><span data-stu-id="c0450-500">Added new 'Get-AzApiManagementTenantAccessSecret' cmdlet and 'Get-AzApiManagementTenantAccess' will not return keys anymore.</span></span>
* <span data-ttu-id="c0450-501">Foi adicionado o cmdlet novo "Get-AzApiManagementTenantGitAccessSecret" e "Get-AzApiManagementTenantGitAccess" vai deixar de devolver chaves.</span><span class="sxs-lookup"><span data-stu-id="c0450-501">Added new 'Get-AzApiManagementTenantGitAccessSecret' cmdlet and 'Get-AzApiManagementTenantGitAccess' will not return keys anymore.</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="c0450-502">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-502">Az.ApplicationInsights</span></span>
* <span data-ttu-id="c0450-503">Parâmetros adicionados: "RetentionInDays" "PublicNetworkAccessForIngestion" "PublicNetworkAccessForQuery" a "New-AzApplicationInsights"</span><span class="sxs-lookup"><span data-stu-id="c0450-503">Added Parameters: 'RetentionInDays' 'PublicNetworkAccessForIngestion' 'PublicNetworkAccessForQuery' for 'New-AzApplicationInsights'</span></span>
* <span data-ttu-id="c0450-504">Foi criado o cmdlet "Update-AzApplicationInsights”</span><span class="sxs-lookup"><span data-stu-id="c0450-504">Created cmdlet 'Update-AzApplicationInsights'</span></span>
* <span data-ttu-id="c0450-505">Foram criados cmdlets para a Conta de Armazenamento Associada</span><span class="sxs-lookup"><span data-stu-id="c0450-505">Created cmdlets for Linked Storage Account</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c0450-506">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c0450-506">Az.Batch</span></span>
* <span data-ttu-id="c0450-507">Az.Batch foi atualizado para utilizar a versão do SDK "Microsoft.Azure.Batc" 13.0.0 e a versão do SDK "Microsoft.Azure.Management.Batch" 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="c0450-507">Updated Az.Batch to use 'Microsoft.Azure.Batch' SDK version 13.0.0 and 'Microsoft.Azure.Management.Batch' SDK version 9.0.0.</span></span>
* <span data-ttu-id="c0450-508">Foi adicionada a capacidade de selecionar o tipo de certificado que vai ser adicionado mediante a utilização do novo parâmetro "-CertificateKind" para "New-AzBatchCertificate".</span><span class="sxs-lookup"><span data-stu-id="c0450-508">Added the ability to select the kind of certificate being added using the new '-CertificateKind' parameter to 'New-AzBatchCertificate'.</span></span>
* <span data-ttu-id="c0450-509">A propriedade "ApplicationPackages" foi removida de "PSApplication", que anteriormente era sempre ''.</span><span class="sxs-lookup"><span data-stu-id="c0450-509">Removed 'ApplicationPackages' property from 'PSApplication' which was previously always ''.</span></span>
  - <span data-ttu-id="c0450-510">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com "Get-AzBatchApplicationPackage".</span><span class="sxs-lookup"><span data-stu-id="c0450-510">The specific packages inside of an application now can be retrieved using 'Get-AzBatchApplicationPackage'.</span></span> <span data-ttu-id="c0450-511">Por exemplo: "Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication".</span><span class="sxs-lookup"><span data-stu-id="c0450-511">For example: 'Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication'.</span></span>
* <span data-ttu-id="c0450-512">Agora, ao utilizar "New-AzBatchPool" para criar um conjunto, a propriedade "VirtualMachineImageId" de "PSImageReference" só pode fazer referência a uma imagem do Shared Image Gallery.</span><span class="sxs-lookup"><span data-stu-id="c0450-512">When creating a pool using 'New-AzBatchPool', the 'VirtualMachineImageId' property of 'PSImageReference' can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="c0450-513">Ao utilizar "New-AzBatchPool" para criar um conjunto, o conjunto pode ser aprovisionado sem um IP público mediante a utilização da nova propriedade "PublicIPAddressConfiguration" de "PSNetworkConfiguration".</span><span class="sxs-lookup"><span data-stu-id="c0450-513">When creating a pool using 'New-AzBatchPool', the pool can be provisioned without a public IP using the new 'PublicIPAddressConfiguration' property of 'PSNetworkConfiguration'.</span></span>
  - <span data-ttu-id="c0450-514">A propriedade "PublicIPs" de "PSNetworkConfiguration" foi igualmente movida para "PSPublicIPAddressConfiguration".</span><span class="sxs-lookup"><span data-stu-id="c0450-514">The 'PublicIPs' property of 'PSNetworkConfiguration' has moved in to 'PSPublicIPAddressConfiguration' as well.</span></span> <span data-ttu-id="c0450-515">Esta propriedade só pode ser especificada se "IPAddressProvisioningType" for "UserManaged".</span><span class="sxs-lookup"><span data-stu-id="c0450-515">This property can only be specified if 'IPAddressProvisioningType' is 'UserManaged'.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-516">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-516">Az.Compute</span></span>
* <span data-ttu-id="c0450-517">Foi adicionado o parâmetro HostId ao cmdlet "Update-AzVM"</span><span class="sxs-lookup"><span data-stu-id="c0450-517">Added HostId parameter to 'Update-AzVM' cmdlet</span></span>
* <span data-ttu-id="c0450-518">Os documentos de Ajuda para os cmdlets "New-AzVMConfig", "New-AzVmssConfig", "Update-AzVmss", "Set-AzVMOperatingSystem" e "Set-AzVmssOsProfile" foram atualizados.</span><span class="sxs-lookup"><span data-stu-id="c0450-518">Updated Help documents for 'New-AzVMConfig', 'New-AzVmssConfig', 'Update-AzVmss', 'Set-AzVMOperatingSystem' and 'Set-AzVmssOsProfile' cmdlets.</span></span>
* <span data-ttu-id="c0450-519">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="c0450-519">Breaking changes</span></span>
    - <span data-ttu-id="c0450-520">O parâmetro FilterExpression foi removido do cmdlet "Get-AzVMImage".</span><span class="sxs-lookup"><span data-stu-id="c0450-520">FilterExpression parameter is removed from 'Get-AzVMImage' cmdlet.</span></span>
    - <span data-ttu-id="c0450-521">O parâmetro AssignIdentity foi removido dos cmdlets "New-AzVmssConfig", "New-AzVMConfig" e "Update-AzVM".</span><span class="sxs-lookup"><span data-stu-id="c0450-521">AssignIdentity parameter is removed from 'New-AzVmssConfig', 'New-AzVMConfig' and 'Update-AzVM' cmdlets.</span></span>
    - <span data-ttu-id="c0450-522">AutomaticRepairMaxInstanceRepairsPercent foi removido dos cmdlets "New-AzVmssConfig" e "Update-AzVmss".</span><span class="sxs-lookup"><span data-stu-id="c0450-522">AutomaticRepairMaxInstanceRepairsPercent is removed from 'New-AzVmssConfig' and 'Update-AzVmss' cmdlets.</span></span>
    - <span data-ttu-id="c0450-523">As propriedades AvailabilitySetsColocationStatus, VirtualMachinesColocationStatus e VirtualMachineScaleSetsColocationStatus foram removidas de ProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="c0450-523">AvailabilitySetsColocationStatus, VirtualMachinesColocationStatus and VirtualMachineScaleSetsColocationStatus properties are removed from ProximityPlacementGroup.</span></span>
    - <span data-ttu-id="c0450-524">A propriedade MaxInstanceRepairsPercent foi removida de AutomaticRepairsPolicy.</span><span class="sxs-lookup"><span data-stu-id="c0450-524">MaxInstanceRepairsPercent property is removed from AutomaticRepairsPolicy.</span></span>
    - <span data-ttu-id="c0450-525">Os tipos de AvailabilitySets, VirtualMachines e VirtualMachineScaleSets foram alterados de IList<SubResource> para IList<SubResourceWithColocationStatus>.</span><span class="sxs-lookup"><span data-stu-id="c0450-525">The types of AvailabilitySets, VirtualMachines and VirtualMachineScaleSets are changed from IList<SubResource> to IList<SubResourceWithColocationStatus>.</span></span>
* <span data-ttu-id="c0450-526">A descrição do cmdlet "Get-AzVM" foi atualizada para o descrever melhor.</span><span class="sxs-lookup"><span data-stu-id="c0450-526">Description for 'Get-AzVM' cmdlet has been updated to better describe it.</span></span> 

#### <a name="azdatafactory"></a><span data-ttu-id="c0450-527">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c0450-527">Az.DataFactory</span></span>
* <span data-ttu-id="c0450-528">CRUD suportado das propriedades de fluxo de dados no IR Gerido.</span><span class="sxs-lookup"><span data-stu-id="c0450-528">Supported CRUD of data flow runtime properties in Managed IR.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c0450-529">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c0450-529">Az.FrontDoor</span></span>
* <span data-ttu-id="c0450-530">Foram adicionados cmdlets novos para criação, atualização, obtenção e eliminação do objeto de Motor de Regras do Front Door</span><span class="sxs-lookup"><span data-stu-id="c0450-530">Added new cmdlets for creation, update, retreival, and deletion of Front Door Rules Engine object</span></span>
* <span data-ttu-id="c0450-531">Foram adicionados cmdlets de programas auxiliares para construção do objeto de Motor de Regras do Front Door</span><span class="sxs-lookup"><span data-stu-id="c0450-531">Added helper cmdlets for construction of Front Door Rules Engine object</span></span>
* <span data-ttu-id="c0450-532">Foi adicionada a referência ao Motor de Regras ao objeto Regra de Encaminhamento do Front Door.</span><span class="sxs-lookup"><span data-stu-id="c0450-532">Added Rules Engine reference to Front Door Routing Rule object.</span></span>
* <span data-ttu-id="c0450-533">Foram adicionados parâmetros do Private Link ao objeto de Back-end do Front Door</span><span class="sxs-lookup"><span data-stu-id="c0450-533">Added Private Link parameters to Front Door Backend object</span></span>

#### <a name="azfunctions"></a><span data-ttu-id="c0450-534">Az.Functions</span><span class="sxs-lookup"><span data-stu-id="c0450-534">Az.Functions</span></span>
* <span data-ttu-id="c0450-535">Disponibilidade geral do módulo Az.Functions</span><span class="sxs-lookup"><span data-stu-id="c0450-535">General availability of ''Az.Functions'' module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c0450-536">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c0450-536">Az.HDInsight</span></span>
* <span data-ttu-id="c0450-537">Encriptação de discos de chave gerida pelo cliente suportada</span><span class="sxs-lookup"><span data-stu-id="c0450-537">Supported Customer-managed key disk encryption.</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="c0450-538">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="c0450-538">Az.HealthcareApis</span></span>
* <span data-ttu-id="c0450-539">As políticas de acesso já não são predefinidas para o principal atual</span><span class="sxs-lookup"><span data-stu-id="c0450-539">Access policies are no longer defaulted to the current principal</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c0450-540">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c0450-540">Az.IotHub</span></span>
* <span data-ttu-id="c0450-541">Foi adicionado um cmdlet para invocar uma consulta num hub IoT para obter informações mediante a utilização de uma linguagem tipo SQL.</span><span class="sxs-lookup"><span data-stu-id="c0450-541">Added cmdlet to invoke a query in an IoT hub to retrieve information using a SQL-like language.</span></span>
* <span data-ttu-id="c0450-542">Foi corrigido um problema em que "Add-AzIotHubDevice" falha ao criar um Dispositivo Compatível com o Edge sem dispositivos subordinados [#11597]</span><span class="sxs-lookup"><span data-stu-id="c0450-542">Fix issue that 'Add-AzIotHubDevice' fails to create Edge Enabled Device without child devices [#11597]</span></span>
* <span data-ttu-id="c0450-543">Foi adicionado o cmdlet para gerar o token de SAS para o Hub IoT, um dispositivo ou um módulo.</span><span class="sxs-lookup"><span data-stu-id="c0450-543">Added cmdlet to generate SAS token for Iot Hub, device or module.</span></span>
* <span data-ttu-id="c0450-544">Foi adicionado um cmdlet para invocar a consulta de métricas de configuração.</span><span class="sxs-lookup"><span data-stu-id="c0450-544">Added cmdlet to invoke configuration metrics query.</span></span>
* <span data-ttu-id="c0450-545">Gerir implementações automáticas do IoT Edge em escala.</span><span class="sxs-lookup"><span data-stu-id="c0450-545">Manage IoT Edge automatic deployment at scale.</span></span> <span data-ttu-id="c0450-546">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="c0450-546">New cmdlets are:</span></span>
    - <span data-ttu-id="c0450-547">"Add-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="c0450-547">'Add-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="c0450-548">"Get-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="c0450-548">'Get-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="c0450-549">"Remove-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="c0450-549">'Remove-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="c0450-550">"Set-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="c0450-550">'Set-AzIotHubDeployment'</span></span>
* <span data-ttu-id="c0450-551">Foi adicionado um cmdlet para invocar uma consulta de métricas de implementação do IoT Edge.</span><span class="sxs-lookup"><span data-stu-id="c0450-551">Added cmdlet to invoke an IoT Edge deployment metrics query.</span></span>
* <span data-ttu-id="c0450-552">Foi adicionado um cmdlet para aplicar o conteúdo da configuração ao dispositivo edge especificado.</span><span class="sxs-lookup"><span data-stu-id="c0450-552">Added cmdlet to apply the configuration content to the specified edge device.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c0450-553">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0450-553">Az.KeyVault</span></span>
* <span data-ttu-id="c0450-554">Foram removidos dois aliases: "New-AzKeyVaultCertificateAdministratorDetails" e "New-AzKeyVaultCertificateOrganizationDetails"</span><span class="sxs-lookup"><span data-stu-id="c0450-554">Removed two aliases: 'New-AzKeyVaultCertificateAdministratorDetails' and 'New-AzKeyVaultCertificateOrganizationDetails'</span></span>
* <span data-ttu-id="c0450-555">A eliminação recuperável foi ativada por predefinição ao criar um cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="c0450-555">Enabled soft delete by default when creating a key vault</span></span>
* <span data-ttu-id="c0450-556">Podem ser definidas regras de rede para governar a acessibilidade a partir de localizações na rede ao criar um cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="c0450-556">Network rules can be set to govern the accessibility from specific network locations when creating a key vault</span></span>
* <span data-ttu-id="c0450-557">Foi adicionado suporte para Bring Your Own Key (BYOK)</span><span class="sxs-lookup"><span data-stu-id="c0450-557">Added support to bring your own key (BYOK)</span></span>
    - <span data-ttu-id="c0450-558">"Add-AzKeyVaultKey" suporta a geração de chaves de intercâmbio de chaves</span><span class="sxs-lookup"><span data-stu-id="c0450-558">'Add-AzKeyVaultKey' supports generating a key exchange key</span></span>
    - <span data-ttu-id="c0450-559">"Get-AzKeyVaultKey" suporta a transferência de chaves públicas no formato PEM</span><span class="sxs-lookup"><span data-stu-id="c0450-559">'Get-AzKeyVaultKey' supports downloading a public key in PEM format</span></span>
* <span data-ttu-id="c0450-560">"KeyOps" foi atualizado como parte do documento de ajuda de "Add-AzKeyVaultKey"</span><span class="sxs-lookup"><span data-stu-id="c0450-560">Updated the 'KeyOps' part of the help document of 'Add-AzKeyVaultKey'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c0450-561">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c0450-561">Az.Monitor</span></span>
* <span data-ttu-id="c0450-562">Foi corrigido um erro em "Set-AzDiagnosticSettings"; a política de retenção não se aplicará a todas as categorias [#11589]</span><span class="sxs-lookup"><span data-stu-id="c0450-562">Fixed bug for 'Set-AzDiagnosticSettings', retention policy won't apply to all categories [#11589]</span></span>
* <span data-ttu-id="c0450-563">Suporte para critérios de disponibilidade de WebTest para alertas de métricas V2</span><span class="sxs-lookup"><span data-stu-id="c0450-563">Supported WebTest availability criteria for metric alert V2</span></span>
    - <span data-ttu-id="c0450-564">Novo "New-AzMetricAlertRuleV2Criteria": foi adicionada uma opção para criar critérios de disponibilidade WebTest</span><span class="sxs-lookup"><span data-stu-id="c0450-564">'New-AzMetricAlertRuleV2Criteria': an option to create webtest availability criteria was added</span></span>
    - <span data-ttu-id="c0450-565">"Add-AzMetricAlertRuleV2": suporta os novos critérios de disponibilidade de WebTest</span><span class="sxs-lookup"><span data-stu-id="c0450-565">'Add-AzMetricAlertRuleV2': supports the new webtest availability criteria</span></span>
* <span data-ttu-id="c0450-566">Foi removida a definição redundante de RetentionPolicy em PSLogProfile [#7608]</span><span class="sxs-lookup"><span data-stu-id="c0450-566">Removed redundant definition for RetentionPolicy in PSLogProfile [#7608]</span></span>
* <span data-ttu-id="c0450-567">Foram removidas as propriedades redundantes definidas em PSEventData [#11353]</span><span class="sxs-lookup"><span data-stu-id="c0450-567">Removed redundant properties difined in PSEventData [#11353]</span></span>
* <span data-ttu-id="c0450-568">O nome de "Get-AzLog" foi mudado para "Get-AzActivityLog"</span><span class="sxs-lookup"><span data-stu-id="c0450-568">Renamed 'Get-AzLog' to 'Get-AzActivityLog'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-569">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-569">Az.Network</span></span>
* <span data-ttu-id="c0450-570">Foi adicionado um atributo de alteração interruptiva para notificar que o comportamento predefinido da Zona vai ser alterado</span><span class="sxs-lookup"><span data-stu-id="c0450-570">Added breaking change attribute to notify that Zone default behaviour will be changed</span></span>
    - <span data-ttu-id="c0450-571">"New-AzPublicIpAddress"</span><span class="sxs-lookup"><span data-stu-id="c0450-571">'New-AzPublicIpAddress'</span></span>
    - <span data-ttu-id="c0450-572">"New-AzPublicIpPrefix"</span><span class="sxs-lookup"><span data-stu-id="c0450-572">'New-AzPublicIpPrefix'</span></span>
    - <span data-ttu-id="c0450-573">"New-AzLoadBalancerFrontendIpConfig"</span><span class="sxs-lookup"><span data-stu-id="c0450-573">'New-AzLoadBalancerFrontendIpConfig'</span></span>
* <span data-ttu-id="c0450-574">Foi adicionado suportado para um recurso de nível superior novo SecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="c0450-574">Added support for a new top level resource SecurityPartnerProvider</span></span>
    - <span data-ttu-id="c0450-575">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c0450-575">New cmdlets added:</span></span>
        - <span data-ttu-id="c0450-576">New-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="c0450-576">New-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="c0450-577">Remove-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="c0450-577">Remove-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="c0450-578">Get-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="c0450-578">Get-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="c0450-579">Set-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="c0450-579">Set-AzSecurityPartnerProvider</span></span>
* <span data-ttu-id="c0450-580">Foi adicionado "RequiredZoneNames" em "PSPrivateLinkResource" e "GroupId" em "PSPrivateEndpointConnection”</span><span class="sxs-lookup"><span data-stu-id="c0450-580">Added 'RequiredZoneNames' on 'PSPrivateLinkResource' and 'GroupId' on 'PSPrivateEndpointConnection'</span></span>
* <span data-ttu-id="c0450-581">Foi corrigido o tipo incorreto do parâmetro SuccessThresholdRoundTripTimeMs para New-AzNetworkWatcherConnectionMonitorTestConfigurationObject</span><span class="sxs-lookup"><span data-stu-id="c0450-581">Fixed incorrect type of SuccessThresholdRoundTripTimeMs parameter for New-AzNetworkWatcherConnectionMonitorTestConfigurationObject</span></span>
* <span data-ttu-id="c0450-582">Foram atualizados os cmdlets VirtualWan para definir o valor predefinido do argumento AllowVnetToVnetTraffic como Verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="c0450-582">Updated VirtualWan cmdlets to set default value of AllowVnetToVnetTraffic argument to True.</span></span>
    - <span data-ttu-id="c0450-583">"New-AzVirtualWan"</span><span class="sxs-lookup"><span data-stu-id="c0450-583">'New-AzVirtualWan'</span></span>
    - <span data-ttu-id="c0450-584">"Update-AzVirtualWan"</span><span class="sxs-lookup"><span data-stu-id="c0450-584">'Update-AzVirtualWan'</span></span>
* <span data-ttu-id="c0450-585">Foram adicionados cmdlets para suportar o grupo de zonas DNS para pontos finais privados</span><span class="sxs-lookup"><span data-stu-id="c0450-585">Added new cmdlets to support DNS zone group for private endpoint</span></span>
    - <span data-ttu-id="c0450-586">"New-AzPrivateDnsZoneConfig"</span><span class="sxs-lookup"><span data-stu-id="c0450-586">'New-AzPrivateDnsZoneConfig'</span></span>
    - <span data-ttu-id="c0450-587">"Get-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="c0450-587">'Get-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="c0450-588">"New-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="c0450-588">'New-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="c0450-589">"Set-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="c0450-589">'Set-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="c0450-590">"Remove-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="c0450-590">'Remove-AzPrivateDnsZoneGroup'</span></span>
* <span data-ttu-id="c0450-591">Foram adicionados os parâmetros "DNSEnableProxy", "DNSRequireProxyForNetworkRules" e "DNSServers" a "AzureFirewall"</span><span class="sxs-lookup"><span data-stu-id="c0450-591">Added 'DNSEnableProxy', 'DNSRequireProxyForNetworkRules' and 'DNSServers' parameters to 'AzureFirewall'</span></span>
* <span data-ttu-id="c0450-592">Foram adicionados os parâmetros "EnableDnsProxy", "DnsProxyNotRequiredForNetworkRule" e "DnsServer" a "AzureFirewall"</span><span class="sxs-lookup"><span data-stu-id="c0450-592">Added 'EnableDnsProxy', 'DnsProxyNotRequiredForNetworkRule' and 'DnsServer' parameters to 'AzureFirewall'</span></span>
    - <span data-ttu-id="c0450-593">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="c0450-593">Updated cmdlet:</span></span>
        - <span data-ttu-id="c0450-594">New-AzFirewall</span><span class="sxs-lookup"><span data-stu-id="c0450-594">New-AzFirewall</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c0450-595">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-595">Az.OperationalInsights</span></span>
* <span data-ttu-id="c0450-596">O código legado foi atualizado para aplicar o SDK recém-gerado</span><span class="sxs-lookup"><span data-stu-id="c0450-596">Updated legacy code to apply new generated SDK</span></span>
* <span data-ttu-id="c0450-597">Foram eliminados cmdlets devido a APIs preteridas</span><span class="sxs-lookup"><span data-stu-id="c0450-597">Deleted cmdlets due to deprecated APIs</span></span>
    - <span data-ttu-id="c0450-598">"Get-AzOperationalInsightsSavedSearchResult" (alias "Get-AzOperationalInsightsSavedSearchResults")</span><span class="sxs-lookup"><span data-stu-id="c0450-598">'Get-AzOperationalInsightsSavedSearchResult' (alias 'Get-AzOperationalInsightsSavedSearchResults')</span></span>
    - <span data-ttu-id="c0450-599">"Get-AzOperationalInsightsSearchResult" (alias "Get-AzOperationalInsightsSearchResults")</span><span class="sxs-lookup"><span data-stu-id="c0450-599">'Get-AzOperationalInsightsSearchResult' (alias 'Get-AzOperationalInsightsSearchResults')</span></span>
    - <span data-ttu-id="c0450-600">"Get-AzOperationalInsightsLinkTarget" (alias "Get-AzOperationalInsightsLinkTargets")</span><span class="sxs-lookup"><span data-stu-id="c0450-600">'Get-AzOperationalInsightsLinkTarget' (alias 'Get-AzOperationalInsightsLinkTargets')</span></span>
* <span data-ttu-id="c0450-601">Foram adicionados parâmetros para "Set-AzOperationalInsightsWorkspace" e "New-AzOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="c0450-601">Added parameters for 'Set-AzOperationalInsightsWorkspace' and 'New-AzOperationalInsightsWorkspace'</span></span>
* <span data-ttu-id="c0450-602">Foram criados cmdlets para a Conta de Armazenamento Associada</span><span class="sxs-lookup"><span data-stu-id="c0450-602">Created cmdlets for Linked Stoarge Account</span></span>
* <span data-ttu-id="c0450-603">Foram criados cmdlets para Clusters e para o Serviço Associado</span><span class="sxs-lookup"><span data-stu-id="c0450-603">Created cmdlets for Clusters and Linked Service</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-604">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-604">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-605">O Azure Site Recovery adicionou suporte para proteger máquinas virtuais de grupo de colocação por proximidade para fornecedor do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-605">Azure Site Recovery added support for protecting proximity placement group virtual machines for Azure to Azure provider.</span></span>
* <span data-ttu-id="c0450-606">O Azure Site Recovery adicionou suporte para a replicação de zona para zona.</span><span class="sxs-lookup"><span data-stu-id="c0450-606">Azure Site Recovery added support for zone to zone replication.</span></span>
* <span data-ttu-id="c0450-607">O Azure Backup adicionou suporte para a retenção de longo prazo para Pontos de Recuperação de Partilhas de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-607">Azure Backup Added Long term retention support for Azure FileShare Recovery Points.</span></span>
* <span data-ttu-id="c0450-608">O Azure Backup adicionou propriedades de exclusão de discos à saída do cmdlet "Get-AzRecoveryServicesBackupItem".</span><span class="sxs-lookup"><span data-stu-id="c0450-608">Azure Backup Added disk exclusion properties to 'Get-AzRecoveryServicesBackupItem' cmdlet output.</span></span>
* <span data-ttu-id="c0450-609">Foi adicionado o ponto final privado para o ficheiro de credenciais de Cofre para o Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="c0450-609">Added private endpoint for Vault credential file for site recovery service.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-610">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-610">Az.Resources</span></span>
* <span data-ttu-id="c0450-611">Foi adicionado um aviso de mensagem relativo a um atraso na vista ao criar uma Definição de Função nova</span><span class="sxs-lookup"><span data-stu-id="c0450-611">Added message warning about view delay when creating a new Role Definition</span></span>
* <span data-ttu-id="c0450-612">Os cmdlets de política foram alterados para produzir objetos de tipos compatíveis</span><span class="sxs-lookup"><span data-stu-id="c0450-612">Changed policy cmdlets to output strongly-typed objects</span></span>
* <span data-ttu-id="c0450-613">Foi removido o parâmetro "-TenantLevel" utilizado no cmdlet "Get-AzResourceLock" [#11335]</span><span class="sxs-lookup"><span data-stu-id="c0450-613">Removed '-TenantLevel' parameter used for on the 'Get-AzResourceLock' cmdlet [#11335]</span></span>
* <span data-ttu-id="c0450-614">"Remove-AzResourceGroup -Id ResourceId" foi corrigido [#9882]</span><span class="sxs-lookup"><span data-stu-id="c0450-614">Fixed 'Remove-AzResourceGroup -Id ResourceId'[#9882]</span></span>
* <span data-ttu-id="c0450-615">Foi adicionado um cmdlet novo para obter resultados de What-If de modelos do ARM no âmbito de um grupo de recursos: "Get-AzDeploymentResourceGroupWhatIfResult"</span><span class="sxs-lookup"><span data-stu-id="c0450-615">Added new cmdlet for getting ARM template What-If results at resource group scope: 'Get-AzDeploymentResourceGroupWhatIfResult'</span></span>
* <span data-ttu-id="c0450-616">Foi adicionado um cmdlet novo para obter resultados de What-If de modelos do ARM no âmbito de uma subscrição: "Get-AzDeploymentWhatIfResult"</span><span class="sxs-lookup"><span data-stu-id="c0450-616">Added new cmdlet for getting ARM template What-If results at subscription scope: 'Get-AzDeploymentWhatIfResult'</span></span>
   - <span data-ttu-id="c0450-617">Alias: "Get-AzSubscriptionDeploymentWhatIf"</span><span class="sxs-lookup"><span data-stu-id="c0450-617">Alias: 'Get-AzSubscriptionDeploymentWhatIf'</span></span>
* <span data-ttu-id="c0450-618">Os parâmetros "-WhatIf" e "-Confirm" foram substituídos para "New-AzDeployment" e "New-AzResourceGroupDeployment" para utilizar resultados de What-If de modelos do ARM</span><span class="sxs-lookup"><span data-stu-id="c0450-618">Overrode '-WhatIf' and '-Confirm' parameters for 'New-AzDeployment' and 'New-AzResourceGroupDeployment' to use ARM template What-If results</span></span>
* <span data-ttu-id="c0450-619">Foi adicionada a mensagem de descontinuação para o parâmetro "ApiVersion" em cmdlets implementados</span><span class="sxs-lookup"><span data-stu-id="c0450-619">Added deprecation message for 'ApiVersion' parameter in deployment cmdlets</span></span>
* <span data-ttu-id="c0450-620">Foi adicionada a capacidade para mostrar mensagens de erro melhoradas relativas a falhas em implementações</span><span class="sxs-lookup"><span data-stu-id="c0450-620">Added capability to show improved error messages for deployment failures</span></span>
* <span data-ttu-id="c0450-621">Foi adicionado o registo de correlationId para falhas em implementações</span><span class="sxs-lookup"><span data-stu-id="c0450-621">Added correlationId logging for deployment failures</span></span>
* <span data-ttu-id="c0450-622">Foi adicionada a propriedade "error" à saída do script de implementação</span><span class="sxs-lookup"><span data-stu-id="c0450-622">Added 'error' property to the deployment script output</span></span>
* <span data-ttu-id="c0450-623">O nuget Microsoft.Azure.Management.ResourceManager foi atualizado para "3.7.1-preview"</span><span class="sxs-lookup"><span data-stu-id="c0450-623">Updated nuget Microsoft.Azure.Management.ResourceManager to '3.7.1-preview'</span></span>
* <span data-ttu-id="c0450-624">Foram removidos casos de teste específicos, uma vez que a propriedade Error em DeploymentValidateResult foi alterada para apenas de leitura a partir de 3.7.1-preview</span><span class="sxs-lookup"><span data-stu-id="c0450-624">Removed specific test cases as Error property in DeploymentValidateResult has changed to readonly from nuget 3.7.1-preview</span></span>
* <span data-ttu-id="c0450-625">GenericResourceExpanded foi importado do SDK ResourceManager 3.7.1-preview</span><span class="sxs-lookup"><span data-stu-id="c0450-625">Brought GenericResourceExpanded from SDK ResourceManager 3.7.1-preview</span></span>
* <span data-ttu-id="c0450-626">Foi adicionado suporte para etiquetas a todos os cmdlets Get para implementação, bem como</span><span class="sxs-lookup"><span data-stu-id="c0450-626">Added tag support for all Get cmdlets for deployment, as well as</span></span>
    - <span data-ttu-id="c0450-627">"New-AzDeployment"</span><span class="sxs-lookup"><span data-stu-id="c0450-627">'New-AzDeployment'</span></span>
    - <span data-ttu-id="c0450-628">"New-AzManagementGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="c0450-628">'New-AzManagementGroupDeployment'</span></span>
    - <span data-ttu-id="c0450-629">"New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="c0450-629">'New-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="c0450-630">"New-AzTenantDeployment"</span><span class="sxs-lookup"><span data-stu-id="c0450-630">'New-AzTenantDeployment'</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c0450-631">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c0450-631">Az.ServiceFabric</span></span>
* <span data-ttu-id="c0450-632">Foi corrigido um erro na adição de certificados mediante a utilização de --SecretIdentifier que obtinha o thumbprint de certificado incorreto</span><span class="sxs-lookup"><span data-stu-id="c0450-632">Fixed bug in add certificate using --SecretIdentifier that was getting the wrong certificate thumbprint</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-633">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-633">Az.Sql</span></span>
* <span data-ttu-id="c0450-634">Foi melhorado o desempenho de:</span><span class="sxs-lookup"><span data-stu-id="c0450-634">Enhance performance of:</span></span>
    - <span data-ttu-id="c0450-635">"Set-AzSqlDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="c0450-635">'Set-AzSqlDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="c0450-636">"Set-AzSqlInstanceDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="c0450-636">'Set-AzSqlInstanceDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="c0450-637">"Remove-AzSqlDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="c0450-637">'Remove-AzSqlDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="c0450-638">"Remove-AzSqlInstanceDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="c0450-638">'Remove-AzSqlInstanceDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="c0450-639">"Enable-AzSqlDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="c0450-639">'Enable-AzSqlDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="c0450-640">"Enable-AzSqlInstanceDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="c0450-640">'Enable-AzSqlInstanceDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="c0450-641">"Disable-AzSqlDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="c0450-641">'Disable-AzSqlDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="c0450-642">"Disable-AzSqlInstanceDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="c0450-642">'Disable-AzSqlInstanceDatabaseSensitivityRecommendation'</span></span>
* <span data-ttu-id="c0450-643">Foi removida a validação do lado do cliente do parâmetro "RetentionDays" do cmdlet "Set-AzSqlDatabaseBackupShortTermRetentionPolicy"</span><span class="sxs-lookup"><span data-stu-id="c0450-643">Removed client-side validation of 'RetentionDays' parameter from cmdlet 'Set-AzSqlDatabaseBackupShortTermRetentionPolicy'</span></span>
* <span data-ttu-id="c0450-644">Auditoria a uma conta de armazenamento na Vnet; corrigido um erro ao criar uma função de Contribuidor de Dados de Blobs de Armazenamento.</span><span class="sxs-lookup"><span data-stu-id="c0450-644">Auditing to a storage account in Vnet, fixing a bug when creating a Storage Blob Data Contributor role.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-645">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-645">Az.Storage</span></span>
* <span data-ttu-id="c0450-646">Foi adicionado "-AsJob" ao cmdlet para obter/listar contas "Get-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c0450-646">Added '-AsJob' to get/list account cmdlet 'Get-AzStorageAccount'</span></span>
* <span data-ttu-id="c0450-647">KeyVersion foi tornado opcional ao atualizar a conta de Armazenamento com KeyvaultEncryption, para suportar a rotação automática de chaves</span><span class="sxs-lookup"><span data-stu-id="c0450-647">Make KeyVersion to optional when update Storage account with KeyvaultEncryption, to support key auto-rotation</span></span>
    - <span data-ttu-id="c0450-648">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c0450-648">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="c0450-649">Corrigida a remoção de falha do Diretório de Ficheiros do Azure com o pipeline</span><span class="sxs-lookup"><span data-stu-id="c0450-649">Fixed remove Azure File Directory fail with pipeline</span></span>
    - <span data-ttu-id="c0450-650">"Remove-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="c0450-650">'Remove-AzStorageDirectory'</span></span>
* <span data-ttu-id="c0450-651">Corrigido [#9880]: A definição do valor DefaultAction de NetWorkRule foi alterado para estar alinhado com o swagger.</span><span class="sxs-lookup"><span data-stu-id="c0450-651">Fixed [#9880]: Change NetWorkRule DefaultAction value defination to align with swagger.</span></span>
    - <span data-ttu-id="c0450-652">"Update-AzStorageAccountNetworkRuleSet"</span><span class="sxs-lookup"><span data-stu-id="c0450-652">'Update-AzStorageAccountNetworkRuleSet'</span></span>
    - <span data-ttu-id="c0450-653">"Get-AzStorageAccountNetworkRuleSet"</span><span class="sxs-lookup"><span data-stu-id="c0450-653">'Get-AzStorageAccountNetworkRuleSet'</span></span>
* <span data-ttu-id="c0450-654">Corrigido [#11624]: Ignorar regras duplicadas ao adicionar NetworkRules, para evitar falhas de servidores</span><span class="sxs-lookup"><span data-stu-id="c0450-654">Fixed [#11624]: Skip duplicated rules when add NetworkRules, to avoid server failure</span></span>
    - <span data-ttu-id="c0450-655">"Add-AzStorageAccountNetworkRule"</span><span class="sxs-lookup"><span data-stu-id="c0450-655">'Add-AzStorageAccountNetworkRule'</span></span>
* <span data-ttu-id="c0450-656">O SDK Microsoft.Azure.Cosmos.Table foi atualizado para 1.0.7</span><span class="sxs-lookup"><span data-stu-id="c0450-656">Upgraded Microsoft.Azure.Cosmos.Table SDK to 1.0.7</span></span>
* <span data-ttu-id="c0450-657">Foi adicionada uma mensagem de aviso para relembrar o utilizador para listar novamente com ContinuationToken apenas quando são devolvidos itens de peças na lista DataLake Gen2 Items,</span><span class="sxs-lookup"><span data-stu-id="c0450-657">Added a warning message to remind user to list again with ContinuationToken when only part items are returned in list DataLake Gen2 Items,</span></span>
    - <span data-ttu-id="c0450-658">"Get-AzDataLakeGen2ChildItem"</span><span class="sxs-lookup"><span data-stu-id="c0450-658">'Get-AzDataLakeGen2ChildItem'</span></span>
* <span data-ttu-id="c0450-659">Suportado para criar ou atualizar a conta de Armazenamento com a Autenticação do Active Directory Domain Service dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="c0450-659">Supported to create or update Storage account with Azure Files Active Directory Domain Service Authentication</span></span>
    -  <span data-ttu-id="c0450-660">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c0450-660">'New-AzStorageAccount'</span></span>
    -  <span data-ttu-id="c0450-661">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c0450-661">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="c0450-662">Suportado para os comandos "new" ou "list" de chaves de Kerberos da conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="c0450-662">Supported to new or list Kerberos keys of Storage account</span></span>
    -  <span data-ttu-id="c0450-663">"New-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="c0450-663">'New-AzStorageAccountKey'</span></span>
    -  <span data-ttu-id="c0450-664">"Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="c0450-664">'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="c0450-665">Suportada conta de Armazenamento de ativação pós-falha</span><span class="sxs-lookup"><span data-stu-id="c0450-665">Supported failover Storage account</span></span>
    - <span data-ttu-id="c0450-666">"Invoke-AzStorageAccountFailover"</span><span class="sxs-lookup"><span data-stu-id="c0450-666">'Invoke-AzStorageAccountFailover'</span></span>
* <span data-ttu-id="c0450-667">Ajuda de "Get-AzStorageBlobCopyState" atualizada</span><span class="sxs-lookup"><span data-stu-id="c0450-667">Updated help of 'Get-AzStorageBlobCopyState'</span></span>
* <span data-ttu-id="c0450-668">Ajuda de "Get-AzStorageFileCopyState" e "Start-AzStorageBlobCopy" atualizada</span><span class="sxs-lookup"><span data-stu-id="c0450-668">Updated help of 'Get-AzStorageFileCopyState' and 'Start-AzStorageBlobCopy'</span></span>
* <span data-ttu-id="c0450-669">Integração da biblioteca de cliente do Armazenamento v12 para cmdlets de Filas e Ficheiros</span><span class="sxs-lookup"><span data-stu-id="c0450-669">Integrated Storage client library v12 to Queue and File cmdlets</span></span>
* <span data-ttu-id="c0450-670">Alteração ao tipo de saída de CloudFile para AzureStorageFile; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="c0450-670">Changed output type from CloudFile to AzureStorageFile, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="c0450-671">"Get-AzStorageFile"</span><span class="sxs-lookup"><span data-stu-id="c0450-671">'Get-AzStorageFile'</span></span>
    - <span data-ttu-id="c0450-672">"Remove-AzStorageFile"</span><span class="sxs-lookup"><span data-stu-id="c0450-672">'Remove-AzStorageFile'</span></span>
    - <span data-ttu-id="c0450-673">"Get-AzStorageFileContent"</span><span class="sxs-lookup"><span data-stu-id="c0450-673">'Get-AzStorageFileContent'</span></span>
    - <span data-ttu-id="c0450-674">"Set-AzStorageFileContent"</span><span class="sxs-lookup"><span data-stu-id="c0450-674">'Set-AzStorageFileContent'</span></span>
    - <span data-ttu-id="c0450-675">"Start-AzStorageFileCopy"</span><span class="sxs-lookup"><span data-stu-id="c0450-675">'Start-AzStorageFileCopy'</span></span>
* <span data-ttu-id="c0450-676">Alteração ao tipo de saída de CloudFileDirectory para AzureStorageFileDirectory; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="c0450-676">Changed output type from CloudFileDirectory to AzureStorageFileDirectory, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="c0450-677">"New-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="c0450-677">'New-AzStorageDirectory'</span></span>
    - <span data-ttu-id="c0450-678">"Remove-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="c0450-678">'Remove-AzStorageDirectory'</span></span>
* <span data-ttu-id="c0450-679">Alteração ao tipo de saída de CloudFileShare para AzureStorageFileShare; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="c0450-679">Changed output type from CloudFileShare to AzureStorageFileShare, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="c0450-680">"Get-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="c0450-680">'Get-AzStorageShare'</span></span>
    - <span data-ttu-id="c0450-681">"New-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="c0450-681">'New-AzStorageShare'</span></span>
    - <span data-ttu-id="c0450-682">"Remove-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="c0450-682">'Remove-AzStorageShare'</span></span>
* <span data-ttu-id="c0450-683">Alteração ao tipo de saída de FileShareProperties para AzureStorageFileShare; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="c0450-683">Changed output type from FileShareProperties to AzureStorageFileShare, the original output will become a sub child property of the new output</span></span>
    - <span data-ttu-id="c0450-684">"Set-AzStorageShareQuota"</span><span class="sxs-lookup"><span data-stu-id="c0450-684">'Set-AzStorageShareQuota'</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="c0450-685">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c0450-685">Az.TrafficManager</span></span>
* <span data-ttu-id="c0450-686">Corrigido o nome de perfil errado na saída verbosa de "DisableAzureTrafficManagerEndpoint"</span><span class="sxs-lookup"><span data-stu-id="c0450-686">Fixed incorrect profile name in 'DisableAzureTrafficManagerEndpoint' verbose output</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c0450-687">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-687">Az.Websites</span></span>
* <span data-ttu-id="c0450-688">Corrigido um erro ortográfico na ajuda de "Update-AzWebAppAccessRestrictionConfig".</span><span class="sxs-lookup"><span data-stu-id="c0450-688">Fixed typo on help of 'Update-AzWebAppAccessRestrictionConfig'.</span></span>

## <a name="380---april-2020"></a><span data-ttu-id="c0450-689">3.8.0 - Abril de 2020</span><span class="sxs-lookup"><span data-stu-id="c0450-689">3.8.0 - April 2020</span></span>
### <a name="highlights-since-the-last-release"></a><span data-ttu-id="c0450-690">Destaques desde a última versão</span><span class="sxs-lookup"><span data-stu-id="c0450-690">Highlights since the last release</span></span>
* <span data-ttu-id="c0450-691">Versões do Powershell suportadas pelo Az.Storage: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span><span class="sxs-lookup"><span data-stu-id="c0450-691">PowerShell versions that Az.Storage supports: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c0450-692">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-692">Az.Accounts</span></span>
* <span data-ttu-id="c0450-693">Atualização do URL de inquérito do Azure PowerShell em "Resolve-AzError" [#11507]</span><span class="sxs-lookup"><span data-stu-id="c0450-693">Updated Azure PowerShell survey URL in 'Resolve-AzError' [#11507]</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c0450-694">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c0450-694">Az.ApiManagement</span></span>
* <span data-ttu-id="c0450-695">Adicionado aviso de alteração interruptiva para a alteração de resultados de cmdlets de Ficheiro do Azure numa versão futura</span><span class="sxs-lookup"><span data-stu-id="c0450-695">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="c0450-696">Documentação atualizada de "Set-AzApiManagementGroup" para especificar o parâmetro GroupId</span><span class="sxs-lookup"><span data-stu-id="c0450-696">'Set-AzApiManagementGroup' Updated documentation to specify the GroupId parameter</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c0450-697">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c0450-697">Az.Cdn</span></span>
* <span data-ttu-id="c0450-698">Correção da apresentação do SKU de preços relacionados com ChinaCDN</span><span class="sxs-lookup"><span data-stu-id="c0450-698">Fixed ChinaCDN related pricing SKU display</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c0450-699">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c0450-699">Az.CognitiveServices</span></span>
* <span data-ttu-id="c0450-700">Suporte para Identidade, Encriptação, UserOwnedStorage</span><span class="sxs-lookup"><span data-stu-id="c0450-700">Supported Identity, Encryption, UserOwnedStorage</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-701">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-701">Az.Compute</span></span>
* <span data-ttu-id="c0450-702">Adicionado o cmdlet "Set-AzVmssOrchestrationServiceState".</span><span class="sxs-lookup"><span data-stu-id="c0450-702">Added 'Set-AzVmssOrchestrationServiceState' cmdlet.</span></span>
* <span data-ttu-id="c0450-703">"Get-AzVmss" com -InstanceView mostra os estados de OrchestrationService.</span><span class="sxs-lookup"><span data-stu-id="c0450-703">'Get-AzVmss' with -InstanceView shows OrchestrationService states.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c0450-704">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c0450-704">Az.IotHub</span></span>
* <span data-ttu-id="c0450-705">Gestão da configuração do dispositivo duplo de IoT. Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="c0450-705">Manage IoT device twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="c0450-706">"Get-AzIotHubDeviceTwin"</span><span class="sxs-lookup"><span data-stu-id="c0450-706">'Get-AzIotHubDeviceTwin'</span></span>
    - <span data-ttu-id="c0450-707">"Update-AzIotHubDeviceTwin"</span><span class="sxs-lookup"><span data-stu-id="c0450-707">'Update-AzIotHubDeviceTwin'</span></span>
* <span data-ttu-id="c0450-708">Adicionado cmdlet para invocar o método direto num dispositivo num hub IoT.</span><span class="sxs-lookup"><span data-stu-id="c0450-708">Added cmdlet to invoke direct method on a device in an Iot Hub.</span></span>
* <span data-ttu-id="c0450-709">Gestão da configuração do módulo duplo do dispositivo de IoT. Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="c0450-709">Manage IoT device module twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="c0450-710">"Get-AzIotHubModuleTwin"</span><span class="sxs-lookup"><span data-stu-id="c0450-710">'Get-AzIotHubModuleTwin'</span></span>
    - <span data-ttu-id="c0450-711">"Update-AzIotHubModuleTwin"</span><span class="sxs-lookup"><span data-stu-id="c0450-711">'Update-AzIotHubModuleTwin'</span></span>
* <span data-ttu-id="c0450-712">Gestão da configuração da gestão automática de dispositivos IoT em escala.</span><span class="sxs-lookup"><span data-stu-id="c0450-712">Manage IoT automatic device management configuration at scale.</span></span> <span data-ttu-id="c0450-713">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="c0450-713">New cmdlets are:</span></span>
    - <span data-ttu-id="c0450-714">"Add-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c0450-714">'Add-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="c0450-715">"Get-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c0450-715">'Get-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="c0450-716">"Remove-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c0450-716">'Remove-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="c0450-717">"Set-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c0450-717">'Set-AzIotHubConfiguration'</span></span>
* <span data-ttu-id="c0450-718">Adicionado cmdlet para invocar um método de módulo de periferia num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="c0450-718">Added cmdlet to invoke an edge module method in an Iot Hub.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c0450-719">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0450-719">Az.KeyVault</span></span>
* <span data-ttu-id="c0450-720">Adicionado um novo cmdlet "Update-AzKeyVault" que pode permitir a eliminação recuperável e a proteção contra remoções num cofre</span><span class="sxs-lookup"><span data-stu-id="c0450-720">Added a new cmdlet 'Update-AzKeyVault' that can enable soft delete and purge protection on a vault</span></span>
* <span data-ttu-id="c0450-721">Adicionado suporte para Microsoft.PowerShell.SecretManagement [#11178]</span><span class="sxs-lookup"><span data-stu-id="c0450-721">Added support to Microsoft.PowerShell.SecretManagement [#11178]</span></span>
* <span data-ttu-id="c0450-722">Correção do erro nos exemplos de "Remove-AzKeyVaultManagedStorageSasDefinition" [#11479]</span><span class="sxs-lookup"><span data-stu-id="c0450-722">Fixed error in the examples of 'Remove-AzKeyVaultManagedStorageSasDefinition' [#11479]</span></span>
* <span data-ttu-id="c0450-723">Adicionado suporte para o ponto final privado</span><span class="sxs-lookup"><span data-stu-id="c0450-723">Added support to private endpoint</span></span>

#### <a name="azmaintenance"></a><span data-ttu-id="c0450-724">Az.Maintenance</span><span class="sxs-lookup"><span data-stu-id="c0450-724">Az.Maintenance</span></span>
* <span data-ttu-id="c0450-725">Publicação da versão de lançamento dos cmdlets de Manutenção para Disponibilidade Geral</span><span class="sxs-lookup"><span data-stu-id="c0450-725">Publishing release version of Maintenance cmdlets for GA</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c0450-726">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c0450-726">Az.Monitor</span></span>
* <span data-ttu-id="c0450-727">Adicionados cmdlets para o âmbito de ligação privada</span><span class="sxs-lookup"><span data-stu-id="c0450-727">Added cmdlets for private link scope</span></span>
    - <span data-ttu-id="c0450-728">"Get-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="c0450-728">'Get-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="c0450-729">"Remove-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="c0450-729">'Remove-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="c0450-730">"New-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="c0450-730">'New-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="c0450-731">"Update-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="c0450-731">'Update-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="c0450-732">"Get-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="c0450-732">'Get-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="c0450-733">"New-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="c0450-733">'New-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="c0450-734">"Remove-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="c0450-734">'Remove-AzInsightsPrivateLinkScopedResource'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-735">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-735">Az.Network</span></span>
* <span data-ttu-id="c0450-736">Atualização dos cmdlets para permitir a ligação num IP privado para o Gateway de Rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="c0450-736">Updated cmdlets to enable connection on private IP for Virtual Network Gateway.</span></span>
    - <span data-ttu-id="c0450-737">"New-AzVirtualNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="c0450-737">'New-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="c0450-738">"Set-AzVirtualNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="c0450-738">'Set-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="c0450-739">"New-AzVirtualNetworkGatewayConnection"</span><span class="sxs-lookup"><span data-stu-id="c0450-739">'New-AzVirtualNetworkGatewayConnection'</span></span>
    - <span data-ttu-id="c0450-740">"Set-AzVirtualNetworkGatewayConnection"</span><span class="sxs-lookup"><span data-stu-id="c0450-740">'Set-AzVirtualNetworkGatewayConnection'</span></span>
* <span data-ttu-id="c0450-741">Atualização dos cmdlets para permitir LocalNetworkGateways e VpnSites com base em FQDN</span><span class="sxs-lookup"><span data-stu-id="c0450-741">Updated cmdlets to enable FQDN based LocalNetworkGateways and VpnSites</span></span>
    - <span data-ttu-id="c0450-742">"New-AzLocalNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="c0450-742">'New-AzLocalNetworkGateway'</span></span>
    - <span data-ttu-id="c0450-743">"New-AzVpnSiteLink"</span><span class="sxs-lookup"><span data-stu-id="c0450-743">'New-AzVpnSiteLink'</span></span>
* <span data-ttu-id="c0450-744">Adicionado suporte para a família de endereços IPv6 em ExpressRouteCircuitConnectionConfig (Alcance Global)</span><span class="sxs-lookup"><span data-stu-id="c0450-744">Added support for IPv6 address family in ExpressRouteCircuitConnectionConfig (Global Reach)</span></span>
    - <span data-ttu-id="c0450-745">Adicionado "Set-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="c0450-745">Added 'Set-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="c0450-746">permite a definição de todas as propriedades existentes, incluindo o IPv6CircuitConnectionProperties</span><span class="sxs-lookup"><span data-stu-id="c0450-746">allows setting of all the existing properties including the IPv6CircuitConnectionProperties</span></span>
    - <span data-ttu-id="c0450-747">Atualização de "Add-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="c0450-747">Updated 'Add-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="c0450-748">Adicionado outro parâmetro opcional AddressPrefixType para especificar a família de endereços do prefixo de endereço</span><span class="sxs-lookup"><span data-stu-id="c0450-748">Added another optional parameter AddressPrefixType to specify the address family of address prefix</span></span>
* <span data-ttu-id="c0450-749">Atualização dos cmdlets para permitir a definição do Tempo Limite de DPD nas Ligações do Gateway de Rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="c0450-749">Updated cmdlets to enable setting of DPD Timeout on Virtual Network Gateway Connections.</span></span>
    - <span data-ttu-id="c0450-750">New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-750">New-AzVirtualNetworkGatewayConnection</span></span>
    - <span data-ttu-id="c0450-751">Set-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-751">Set-AzVirtualNetworkGatewayConnection</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c0450-752">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-752">Az.PolicyInsights</span></span>
* <span data-ttu-id="c0450-753">Adicionado o cmdlet "Start-AzPolicyComplianceScan" para acionar análises de conformidade de políticas</span><span class="sxs-lookup"><span data-stu-id="c0450-753">Added 'Start-AzPolicyComplianceScan' cmdlet for triggering policy compliance scans</span></span>
* <span data-ttu-id="c0450-754">Adição de definição de políticas, definição de conjuntos e versões de atribuição ao resultado de "Get-AzPolicyState"</span><span class="sxs-lookup"><span data-stu-id="c0450-754">Added policy definition, set definition, and assignment versions to 'Get-AzPolicyState' output</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c0450-755">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c0450-755">Az.ServiceFabric</span></span>
* <span data-ttu-id="c0450-756">Melhorias da formatação e usabilidade do código dos exemplos de "New-AzServiceFabricCluster"</span><span class="sxs-lookup"><span data-stu-id="c0450-756">Improved code formatting and usability of 'New-AzServiceFabricCluster' examples</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-757">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-757">Az.Sql</span></span>
* <span data-ttu-id="c0450-758">Adicionados os cmdlets "Get-AzSqlInstanceOperation" e "Stop-AzSqlInstanceOperation"</span><span class="sxs-lookup"><span data-stu-id="c0450-758">Added cmdlets 'Get-AzSqlInstanceOperation' and 'Stop-AzSqlInstanceOperation'</span></span>
* <span data-ttu-id="c0450-759">Suporte de auditorias a uma conta de armazenamento numa VNet.</span><span class="sxs-lookup"><span data-stu-id="c0450-759">Supported auditing to a storage account in VNet.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-760">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-760">Az.Storage</span></span>
* <span data-ttu-id="c0450-761">Adicionado aviso de alteração interruptiva para a alteração de resultados de cmdlets de Ficheiro do Azure numa versão futura</span><span class="sxs-lookup"><span data-stu-id="c0450-761">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="c0450-762">Suportado novo SkuName StandardGZRS, StandardRAGZRS ao criar/atualizar a Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="c0450-762">Supported new SkuName StandardGZRS, StandardRAGZRS when create/update Storage account</span></span>
    - <span data-ttu-id="c0450-763">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c0450-763">'New-AzStorageAccount'</span></span>
    - <span data-ttu-id="c0450-764">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c0450-764">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="c0450-765">Suportado o DataLake Gen2</span><span class="sxs-lookup"><span data-stu-id="c0450-765">Supported DataLake Gen2</span></span>
    - <span data-ttu-id="c0450-766">"New-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="c0450-766">'New-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="c0450-767">"Get-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="c0450-767">'Get-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="c0450-768">"Get-AzDataLakeGen2ChildItem"</span><span class="sxs-lookup"><span data-stu-id="c0450-768">'Get-AzDataLakeGen2ChildItem'</span></span>
    - <span data-ttu-id="c0450-769">"Move-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="c0450-769">'Move-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="c0450-770">"Set-AzDataLakeGen2ItemAclObject"</span><span class="sxs-lookup"><span data-stu-id="c0450-770">'Set-AzDataLakeGen2ItemAclObject'</span></span>
    - <span data-ttu-id="c0450-771">"Update-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="c0450-771">'Update-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="c0450-772">"Get-AzDataLakeGen2ItemContent"</span><span class="sxs-lookup"><span data-stu-id="c0450-772">'Get-AzDataLakeGen2ItemContent'</span></span>
    - <span data-ttu-id="c0450-773">"Remove-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="c0450-773">'Remove-AzDataLakeGen2Item'</span></span>

## <a name="0100-preview---april-2020"></a><span data-ttu-id="c0450-774">0.10.0-preview - Abril de 2020</span><span class="sxs-lookup"><span data-stu-id="c0450-774">0.10.0-preview - April 2020</span></span>
### <a name="general"></a><span data-ttu-id="c0450-775">Geral</span><span class="sxs-lookup"><span data-stu-id="c0450-775">General</span></span>
* <span data-ttu-id="c0450-776">Os módulos Az já estão disponíveis em pré-visualização no Azure Stack Hub.</span><span class="sxs-lookup"><span data-stu-id="c0450-776">Az modules is now available in preview on Azure Stack Hub.</span></span> <span data-ttu-id="c0450-777">Isto permite a compatibilidade entre plataformas diferentes com o Linux e macOS.</span><span class="sxs-lookup"><span data-stu-id="c0450-777">This allows for cross-platform compatibility with Linux and macOs.</span></span> <span data-ttu-id="c0450-778">Agora, o Azure Stack Hub suporta o PowerShell Core com os módulos Az. Obtenha mais informações [aqui](https://aka.ms/az4AzureStack)</span><span class="sxs-lookup"><span data-stu-id="c0450-778">Azure Stack Hub now supports PowerShell core with the Az modules, more information [here](https://aka.ms/az4AzureStack)</span></span>
* <span data-ttu-id="c0450-779">Os módulos Az suportam o perfil 2019-03-01-hybrid:</span><span class="sxs-lookup"><span data-stu-id="c0450-779">Az modules support profile 2019-03-01-hybrid:</span></span>
  - <span data-ttu-id="c0450-780">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="c0450-780">Az.Billing</span></span>
  - <span data-ttu-id="c0450-781">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-781">Az.Compute</span></span>
  - <span data-ttu-id="c0450-782">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="c0450-782">Az.DataBoxEdge</span></span>
  - <span data-ttu-id="c0450-783">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c0450-783">Az.EventHub</span></span>
  - <span data-ttu-id="c0450-784">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c0450-784">Az.IotHub</span></span>
  - <span data-ttu-id="c0450-785">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0450-785">Az.KeyVault</span></span>
  - <span data-ttu-id="c0450-786">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c0450-786">Az.Monitor</span></span>
  - <span data-ttu-id="c0450-787">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-787">Az.Network</span></span>
  - <span data-ttu-id="c0450-788">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-788">Az.Resources</span></span>
  - <span data-ttu-id="c0450-789">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-789">Az.Storage</span></span>
  - <span data-ttu-id="c0450-790">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-790">Az.Websites</span></span>
* <span data-ttu-id="c0450-791">Foram introduzidos três novos módulos do PowerShell para Az que funcionam com o Azure Stack Hub. São eles o Az.Databox, Az.IotHub e Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c0450-791">Three new PowerShell modules for az have been introduced that work with Azure Stack Hub, which are Az.Databox, Az.IotHub, and Az.EventHub</span></span>
* <span data-ttu-id="c0450-792">Os comandos permanecem sensivelmente iguais, com pequenas alterações como, por exemplo, a alteração do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="c0450-792">Commands remain relatively the same, with minor changes such as changing AzureRM to Az</span></span>
* <span data-ttu-id="c0450-793">Veja uma ligação atualizada à documentação do PowerShell para o Azure Stack Hub [aqui](https://aka.ms/InstallASHPowerShell)</span><span class="sxs-lookup"><span data-stu-id="c0450-793">Updated link to PowerShell documentation for Azure Stack Hub can be found [here](https://aka.ms/InstallASHPowerShell)</span></span>

## <a name="370---march-2020"></a><span data-ttu-id="c0450-794">3.7.0 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="c0450-794">3.7.0 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c0450-795">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-795">Az.Accounts</span></span>
* <span data-ttu-id="c0450-796">Foram corrigidos os parâmetros "Get-AzTenant"/"Get-AzDefault"/"Set-AzDefault" que emitiam uma NullReferenceException quando a sessão não estava iniciada [#10292]</span><span class="sxs-lookup"><span data-stu-id="c0450-796">Fixed 'Get-AzTenant'/'Get-AzDefault'/'Set-AzDefault' throw NullReferenceException when not login [#10292]</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-797">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-797">Az.Compute</span></span>
* <span data-ttu-id="c0450-798">Foram adicionados os seguintes parâmetros ao cmdlet "New-AzDiskConfig":</span><span class="sxs-lookup"><span data-stu-id="c0450-798">Added the following parameters to 'New-AzDiskConfig' cmdlet:</span></span>
    - <span data-ttu-id="c0450-799">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span><span class="sxs-lookup"><span data-stu-id="c0450-799">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span></span>
* <span data-ttu-id="c0450-800">A propriedade Encryption foi permitida para o parâmetro Target do cmdlet "New-AzGalleryImageVersion".</span><span class="sxs-lookup"><span data-stu-id="c0450-800">Allowed Encryption property to Target parameter of 'New-AzGalleryImageVersion' cmdlet.</span></span>
* <span data-ttu-id="c0450-801">Foi corrigido o problema de tempDisk para os cmdlets "Set-AzVmss" -Reimage e "Invoke-AzVMReimage".</span><span class="sxs-lookup"><span data-stu-id="c0450-801">Fixed tempDisk issue for 'Set-AzVmss' -Reimage and 'Invoke-AzVMReimage' cmdlets.</span></span> <span data-ttu-id="c0450-802">[#11354]</span><span class="sxs-lookup"><span data-stu-id="c0450-802">[#11354]</span></span>
* <span data-ttu-id="c0450-803">Foi adicionado suporte aos cmdlets abaixo para a nova Extensão SAP</span><span class="sxs-lookup"><span data-stu-id="c0450-803">Added support to below cmdlets for new SAP Extension</span></span>
    - <span data-ttu-id="c0450-804">"Set-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="c0450-804">'Set-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="c0450-805">"Get-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="c0450-805">'Get-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="c0450-806">"Remove-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="c0450-806">'Remove-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="c0450-807">"Update-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="c0450-807">'Update-AzVMAEMExtension'</span></span>
* <span data-ttu-id="c0450-808">Foram corrigidos os erros em exemplos do documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="c0450-808">Fixed errors in examples of help document</span></span>
* <span data-ttu-id="c0450-809">É apresentado o valor de cadeia exato para o PowerState da VM no formato de tabela.</span><span class="sxs-lookup"><span data-stu-id="c0450-809">Showed the exact string value for VM PowerState in the table format.</span></span>
* <span data-ttu-id="c0450-810">"New-AzVmssConfig": foi corrigida a serialização da propriedade AutomaticRepairs quando a opção SinglePlacementGroup está desativada.</span><span class="sxs-lookup"><span data-stu-id="c0450-810">'New-AzVmssConfig': fixed serialization of AutomaticRepairs property when SinglePlacementGroup is disabled.</span></span> <span data-ttu-id="c0450-811">[#11257]</span><span class="sxs-lookup"><span data-stu-id="c0450-811">[#11257]</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c0450-812">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c0450-812">Az.DataFactory</span></span>
* <span data-ttu-id="c0450-813">Atualização da versão do SDK .Net do ADF para 4.8.0</span><span class="sxs-lookup"><span data-stu-id="c0450-813">Updated ADF .Net SDK version to 4.8.0</span></span>
* <span data-ttu-id="c0450-814">Foram adicionados parâmetros opcionais ao comando "Invoke-AzDataFactoryV2Pipeline" para suportar uma nova execução</span><span class="sxs-lookup"><span data-stu-id="c0450-814">Added optional parameters to 'Invoke-AzDataFactoryV2Pipeline' command to support rerun</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c0450-815">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c0450-815">Az.DataLakeStore</span></span>
* <span data-ttu-id="c0450-816">Foi adicionada a descrição da alteração interruptiva para "Export-AzDataLakeStoreItem" e "Import-AzDataLakeStoreItem"</span><span class="sxs-lookup"><span data-stu-id="c0450-816">Added breaking change description for 'Export-AzDataLakeStoreItem' and 'Import-AzDataLakeStoreItem'</span></span>
* <span data-ttu-id="c0450-817">Foi adicionada a opção de codificação de bytes para "New-AzDataLakeStoreItem", "Add-AzDAtaLakeStoreItemContent" e "Get-AzDAtaLakeStoreItemContent"</span><span class="sxs-lookup"><span data-stu-id="c0450-817">Added option of Byte encoding for 'New-AzDataLakeStoreItem', 'Add-AzDAtaLakeStoreItemContent', and 'Get-AzDAtaLakeStoreItemContent'</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c0450-818">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c0450-818">Az.HDInsight</span></span>
* <span data-ttu-id="c0450-819">É suportada a versão de TLS mínima suportada ao criar o cluster.</span><span class="sxs-lookup"><span data-stu-id="c0450-819">Supported specifying minimal supported TLS version when creating cluster.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c0450-820">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c0450-820">Az.IotHub</span></span>
* <span data-ttu-id="c0450-821">Foi adicionado suporte para gerir as definições distribuídas por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0450-821">Added support to manage distributed settings per-device.</span></span> <span data-ttu-id="c0450-822">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="c0450-822">New Cmdlets are:</span></span>
    - <span data-ttu-id="c0450-823">"Get-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="c0450-823">'Get-AzIotHubDistributedTracing'</span></span>
    - <span data-ttu-id="c0450-824">"Set-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="c0450-824">'Set-AzIotHubDistributedTracing'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c0450-825">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0450-825">Az.KeyVault</span></span>
* <span data-ttu-id="c0450-826">Foram adicionados os atributos da alteração interruptiva a "New-AzKeyVault"</span><span class="sxs-lookup"><span data-stu-id="c0450-826">Added breaking change attributes to 'New-AzKeyVault'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c0450-827">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c0450-827">Az.Monitor</span></span>
* <span data-ttu-id="c0450-828">Foi atualizada a documentação de "New-AzScheduledQueryRuleLogMetricTrigger"</span><span class="sxs-lookup"><span data-stu-id="c0450-828">Updated documentation for 'New-AzScheduledQueryRuleLogMetricTrigger'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-829">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-829">Az.Network</span></span>
* <span data-ttu-id="c0450-830">Foram atualizados os cmdlets para permitir VirtualHubVnetConnections entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="c0450-830">Updated cmdlets to allow cross-tenant VirtualHubVnetConnections</span></span>
    - <span data-ttu-id="c0450-831">"New-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="c0450-831">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="c0450-832">"Update-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="c0450-832">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="c0450-833">"New-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="c0450-833">'New-AzVirtualHub'</span></span>
    - <span data-ttu-id="c0450-834">"Update-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="c0450-834">'Update-AzVirtualHub'</span></span>
* <span data-ttu-id="c0450-835">Foi removida a dependência do SDK do SQL Management</span><span class="sxs-lookup"><span data-stu-id="c0450-835">Removed Sql Management SDK dependency</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c0450-836">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-836">Az.PolicyInsights</span></span>
* <span data-ttu-id="c0450-837">Mensagens de erro melhoradas</span><span class="sxs-lookup"><span data-stu-id="c0450-837">Improved error messages</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-838">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-838">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-839">O Azure Site Recovery adicionou suporte para nova proteção e atualização das propriedades de VM para Máquinas Virtuais encriptadas em disco do Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-839">Azure Site Recovery added support for doing reprotect and updated vm properties for Azure disk encrypted Virtual Machines.</span></span>
* <span data-ttu-id="c0450-840">Foi adicionada monitorização DR das propriedades VmwareToAzure ao Azure Site Recovery</span><span class="sxs-lookup"><span data-stu-id="c0450-840">Added Azure Site Recovery VmwareToAzure properties DR monitoring</span></span>
* <span data-ttu-id="c0450-841">O Azure Backup adicionou suporte para repetir a atualização de políticas para itens falhados.</span><span class="sxs-lookup"><span data-stu-id="c0450-841">Azure Backup added support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="c0450-842">O Azure Backup adicionou suporte para definições de exclusão do disco durante a cópia de segurança e o restauro.</span><span class="sxs-lookup"><span data-stu-id="c0450-842">Azure Backup Added support for disk exclusion settings during backup and restore.</span></span>
* <span data-ttu-id="c0450-843">O Azure Backup adicionou suporte para restaurar vários ficheiros/pastas no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="c0450-843">Azure Backup Added Support for Restoring Multiple files/folders in AzureFileShare</span></span>
* <span data-ttu-id="c0450-844">O Azure Backup adicionou suporte para o Resourcegroup especificado pelo utilizador durante a atualização da Política IaasVM</span><span class="sxs-lookup"><span data-stu-id="c0450-844">Azure Backup Added support for User-specified Resourcegroup support while updating IaasVM Policy</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-845">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-845">Az.Resources</span></span>
* <span data-ttu-id="c0450-846">Foi corrigido o parâmetro "Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType" para utilizar a apiVersion real dos recursos em vez da apiVersion predefinida [#11267]</span><span class="sxs-lookup"><span data-stu-id="c0450-846">Fixed 'Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType' to use actual apiVersion of resources instead of default apiVersion [#11267]</span></span>
* <span data-ttu-id="c0450-847">Foi adicionado o registo de correlationId para cenários de erro</span><span class="sxs-lookup"><span data-stu-id="c0450-847">Added correlationId logging for error scenarios</span></span>
* <span data-ttu-id="c0450-848">Pequena alteração à documentação referente a "Get-AzResourceLock".</span><span class="sxs-lookup"><span data-stu-id="c0450-848">Small documentation change to 'Get-AzResourceLock'.</span></span> <span data-ttu-id="c0450-849">Exemplo adicionado.</span><span class="sxs-lookup"><span data-stu-id="c0450-849">Added example.</span></span>
* <span data-ttu-id="c0450-850">Aspas com caráter de escape no valor de parâmetro "Get-AzADUser" [#11317]</span><span class="sxs-lookup"><span data-stu-id="c0450-850">Escaped single quote in parameter value of 'Get-AzADUser' [#11317]</span></span>
* <span data-ttu-id="c0450-851">Foram adicionados novos cmdlets aos Scripts de Implementação ("Get-AzDeploymentScript", "Get-AzDeploymentScriptLog", "Save-AzDeploymentScriptLog", "Remove-AzDeploymentScript")</span><span class="sxs-lookup"><span data-stu-id="c0450-851">Added new cmdlets for Deployment Scripts ('Get-AzDeploymentScript', 'Get-AzDeploymentScriptLog', 'Save-AzDeploymentScriptLog', 'Remove-AzDeploymentScript')</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-852">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-852">Az.Sql</span></span>
* <span data-ttu-id="c0450-853">Foi adicionado um parâmetro secundário legível a "Invoke-AzSqlDatabaseFailover"</span><span class="sxs-lookup"><span data-stu-id="c0450-853">Added readable secondary parameter to 'Invoke-AzSqlDatabaseFailover'</span></span>
* <span data-ttu-id="c0450-854">Foi adicionado o cmdlet "Disable-AzSqlServerActiveDirectoryOnlyAuthentication"</span><span class="sxs-lookup"><span data-stu-id="c0450-854">Added cmdlet 'Disable-AzSqlServerActiveDirectoryOnlyAuthentication'</span></span>
* <span data-ttu-id="c0450-855">Classificação de sensibilidade guardada ao classificar as colunas na base de dados.</span><span class="sxs-lookup"><span data-stu-id="c0450-855">Saved sensitivity rank when classifying columns in the database.</span></span>

#### <a name="azsupport"></a><span data-ttu-id="c0450-856">Az.Support</span><span class="sxs-lookup"><span data-stu-id="c0450-856">Az.Support</span></span>
* <span data-ttu-id="c0450-857">Disponibilidade geral do módulo "Az.Support"</span><span class="sxs-lookup"><span data-stu-id="c0450-857">General availability of 'Az.Support' module</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c0450-858">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-858">Az.Websites</span></span>
* <span data-ttu-id="c0450-859">Foi adicionado suporte para utilizar Regras de Encaminhamento de Tráfego webapp através dos novos cmdlets abaixo</span><span class="sxs-lookup"><span data-stu-id="c0450-859">Added support for working with webapp Traffic Routing Rules via below new cmdlets</span></span>
    - <span data-ttu-id="c0450-860">"Get-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="c0450-860">'Get-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="c0450-861">"Update-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="c0450-861">'Update-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="c0450-862">"Add-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="c0450-862">'Add-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="c0450-863">"Remove-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="c0450-863">'Remove-AzWebAppTrafficRouting'</span></span>

## <a name="361---march-2020"></a><span data-ttu-id="c0450-864">3.6.1 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="c0450-864">3.6.1 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c0450-865">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-865">Az.Accounts</span></span>
* <span data-ttu-id="c0450-866">Abrir a página de inquérito do Azure PowerShell em "Send-Feedback" [#11020]</span><span class="sxs-lookup"><span data-stu-id="c0450-866">Open Azure PowerShell survey page in 'Send-Feedback' [#11020]</span></span>
* <span data-ttu-id="c0450-867">Apresentar o URL de inquérito do Azure PowerShell em "Resolve-Error" [#11021]</span><span class="sxs-lookup"><span data-stu-id="c0450-867">Display Azure PowerShell survey URL in 'Resolve-Error' [#11021]</span></span>
* <span data-ttu-id="c0450-868">Adicionada versão de Az em UserAgent</span><span class="sxs-lookup"><span data-stu-id="c0450-868">Added Az version in UserAgent</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c0450-869">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c0450-869">Az.ApiManagement</span></span>
* <span data-ttu-id="c0450-870">Adicionado suporte para a obtenção e configuração do Domínio Personalizado no Ponto Final do DeveloperPortal [#11007]</span><span class="sxs-lookup"><span data-stu-id="c0450-870">Added support for retrieving and configuring Custom Domain on the DeveloperPortal Endpoint [#11007]</span></span>
* <span data-ttu-id="c0450-871">"Export-AzApiManagementApi" Adicionado suporte para a transferência da definição da API no formato JSON [#9987]</span><span class="sxs-lookup"><span data-stu-id="c0450-871">'Export-AzApiManagementApi' Added support for downloading Api Definition in Json format [#9987]</span></span>
* <span data-ttu-id="c0450-872">"Import-AzApiManagementApi" Adicionado suporte para a importação da definição de OpenApi 3.0 a partir de documento JSON</span><span class="sxs-lookup"><span data-stu-id="c0450-872">'Import-AzApiManagementApi' Added support for importing OpenApi 3.0 definition from Json document</span></span>
* <span data-ttu-id="c0450-873">"New-AzApiManagementIdentityProvider" e "Set-AzApiManagementIdentityProvider" Adicionado suporte para a configuração de "Inquilino de Início de Sessão" para Fornecedor de AAD B2C [#9784]</span><span class="sxs-lookup"><span data-stu-id="c0450-873">'New-AzApiManagementIdentityProvider' and 'Set-AzApiManagementIdentityProvider' Added support for configuring 'Signin Tenant' for AAD B2C Provider [#9784]</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c0450-874">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c0450-874">Az.DataLakeStore</span></span>
* <span data-ttu-id="c0450-875">Adicionada referência a System.Buffers explicitamente em csproj e psd1.</span><span class="sxs-lookup"><span data-stu-id="c0450-875">Added reference to System.Buffers explicitly in csproj and psd1.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c0450-876">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c0450-876">Az.IotHub</span></span>
* <span data-ttu-id="c0450-877">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="c0450-877">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="c0450-878">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="c0450-878">New Cmdlets are:</span></span>
    - <span data-ttu-id="c0450-879">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="c0450-879">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="c0450-880">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="c0450-880">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="c0450-881">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="c0450-881">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="c0450-882">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="c0450-882">'Set-AzIotHubDevice'</span></span>
* <span data-ttu-id="c0450-883">Adicionado suporte para a gestão de módulos num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="c0450-883">Added support to manage modules on a target Iot device in an Iot Hub.</span></span> <span data-ttu-id="c0450-884">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="c0450-884">New Cmdlets are:</span></span>
    - <span data-ttu-id="c0450-885">"Add-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="c0450-885">'Add-AzIotHubModule'</span></span>
    - <span data-ttu-id="c0450-886">"Get-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="c0450-886">'Get-AzIotHubModule'</span></span>
    - <span data-ttu-id="c0450-887">"Remove-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="c0450-887">'Remove-AzIotHubModule'</span></span>
    - <span data-ttu-id="c0450-888">"Set-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="c0450-888">'Set-AzIotHubModule'</span></span>
* <span data-ttu-id="c0450-889">Adicionado cmdlet para obter a cadeia de ligação de um dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="c0450-889">Added cmdlet to get the connection string of a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="c0450-890">Adicionado cmdlet para obter a cadeia de ligação de um módulo num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="c0450-890">Added cmdlet to get the connection string of a module on a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="c0450-891">Adicionado suporte para obter/definir dispositivo principal de um dispositivo IoT.</span><span class="sxs-lookup"><span data-stu-id="c0450-891">Added support to get/set parent device of an IoT device.</span></span> <span data-ttu-id="c0450-892">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="c0450-892">New Cmdlets are:</span></span>
    - <span data-ttu-id="c0450-893">"Get-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="c0450-893">'Get-AzIotHubDeviceParent'</span></span>
    - <span data-ttu-id="c0450-894">"Set-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="c0450-894">'Set-AzIotHubDeviceParent'</span></span>
* <span data-ttu-id="c0450-895">Adicionado suporte para gerir relações principal-subordinado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0450-895">Added support to manage device parent-child relationship.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c0450-896">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c0450-896">Az.Monitor</span></span>
* <span data-ttu-id="c0450-897">Corrigido o valor de saída de "Get-AzMetricDefinition" [#9714]</span><span class="sxs-lookup"><span data-stu-id="c0450-897">Fixed output value for 'Get-AzMetricDefinition' [#9714]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-898">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-898">Az.Network</span></span>
* <span data-ttu-id="c0450-899">Sdk Sql Management atualizado.</span><span class="sxs-lookup"><span data-stu-id="c0450-899">Updated Sql Management SDK.</span></span>
* <span data-ttu-id="c0450-900">Corrigido um problema de diferença de nomes na classe PrivateLinkServiceConnectionState.</span><span class="sxs-lookup"><span data-stu-id="c0450-900">Fixed a naming-difference issue in PrivateLinkServiceConnectionState class.</span></span>
    - <span data-ttu-id="c0450-901">Mapeamento do campo ActionsRequired para ActionRequired.</span><span class="sxs-lookup"><span data-stu-id="c0450-901">Mapping the field ActionsRequired to ActionRequired.</span></span>
* <span data-ttu-id="c0450-902">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="c0450-902">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-903">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-903">Az.Resources</span></span>
* <span data-ttu-id="c0450-904">Correção para erro de referência nula em "Get-AzRoleAssignment"</span><span class="sxs-lookup"><span data-stu-id="c0450-904">Fixed for null reference bug in 'Get-AzRoleAssignment'</span></span>
* <span data-ttu-id="c0450-905">Comutadores "-Force" e "-PassThru" marcados como opcionais em "Remove-AzADGroup" [#10849]</span><span class="sxs-lookup"><span data-stu-id="c0450-905">Marked switch '-Force' and '-PassThru' optional in 'Remove-AzADGroup' [#10849]</span></span>
* <span data-ttu-id="c0450-906">Corrigido problema em que "MailNickname" não devolve "Remove-AzADGroup" [#11167]</span><span class="sxs-lookup"><span data-stu-id="c0450-906">Fixed issue that 'MailNickname' doesn't return in 'Remove-AzADGroup' [#11167]</span></span>
* <span data-ttu-id="c0450-907">Corrigido problema em que a operação de pipe "Remove-AzADGroup" não funciona [#11171]</span><span class="sxs-lookup"><span data-stu-id="c0450-907">Fixed issue that 'Remove-AzADGroup' pipe operation doesn't work [#11171]</span></span>
* <span data-ttu-id="c0450-908">Correção para erro de referência nula em GetAzureRoleAssignmentCommand</span><span class="sxs-lookup"><span data-stu-id="c0450-908">Fixed for null reference bug in GetAzureRoleAssignmentCommand</span></span>
* <span data-ttu-id="c0450-909">Adicionados atributos de alterações interruptivas para futuras alterações a cmdlets de política</span><span class="sxs-lookup"><span data-stu-id="c0450-909">Added breaking change attributes for upcoming changes to policy cmdlets</span></span>
* <span data-ttu-id="c0450-910">"Get-AzResourceGroup" atualizado para realizar filtragem de etiqueta de grupo de recursos no lado do servidor</span><span class="sxs-lookup"><span data-stu-id="c0450-910">Updated 'Get-AzResourceGroup' to perform resource group tag filtering on server-side</span></span>
* <span data-ttu-id="c0450-911">Cmdlets Tag alargados para accept -ResourceId</span><span class="sxs-lookup"><span data-stu-id="c0450-911">Extended Tag cmdlets to accept -ResourceId</span></span>
    - <span data-ttu-id="c0450-912">Get-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="c0450-912">Get-AzTag -ResourceId</span></span>
    - <span data-ttu-id="c0450-913">New-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="c0450-913">New-AzTag -ResourceId</span></span>
    - <span data-ttu-id="c0450-914">Remove-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="c0450-914">Remove-AzTag -ResourceId</span></span>
* <span data-ttu-id="c0450-915">Adicionado cmdlet Tag novo</span><span class="sxs-lookup"><span data-stu-id="c0450-915">Added new Tag cmdlet</span></span>
    - <span data-ttu-id="c0450-916">Update-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="c0450-916">Update-AzTag -ResourceId</span></span>
* <span data-ttu-id="c0450-917">ScopedDeployment trazido de SDK 3.3.0</span><span class="sxs-lookup"><span data-stu-id="c0450-917">Brought ScopedDeployment from SDK 3.3.0</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-918">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-918">Az.Sql</span></span>
* <span data-ttu-id="c0450-919">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="c0450-919">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="c0450-920">Adicionado suporte para configuração de cópia de segurança de Retenção de Longo Prazo para Bases de Dados Geridas</span><span class="sxs-lookup"><span data-stu-id="c0450-920">Added support for Long Term Retention backup configuration for Managed Databases</span></span>
    - <span data-ttu-id="c0450-921">Política Get/Set numa base de dados gerida</span><span class="sxs-lookup"><span data-stu-id="c0450-921">Get/Set LTR policy on a managed database</span></span>
    - <span data-ttu-id="c0450-922">Obter cópia(s) de segurança LTR por base de dados gerida, por instância gerida ou por localização</span><span class="sxs-lookup"><span data-stu-id="c0450-922">Get LTR backup(s) by managed database, managed instance, or by location</span></span>
    - <span data-ttu-id="c0450-923">Remover uma cópia de segurança LTR</span><span class="sxs-lookup"><span data-stu-id="c0450-923">Remove an LTR backup</span></span>
    - <span data-ttu-id="c0450-924">Restaurar uma cópia de segurança LTR para criar uma base de dados gerida nova</span><span class="sxs-lookup"><span data-stu-id="c0450-924">Restore an LTR backup to create a new managed database</span></span>
* <span data-ttu-id="c0450-925">Adicionado MinimalTlsVersion a New-AzSqlServer e Set-AzSqlServer</span><span class="sxs-lookup"><span data-stu-id="c0450-925">Added MinimalTlsVersion to New-AzSqlServer and Set-AzSqlServer</span></span>
* <span data-ttu-id="c0450-926">Adicionado MinimalTlsVersion a New-AzSqlInstance e Set-AzSqlInstance</span><span class="sxs-lookup"><span data-stu-id="c0450-926">Added MinimalTlsVersion to New-AzSqlInstance and Set-AzSqlInstance</span></span>
* <span data-ttu-id="c0450-927">Versão de SDK SQL atualizada para Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-927">Bumped SQL SDK version for Az.Network</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-928">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-928">Az.Storage</span></span>
* <span data-ttu-id="c0450-929">AllowProtectedAppendWrite suportada em ImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="c0450-929">Supported AllowProtectedAppendWrite in ImmutabilityPolicy</span></span>
    - <span data-ttu-id="c0450-930">"Set-AzRmStorageContainerImmutabilityPolicy"</span><span class="sxs-lookup"><span data-stu-id="c0450-930">'Set-AzRmStorageContainerImmutabilityPolicy'</span></span>
* <span data-ttu-id="c0450-931">Adicionada uma mensagem de aviso de alteração interruptiva para alteração do tipo AzureStorageTable numa futura versão</span><span class="sxs-lookup"><span data-stu-id="c0450-931">Added breaking change warning message for AzureStorageTable type change in a future release</span></span>
    - <span data-ttu-id="c0450-932">"New-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="c0450-932">'New-AzStorageTable'</span></span>
    - <span data-ttu-id="c0450-933">"Get-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="c0450-933">'Get-AzStorageTable'</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c0450-934">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-934">Az.Websites</span></span>
* <span data-ttu-id="c0450-935">Adicionado o parâmetro Tag para "New-AzAppServicePlan" e "Set-AzAppServicePlan"</span><span class="sxs-lookup"><span data-stu-id="c0450-935">Added Tag parameter for 'New-AzAppServicePlan' and 'Set-AzAppServicePlan'</span></span>
* <span data-ttu-id="c0450-936">Paragem da execução de cmdlet caso seja emitida uma exceção ao adicionar um domínio personalizado a um site</span><span class="sxs-lookup"><span data-stu-id="c0450-936">Stop cmdlet execution if an exception is thrown when adding a custom domain to a website</span></span>
* <span data-ttu-id="c0450-937">Adicionado suporte para a realização de operações para Serviços de Aplicações em grupos de recursos diferentes do Plano do Serviço de Aplicações</span><span class="sxs-lookup"><span data-stu-id="c0450-937">Added support to perform operations for App Services not in the same resource group as the App Service Plan</span></span>
* <span data-ttu-id="c0450-938">Aplicada restrição de acesso a WebApp/Função em diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="c0450-938">Applied access restriction to WebApp/Function in different resource groups</span></span>
* <span data-ttu-id="c0450-939">Corrigido problema para definir os nomes de anfitrião personalizados para WebAppSlots</span><span class="sxs-lookup"><span data-stu-id="c0450-939">Fixed issue to set custom hostnames for WebAppSlots</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="c0450-940">3.5.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="c0450-940">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c0450-941">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="c0450-941">Highlights since the last major release</span></span>
* <span data-ttu-id="c0450-942">Telemetria do lado do cliente atualizada.</span><span class="sxs-lookup"><span data-stu-id="c0450-942">Updated client side telemetry.</span></span>
* <span data-ttu-id="c0450-943">O Az.IotHub adicionou cmdlets para suportar a gestão de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="c0450-943">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="c0450-944">O Az.SqlVirtualMachine adicionou cmdlets ao Serviço de Escuta do Grupo de Disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="c0450-944">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c0450-945">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-945">Az.Accounts</span></span>
* <span data-ttu-id="c0450-946">SubscriptionId, TenantId e tempo de execução adicionados aos dados de telemetria do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="c0450-946">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c0450-947">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c0450-947">Az.Automation</span></span>
* <span data-ttu-id="c0450-948">Foi corrigido o erro no Exemplo 1 na documentação de referência de "New-AzAutomationSoftwareUpdateConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c0450-948">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c0450-949">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c0450-949">Az.CognitiveServices</span></span>
* <span data-ttu-id="c0450-950">SDK atualizado para a versão 7.0</span><span class="sxs-lookup"><span data-stu-id="c0450-950">Updated SDK to 7.0</span></span>
* <span data-ttu-id="c0450-951">Mensagem de erro melhorada quando o servidor responde ao corpo vazio</span><span class="sxs-lookup"><span data-stu-id="c0450-951">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-952">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-952">Az.Compute</span></span>
* <span data-ttu-id="c0450-953">Valor vazio permitido para ProximityPlacementGroupId durante a atualização</span><span class="sxs-lookup"><span data-stu-id="c0450-953">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c0450-954">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c0450-954">Az.FrontDoor</span></span>
* <span data-ttu-id="c0450-955">Cmdlet adicionado para obter definições de regras geridas que podem ser utilizadas na WAF</span><span class="sxs-lookup"><span data-stu-id="c0450-955">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c0450-956">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c0450-956">Az.IotHub</span></span>
* <span data-ttu-id="c0450-957">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="c0450-957">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="c0450-958">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="c0450-958">New Cmdlets are:</span></span>
    - <span data-ttu-id="c0450-959">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="c0450-959">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="c0450-960">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="c0450-960">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="c0450-961">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="c0450-961">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="c0450-962">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="c0450-962">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c0450-963">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0450-963">Az.KeyVault</span></span>
* <span data-ttu-id="c0450-964">Texto duplicado fixo para Add-AzKeyVaultKey.md</span><span class="sxs-lookup"><span data-stu-id="c0450-964">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c0450-965">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c0450-965">Az.Monitor</span></span>
* <span data-ttu-id="c0450-966">Descrição fixa do cmdlet Get-AzLog.</span><span class="sxs-lookup"><span data-stu-id="c0450-966">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="c0450-967">Foi adicionado um novo parâmetro chamado ActionGroupId ao comando "New-AzMetricAlertRuleV2".</span><span class="sxs-lookup"><span data-stu-id="c0450-967">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="c0450-968">O utilizador pode fornecer ActionGroupId(string) ou ActionGorup(ActivityLogAlertActionGroup).</span><span class="sxs-lookup"><span data-stu-id="c0450-968">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-969">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-969">Az.Network</span></span>
* <span data-ttu-id="c0450-970">Foi adicionada uma nota de parâmetro adicional para o parâmetro "-EnableProxyProtocol" para o cmdlet "New-AzPrivateLinkService".</span><span class="sxs-lookup"><span data-stu-id="c0450-970">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="c0450-971">Exemplo de FilterData fixo em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="c0450-971">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="c0450-972">Exemplo de Captura de Pacotes adicionado para capturar todos os pacotes internos e externos em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="c0450-972">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="c0450-973">Política do Azure Firewall suportada em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="c0450-973">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="c0450-974">Não foram adicionados novos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="c0450-974">No new cmdlets are added.</span></span> <span data-ttu-id="c0450-975">Simplificação da restrição da política de firewall em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="c0450-975">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-976">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-976">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-977">Suporte adicionado da funcionalidade Restaurar como ficheiros para Bases de Dados SQL.</span><span class="sxs-lookup"><span data-stu-id="c0450-977">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-978">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-978">Az.Resources</span></span>
* <span data-ttu-id="c0450-979">Cmdlets de implementação de modelos refatorizados</span><span class="sxs-lookup"><span data-stu-id="c0450-979">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="c0450-980">Foram adicionados novos cmdlets para gerir implementações no grupo de gestão: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="c0450-980">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="c0450-981">Foram adicionados novos cmdlets para gerir implementações no inquilino: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="c0450-981">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="c0450-982">Cmdlets \*-AzDeployment refatorizados para trabalhar especificamente no âmbito da subscrição</span><span class="sxs-lookup"><span data-stu-id="c0450-982">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="c0450-983">Foram criados aliases \*-AzSubscriptionDeployment para os cmdlets \*-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="c0450-983">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="c0450-984">"Update-AzADApplication" fixo quando o parâmetro "AvailableToOtherTenants" não está definido</span><span class="sxs-lookup"><span data-stu-id="c0450-984">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="c0450-985">ApplicationObjectWithoutCredentialParameterSet removido para evitar AmbiguousParameterSetException.</span><span class="sxs-lookup"><span data-stu-id="c0450-985">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="c0450-986">Ficheiros de ajuda regenerados</span><span class="sxs-lookup"><span data-stu-id="c0450-986">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-987">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-987">Az.Sql</span></span>
* <span data-ttu-id="c0450-988">Suporte adicionado para restauro para um ponto anterior no tempo entre subscrições nas Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="c0450-988">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="c0450-989">Suporte adicionado para alterar a geração de hardware das Instâncias Geridas de SQL existentes</span><span class="sxs-lookup"><span data-stu-id="c0450-989">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="c0450-990">Exemplos de ajuda "Update-AzSqlServerVulnerabilityAssessmentSetting" fixos: saída do parâmetro/propriedade - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="c0450-990">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="c0450-991">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="c0450-991">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="c0450-992">Cmdlets adicionados para o Serviço de Escuta do Grupo de Disponibilidade</span><span class="sxs-lookup"><span data-stu-id="c0450-992">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="c0450-993">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="c0450-993">Az.StorageSync</span></span>
* <span data-ttu-id="c0450-994">Conjuntos de carateres suportados atualizados em "Invoke-AzStorageSyncCompatibilityCheck".</span><span class="sxs-lookup"><span data-stu-id="c0450-994">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="c0450-995">3.4.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="c0450-995">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c0450-996">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="c0450-996">Highlights since the last major release</span></span>
* <span data-ttu-id="c0450-997">Versão inicial Az.CosmosDB 0.1.0 lançada</span><span class="sxs-lookup"><span data-stu-id="c0450-997">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="c0450-998">Foi adicionado suporte para Az.Network ConnectionMonitor V2</span><span class="sxs-lookup"><span data-stu-id="c0450-998">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c0450-999">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-999">Az.Accounts</span></span>
* <span data-ttu-id="c0450-1000">Foi desativada a gravação automática de contexto quando AzureRmContext.json não está disponível</span><span class="sxs-lookup"><span data-stu-id="c0450-1000">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="c0450-1001">Atualização da referência ao Azure Powershell Common para a pré-visualização 1.3.5</span><span class="sxs-lookup"><span data-stu-id="c0450-1001">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c0450-1002">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c0450-1002">Az.ApiManagement</span></span>
* <span data-ttu-id="c0450-1003">**Get-AzApiManagementApiSchema** Foi corrigido ao obter Open-Api Schema associado a uma API   https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="c0450-1003">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="c0450-1004">**New-AzApiManagementProduct**\* e **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="c0450-1004">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="c0450-1005">Foi corrigida a documentação para https://github.com/Azure/azure-powershell/issues/10472</span><span class="sxs-lookup"><span data-stu-id="c0450-1005">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="c0450-1006">**Set-AzApiManagementApi** Exemplo adicionado para mostrar como atualizar o ServiceUrl com o cmdlet</span><span class="sxs-lookup"><span data-stu-id="c0450-1006">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-1007">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-1007">Az.Compute</span></span>
* <span data-ttu-id="c0450-1008">Foi limitado o número de estados de VM a 100 para evitar limitações quando Get-AzVM-Status é executado sem o nome da VM.</span><span class="sxs-lookup"><span data-stu-id="c0450-1008">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="c0450-1009">Foi adicionado o cmdlet Update-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="c0450-1009">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="c0450-1010">Foram adicionados os parâmetros EncryptionType e DiskEncryptionSetId aos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c0450-1010">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="c0450-1011">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-1011">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="c0450-1012">Foi adicionado o parâmetro ColocationStatus ao cmdlet Get-AzProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="c0450-1012">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c0450-1013">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c0450-1013">Az.DataFactory</span></span>
* <span data-ttu-id="c0450-1014">Atualização do SDK .NET do ADF para a versão 4.7.0</span><span class="sxs-lookup"><span data-stu-id="c0450-1014">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="c0450-1015">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="c0450-1015">Az.DeploymentManager</span></span>
* <span data-ttu-id="c0450-1016">Adiciona operações LIST para os recursos</span><span class="sxs-lookup"><span data-stu-id="c0450-1016">Adds LIST operations for resources</span></span>
* <span data-ttu-id="c0450-1017">Adiciona a capacidade de realizar operações nos passos de Verificação de Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="c0450-1017">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c0450-1018">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c0450-1018">Az.HDInsight</span></span>
* <span data-ttu-id="c0450-1019">Foi corrigido o erro do documento de New-AzHDInsightCluster.</span><span class="sxs-lookup"><span data-stu-id="c0450-1019">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c0450-1020">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0450-1020">Az.KeyVault</span></span>
* <span data-ttu-id="c0450-1021">Foi adicionado o alias do Nome ao atributo VaultName para tornar Remove-AzureKeyVault consistente com New-AzureKeyVault.</span><span class="sxs-lookup"><span data-stu-id="c0450-1021">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-1022">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-1022">Az.Network</span></span>
* <span data-ttu-id="c0450-1023">Foi adicionado um novo exemplo a Set-AzNetworkWatcherConfigFlowLog.md para demonstrar o cenário de desativação da Análise de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="c0450-1023">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="c0450-1024">Foi adicionado suporte para atribuir a configuração IP de gestão ao Azure Firewall, uma sub-rede dedicada e IP Público que a firewall utilizará no tráfego de gestão</span><span class="sxs-lookup"><span data-stu-id="c0450-1024">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="c0450-1025">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="c0450-1025">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="c0450-1026">Foi adicionado o parâmetro -ManagementPublicIpAddress (não obrigatório) que aceita um objeto de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="c0450-1026">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="c0450-1027">Foi adicionado o método SetManagementIpConfiguration no objeto de firewall. Requer uma sub-rede e um endereço IP Público como entrada. O nome da sub-rede tem de ser "AzureFirewallManagementSubnet"</span><span class="sxs-lookup"><span data-stu-id="c0450-1027">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="c0450-1028">Foram corrigidos os exemplos de Get-AzNetworkSecurityGroup para mostrar exemplos de NSGs em vez de interfaces de rede.</span><span class="sxs-lookup"><span data-stu-id="c0450-1028">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="c0450-1029">Foi corrigido um erro no comando New-AzVpnSite que estava a impedir o ID do recurso de concluir um parâmetro.</span><span class="sxs-lookup"><span data-stu-id="c0450-1029">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="c0450-1030">Foi adicionado suporte para a Configuração do URL em Reescrever Conjunto de Ações de Regras no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="c0450-1030">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="c0450-1031">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c0450-1031">New cmdlets added:</span></span>
        - <span data-ttu-id="c0450-1032">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0450-1032">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="c0450-1033">Foram atualizados cmdlets com o parâmetro opcional - UrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0450-1033">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="c0450-1034">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="c0450-1034">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="c0450-1035">Foi adicionado suporte para os recursos do NetworkWatcher ConnectionMonitor versão 2</span><span class="sxs-lookup"><span data-stu-id="c0450-1035">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c0450-1036">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-1036">Az.PolicyInsights</span></span>
* <span data-ttu-id="c0450-1037">Foi adicionado suporte para avaliar a conformidade antes de determinar o recurso a remediar</span><span class="sxs-lookup"><span data-stu-id="c0450-1037">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="c0450-1038">Foi adicionado o parâmetro "-ResourceDiscoverMode" a Start-AzPolicyRemediation</span><span class="sxs-lookup"><span data-stu-id="c0450-1038">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="c0450-1039">Foi adicionado o cmdlet Get-AzPolicyMetadata para obter os recursos de metadados da política</span><span class="sxs-lookup"><span data-stu-id="c0450-1039">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="c0450-1040">Get-AzPolicyState e Get-AzPolicyStateSummary atualizados para a versão da API 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="c0450-1040">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-1041">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-1041">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-1042">Foi adicionado suporte do Azure Site Recovery para remover um disco replicado.</span><span class="sxs-lookup"><span data-stu-id="c0450-1042">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="c0450-1043">O Azure Backup adicionou suporte para adicionar etiquetas ao criar um Cofre dos Serviços de Recuperação.</span><span class="sxs-lookup"><span data-stu-id="c0450-1043">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-1044">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-1044">Az.Resources</span></span>
* <span data-ttu-id="c0450-1045">-Scope foi tornado opcional nos cmdlets \*-AzPolicyAssignment com subscrição de contexto predefinida</span><span class="sxs-lookup"><span data-stu-id="c0450-1045">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="c0450-1046">Foram adicionados exemplos de criação de ADServicePrincipal com credenciais de palavras-passe e chaves</span><span class="sxs-lookup"><span data-stu-id="c0450-1046">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-1047">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-1047">Az.Sql</span></span>
<span data-ttu-id="c0450-1048">Foi corrigido o cmdlet New-AzSqlDatabaseSecondary para verificar a existência de PartnerDatabaseName em vez da existência de DatabaseName.</span><span class="sxs-lookup"><span data-stu-id="c0450-1048">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-1049">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-1049">Az.Storage</span></span>
* <span data-ttu-id="c0450-1050">Foi definido o suporte de Tipo de Chave de Encriptação na Tabela/Fila em Criar Conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="c0450-1050">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="c0450-1051">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c0450-1051">New-AzStorageAccount</span></span>
* <span data-ttu-id="c0450-1052">Será apresentado RequestId quando StorageException não tiver ExtendedErrorInformation</span><span class="sxs-lookup"><span data-stu-id="c0450-1052">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="c0450-1053">Foi corrigido o exemplo 6 do cmdlet Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="c0450-1053">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c0450-1054">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-1054">Az.Websites</span></span>
* <span data-ttu-id="c0450-1055">Set-AzWebapp e Set-AzWebappSlot suportam as propriedades AlwaysOn, MinTls e FtpsState</span><span class="sxs-lookup"><span data-stu-id="c0450-1055">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="c0450-1056">Foi corrigido o problema em que a definição de HttpsOnly, juntamente com a alteração de AppservicePlan ao utilizar o único comando Set-AzWebApp, estava a repor HttpsOnly para o valor predefinido</span><span class="sxs-lookup"><span data-stu-id="c0450-1056">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="c0450-1057">3.3.0 – janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="c0450-1057">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c0450-1058">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-1058">Az.Accounts</span></span>
* <span data-ttu-id="c0450-1059">Add-AzEnvironment e Set-AzEnvironment foram atualizados para aceitar os parâmetros AzureAttestationServiceEndpointResourceId e AzureAttestationServiceEndpointSuffix</span><span class="sxs-lookup"><span data-stu-id="c0450-1059">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c0450-1060">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c0450-1060">Az.Cdn</span></span>
* <span data-ttu-id="c0450-1061">Apresentação dos detalhes da resposta de erro no cmdlet New-AzCdnEndpoint</span><span class="sxs-lookup"><span data-stu-id="c0450-1061">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-1062">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-1062">Az.Compute</span></span>
* <span data-ttu-id="c0450-1063">Correção do cmdlet Set-AzVMCustomScriptExtension para uma VM com disco OD gerido sem perfil de SO.</span><span class="sxs-lookup"><span data-stu-id="c0450-1063">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="c0450-1064">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="c0450-1064">Az.ContainerInstance</span></span>
* <span data-ttu-id="c0450-1065">Foram corrigidos os nomes de parâmetros utilizados pelo exemplo de New-AzContainerGroup</span><span class="sxs-lookup"><span data-stu-id="c0450-1065">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="c0450-1066">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="c0450-1066">Az.DataBoxEdge</span></span>
* <span data-ttu-id="c0450-1067">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="c0450-1067">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="c0450-1068">Obter o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="c0450-1068">Get the Edge Storage Container</span></span>
* <span data-ttu-id="c0450-1069">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="c0450-1069">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="c0450-1070">Criar novo Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="c0450-1070">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="c0450-1071">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="c0450-1071">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="c0450-1072">Remover o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="c0450-1072">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="c0450-1073">Foi adicionado o cmdlet "Invoke-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="c0450-1073">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="c0450-1074">Invocar ação para atualizar os dados no Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="c0450-1074">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="c0450-1075">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c0450-1075">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="c0450-1076">Obter a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="c0450-1076">Get the Edge Storage Account</span></span>
* <span data-ttu-id="c0450-1077">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c0450-1077">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="c0450-1078">Criar nova Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="c0450-1078">Create new Edge Storage Account</span></span>
* <span data-ttu-id="c0450-1079">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c0450-1079">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="c0450-1080">Remover a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="c0450-1080">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="c0450-1081">Invocar o cmdlet "Invoke-AzDataBoxEdgeShare"</span><span class="sxs-lookup"><span data-stu-id="c0450-1081">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="c0450-1082">Invocar ação para atualizar os dados na partilha</span><span class="sxs-lookup"><span data-stu-id="c0450-1082">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="c0450-1083">Foi adicionado o cmdlet "Set-AzDataBoxEdgeStorageAccountCredential"</span><span class="sxs-lookup"><span data-stu-id="c0450-1083">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="c0450-1084">Definição de AzDataBoxEdgeStorageAccountCredential</span><span class="sxs-lookup"><span data-stu-id="c0450-1084">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c0450-1085">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c0450-1085">Az.DataFactory</span></span>
* <span data-ttu-id="c0450-1086">Adição das propriedades AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId e VersionStatus para o cmd Get-AzDataFactoryV2IntegrationRuntime</span><span class="sxs-lookup"><span data-stu-id="c0450-1086">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="c0450-1087">Atualização do SDK .NET do ADF para a versão 4.6.0</span><span class="sxs-lookup"><span data-stu-id="c0450-1087">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="c0450-1088">Adição do parâmetro "PublicIPs" para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a criação de Azure-SSIS IR com endereços IP públicos estáticos.</span><span class="sxs-lookup"><span data-stu-id="c0450-1088">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="c0450-1089">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="c0450-1089">Az.DevTestLabs</span></span>
* <span data-ttu-id="c0450-1090">Remoção da ligação quebrada em Get-AzDtlAllowedVMSizesPolicy.md</span><span class="sxs-lookup"><span data-stu-id="c0450-1090">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c0450-1091">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c0450-1091">Az.EventHub</span></span>
* <span data-ttu-id="c0450-1092">Correção do problema 10634: Correção da referência de objeto nulo para remover eventhubnamespace</span><span class="sxs-lookup"><span data-stu-id="c0450-1092">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c0450-1093">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c0450-1093">Az.HDInsight</span></span>
* <span data-ttu-id="c0450-1094">Correção do erro Invoke-AzHDInsightHiveJob.md.</span><span class="sxs-lookup"><span data-stu-id="c0450-1094">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="c0450-1095">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="c0450-1095">Az.MachineLearning</span></span>
* <span data-ttu-id="c0450-1096">Foram removidos os cmdlets abaixo porque MachineLearningCompute já não está disponível</span><span class="sxs-lookup"><span data-stu-id="c0450-1096">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="c0450-1097">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="c0450-1097">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="c0450-1098">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="c0450-1098">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="c0450-1099">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="c0450-1099">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="c0450-1100">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="c0450-1100">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="c0450-1101">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="c0450-1101">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="c0450-1102">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="c0450-1102">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="c0450-1103">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="c0450-1103">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-1104">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-1104">Az.Network</span></span>
* <span data-ttu-id="c0450-1105">Atualização da dependência de Microsoft.Azure.Management.SQL da versão 1.36-preview para 1.37-preview</span><span class="sxs-lookup"><span data-stu-id="c0450-1105">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-1106">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-1106">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-1107">Alteração do Azure Site Recovery para suportar VMs de disco gerido com encriptação inativa com chaves geridas pelo cliente para o fornecedor do Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-1107">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="c0450-1108">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-1108">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="c0450-1109">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional ao nível do disco para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-1109">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="c0450-1110">Suporte do Azure Site Recovery para atualizar o item protegido por replicação com encriptação de discos e definir o mapa para HyperV para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-1110">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-1111">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-1111">Az.Resources</span></span>
* <span data-ttu-id="c0450-1112">Correção de um erro no documento de ajuda de "Remove-AzTag".</span><span class="sxs-lookup"><span data-stu-id="c0450-1112">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-1113">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-1113">Az.Sql</span></span>
* <span data-ttu-id="c0450-1114">Correção da funcionalidade dos cmdlets de linha de base do conjunto de avaliação de vulnerabilidades para funcionar na base de dados mestre da base de dados do Azure e limitá-la nas bases de dados do sistema de instância gerida</span><span class="sxs-lookup"><span data-stu-id="c0450-1114">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="c0450-1115">Correção de um erro ao criar o grupo de ativação pós-falha de instância SQL</span><span class="sxs-lookup"><span data-stu-id="c0450-1115">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="c0450-1116">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="c0450-1116">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="c0450-1117">Adição de DR como um novo tipo de Licença válido</span><span class="sxs-lookup"><span data-stu-id="c0450-1117">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-1118">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-1118">Az.Storage</span></span>
* <span data-ttu-id="c0450-1119">Adição de uma mensagem de aviso de alteração interruptiva para alteração do valor de DefaultAction numa futura versão</span><span class="sxs-lookup"><span data-stu-id="c0450-1119">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="c0450-1120">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="c0450-1120">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="c0450-1121">Suporte para obter a hora da última sincronização da conta de armazenamento ao executar get-AzureRMStorageAccount com o parâmetro -IncludeGeoReplicationStats</span><span class="sxs-lookup"><span data-stu-id="c0450-1121">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span>
    - <span data-ttu-id="c0450-1122">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c0450-1122">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="c0450-1123">3.2.0 - Dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-1123">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="c0450-1124">Geral</span><span class="sxs-lookup"><span data-stu-id="c0450-1124">General</span></span>
* <span data-ttu-id="c0450-1125">Atualização das referências em .psd1 para utilizar o caminho relativo para todos os módulos</span><span class="sxs-lookup"><span data-stu-id="c0450-1125">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c0450-1126">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-1126">Az.Accounts</span></span>
* <span data-ttu-id="c0450-1127">Definição do UserAgent correto para telemetria do lado do cliente para a pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="c0450-1127">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="c0450-1128">Apresentação de mensagem de erro amigável de utilizador quando o contexto é nulo na pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="c0450-1128">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c0450-1129">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c0450-1129">Az.Batch</span></span>
* <span data-ttu-id="c0450-1130">Correção do problema [10602](https://github.com/Azure/azure-powershell/issues/10602), em que **New-AzBatchPool** não enviava corretamente "VirtualMachineConfiguration.ContainerConfiguration" ou "VirtualMachineConfiguration.DataDisks" para o servidor.</span><span class="sxs-lookup"><span data-stu-id="c0450-1130">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c0450-1131">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c0450-1131">Az.DataFactory</span></span>
* <span data-ttu-id="c0450-1132">Atualização do SDK .NET do ADF para a versão 4.5.0</span><span class="sxs-lookup"><span data-stu-id="c0450-1132">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c0450-1133">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c0450-1133">Az.FrontDoor</span></span>
* <span data-ttu-id="c0450-1134">Adição do suporte de exclusão de regras geridas pela WAF</span><span class="sxs-lookup"><span data-stu-id="c0450-1134">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="c0450-1135">Adição de SocketAddr ao preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="c0450-1135">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="c0450-1136">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="c0450-1136">Az.HealthcareApis</span></span>
* <span data-ttu-id="c0450-1137">Processamento de Exceções</span><span class="sxs-lookup"><span data-stu-id="c0450-1137">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c0450-1138">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0450-1138">Az.KeyVault</span></span>
* <span data-ttu-id="c0450-1139">Correção do erro em que era acedido um valor potencialmente não definido</span><span class="sxs-lookup"><span data-stu-id="c0450-1139">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="c0450-1140">Gestão de Certificados de Criptografia de Curva Elíptica</span><span class="sxs-lookup"><span data-stu-id="c0450-1140">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="c0450-1141">Adicionado suporte para especificar a Curva das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="c0450-1141">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c0450-1142">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c0450-1142">Az.Monitor</span></span>
* <span data-ttu-id="c0450-1143">Adição de um argumento opcional ao comando Adicionar Definições de Diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="c0450-1143">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="c0450-1144">Um argumento de opção que, se estiver presente, indica que a exportação para o Log Analytics deve ser feita para um esquema fixo (também conhecido como</span><span class="sxs-lookup"><span data-stu-id="c0450-1144">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="c0450-1145">tipo de dados dedicado)</span><span class="sxs-lookup"><span data-stu-id="c0450-1145">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-1146">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-1146">Az.Network</span></span>
* <span data-ttu-id="c0450-1147">Suporte para IpGroups na aplicação AzureFirewall, Nat e Regras de Rede.</span><span class="sxs-lookup"><span data-stu-id="c0450-1147">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-1148">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-1148">Az.Resources</span></span>
* <span data-ttu-id="c0450-1149">Correção de um problema em que a implementação do modelo não consegue ler um parâmetro se o nome estiver em conflito com um nome de parâmetro incorporado.</span><span class="sxs-lookup"><span data-stu-id="c0450-1149">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="c0450-1150">Os cmdlets da política foram atualizados para utilizar a nova versão de API 2019-09-01 que introduz suporte de agrupamento nas definições do conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="c0450-1150">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-1151">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-1151">Az.Sql</span></span>
* <span data-ttu-id="c0450-1152">Criação do armazenamento atualizada na ativação automática da Avaliação de Vulnerabilidades para StorageV2</span><span class="sxs-lookup"><span data-stu-id="c0450-1152">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-1153">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-1153">Az.Storage</span></span>
* <span data-ttu-id="c0450-1154">Suporte para gerar um token de SAS baseado na Identidade do Blob/Contentor com Contexto de Armazenamento baseado na autenticação OAuth</span><span class="sxs-lookup"><span data-stu-id="c0450-1154">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="c0450-1155">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="c0450-1155">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="c0450-1156">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="c0450-1156">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="c0450-1157">Suporte para revogar as Chaves de Delegação do Utilizador da Conta de Armazenamento, pelo que todos os tokens de SAS da identidade são revogados</span><span class="sxs-lookup"><span data-stu-id="c0450-1157">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="c0450-1158">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="c0450-1158">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="c0450-1159">Atualização de Microsoft.Azure.Management.Storage 14.2.0 para suportar a nova versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="c0450-1159">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="c0450-1160">Suporte de QuotaGiB (Quota de Partilha em Gibibye) para obter valores superiores a 5120 no plano de Gestão de cmdlets de Partilha de Ficheiros e foi adicionado o alias do parâmetro "Quota" ao parâmetro "QuotaGiB".</span><span class="sxs-lookup"><span data-stu-id="c0450-1160">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span>
    - <span data-ttu-id="c0450-1161">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="c0450-1161">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="c0450-1162">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="c0450-1162">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="c0450-1163">Adição do alias do parâmetro "QuotaGiB" ao parâmetro "Quota"</span><span class="sxs-lookup"><span data-stu-id="c0450-1163">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="c0450-1164">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="c0450-1164">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="c0450-1165">Correção do problema em que Set-AzStorageContainerAcl consegue limpar a Política de Acesso armazenada</span><span class="sxs-lookup"><span data-stu-id="c0450-1165">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="c0450-1166">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="c0450-1166">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="c0450-1167">3.1.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-1167">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c0450-1168">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="c0450-1168">Highlights since the last major release</span></span>
* <span data-ttu-id="c0450-1169">Az.DataBoxEdge 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="c0450-1169">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="c0450-1170">Az.SqlVirtualMachine 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="c0450-1170">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-1171">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-1171">Az.Compute</span></span>
* <span data-ttu-id="c0450-1172">Funcionalidade de Reaplicação da VM</span><span class="sxs-lookup"><span data-stu-id="c0450-1172">VM Reapply feature</span></span>
    - <span data-ttu-id="c0450-1173">Adição do parâmetro Reapply ao cmdlet Set-AzVM</span><span class="sxs-lookup"><span data-stu-id="c0450-1173">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="c0450-1174">Funcionalidade AutomaticRepairs do Conjunto de Dimensionamento de VM:</span><span class="sxs-lookup"><span data-stu-id="c0450-1174">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="c0450-1175">Adição dos parâmetros EnableAutomaticRepair, AutomaticRepairGracePeriod e AutomaticRepairMaxInstanceRepairsPercent aos seguintes cmdlets:   New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="c0450-1175">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="c0450-1176">Suporte para imagens de galeria entre inquilinos para New-AzVM</span><span class="sxs-lookup"><span data-stu-id="c0450-1176">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="c0450-1177">Adição de "Spot" ao preenchedor de argumentos do parâmetro Priority nos cmdlets New-AzVM, New-AzVMConfig e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="c0450-1177">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="c0450-1178">Adição dos parâmetros DiskIOPSReadWrite e DiskMBpsReadWrite ao cmdlet Add-AzVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="c0450-1178">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="c0450-1179">Alteração do parâmetro SourceImageId do cmdlet New-AzGalleryImageVersion para opcional</span><span class="sxs-lookup"><span data-stu-id="c0450-1179">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="c0450-1180">Adição dos parâmetros OSDiskImage e DataDiskImage ao cmdlet New-AzGalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="c0450-1180">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="c0450-1181">Adição do parâmetro HyperVGeneration ao cmdlet New-AzGalleryImageDefinition</span><span class="sxs-lookup"><span data-stu-id="c0450-1181">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="c0450-1182">Adição dos parâmetros SkipExtensionsOnOverprovisionedVMs aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="c0450-1182">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="c0450-1183">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="c0450-1183">Az.DataBoxEdge</span></span>
* <span data-ttu-id="c0450-1184">Adição do cmdlet `Get-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="c0450-1184">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="c0450-1185">Obter a Encomenda</span><span class="sxs-lookup"><span data-stu-id="c0450-1185">Get the Order</span></span>
* <span data-ttu-id="c0450-1186">Adição do cmdlet `New-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="c0450-1186">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="c0450-1187">Criar nova Encomenda</span><span class="sxs-lookup"><span data-stu-id="c0450-1187">Create new Order</span></span>
* <span data-ttu-id="c0450-1188">Adição do cmdlet `Remove-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="c0450-1188">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="c0450-1189">Remover a Encomenda</span><span class="sxs-lookup"><span data-stu-id="c0450-1189">Remove the Order</span></span>
* <span data-ttu-id="c0450-1190">Alteração no cmdlet `New-AzDataBoxEdgeShare`</span><span class="sxs-lookup"><span data-stu-id="c0450-1190">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="c0450-1191">Agora cria uma Partilha Local</span><span class="sxs-lookup"><span data-stu-id="c0450-1191">Now creates Local Share</span></span>
* <span data-ttu-id="c0450-1192">Adição do cmdlet `Set-AzDataBoxEdgeRole`</span><span class="sxs-lookup"><span data-stu-id="c0450-1192">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="c0450-1193">Agora, o IotRole pode ser mapeado para a Partilha</span><span class="sxs-lookup"><span data-stu-id="c0450-1193">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="c0450-1194">Adição do cmdlet `Invoke-AzDataBoxEdgeDevice`</span><span class="sxs-lookup"><span data-stu-id="c0450-1194">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="c0450-1195">Invocar verificação da atualização, transferência da atualização, instalação das atualizações no dispositivo</span><span class="sxs-lookup"><span data-stu-id="c0450-1195">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="c0450-1196">Adição do cmdlet `Get-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="c0450-1196">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="c0450-1197">Obtém as informações sobre os Acionadores</span><span class="sxs-lookup"><span data-stu-id="c0450-1197">Gets the information about Triggers</span></span>
* <span data-ttu-id="c0450-1198">Adição do cmdlet `New-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="c0450-1198">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="c0450-1199">Criar novos Acionadores</span><span class="sxs-lookup"><span data-stu-id="c0450-1199">Create new Triggers</span></span>
* <span data-ttu-id="c0450-1200">Adição do cmdlet `Remove-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="c0450-1200">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="c0450-1201">Remover os Acionadores</span><span class="sxs-lookup"><span data-stu-id="c0450-1201">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c0450-1202">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c0450-1202">Az.DataFactory</span></span>
* <span data-ttu-id="c0450-1203">Atualização do SDK .NET do ADF para a versão 4.4.0</span><span class="sxs-lookup"><span data-stu-id="c0450-1203">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="c0450-1204">Adição do parâmetro "ExpressCustomSetup" para o cmdlet "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir configurações e componentes de terceiros sem scripts de configuração personalizados.</span><span class="sxs-lookup"><span data-stu-id="c0450-1204">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c0450-1205">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c0450-1205">Az.DataLakeStore</span></span>
* <span data-ttu-id="c0450-1206">Atualização da documentação de Get-AzDataLakeStoreDeletedItem e Restore-AzDataLakeStoreDeletedItem</span><span class="sxs-lookup"><span data-stu-id="c0450-1206">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c0450-1207">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c0450-1207">Az.EventHub</span></span>
* <span data-ttu-id="c0450-1208">Correção do problema 10301: Correção do formato de data do token de SAS</span><span class="sxs-lookup"><span data-stu-id="c0450-1208">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c0450-1209">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c0450-1209">Az.FrontDoor</span></span>
* <span data-ttu-id="c0450-1210">Adição do parâmetro MinimumTlsVersion a Enable-AzFrontDoorCustomDomainHttps e New-AzFrontDoorFrontendEndpointObject</span><span class="sxs-lookup"><span data-stu-id="c0450-1210">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="c0450-1211">Adição dos parâmetros HealthProbeMethod e EnabledState a New-AzFrontDoorHealthProbeSettingObject</span><span class="sxs-lookup"><span data-stu-id="c0450-1211">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="c0450-1212">Adição de um novo cmdlet para criar um objeto BackendPoolsSettings para passar para a criação/atualização do Front Door</span><span class="sxs-lookup"><span data-stu-id="c0450-1212">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="c0450-1213">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="c0450-1213">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-1214">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-1214">Az.Network</span></span>
* <span data-ttu-id="c0450-1215">Alteração dos exemplos de opções FilterData de "Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" e "Start-AzVirtualnetworkGatewayPacketCapture.md".</span><span class="sxs-lookup"><span data-stu-id="c0450-1215">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="c0450-1216">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="c0450-1216">Az.PrivateDns</span></span>
* <span data-ttu-id="c0450-1217">Atualização do SDK .NET do PrivateDns para a versão 1.0.0</span><span class="sxs-lookup"><span data-stu-id="c0450-1217">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-1218">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-1218">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-1219">Suporte do Azure Site Recovery para selecionar o tipo de disco ao ativar a proteção.</span><span class="sxs-lookup"><span data-stu-id="c0450-1219">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="c0450-1220">Correção do Azure Site Recovery para a edição de ações do plano de recuperação.</span><span class="sxs-lookup"><span data-stu-id="c0450-1220">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="c0450-1221">Suporte de Restauro de SQL do Azure Backup para aceitar BDs de filestream.</span><span class="sxs-lookup"><span data-stu-id="c0450-1221">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="c0450-1222">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="c0450-1222">Az.RedisCache</span></span>
* <span data-ttu-id="c0450-1223">Adição do parâmetro "MinimumTlsVersion" nos cmdlets "New-AzRedisCache" e "Set-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="c0450-1223">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="c0450-1224">Adição, também, de "MinimumTlsVersion" na saída do cmdlet "Get-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="c0450-1224">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="c0450-1225">Adição da validação no parâmetro "-Size" para os cmdlets "Set-AzRedisCache" e "New-AzRedisCache"</span><span class="sxs-lookup"><span data-stu-id="c0450-1225">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-1226">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-1226">Az.Resources</span></span>
- <span data-ttu-id="c0450-1227">Atualização dos cmdlets de política no sentido de utilizar a nova versão de api 2019-06-01, a qual tem a nova propriedade EnforcementMode na atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="c0450-1227">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="c0450-1228">Atualização do exemplo de ajuda da definição da política de criação</span><span class="sxs-lookup"><span data-stu-id="c0450-1228">Updated create policy definition help example</span></span>
- <span data-ttu-id="c0450-1229">Correção do erro Remove-AZADServicePrincipal -ServicePrincipalName. Apresentação de uma referência nula quando o nome do principal do serviço não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="c0450-1229">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="c0450-1230">Correção do erro New-AZADServicePrincipal. Apresentação de uma referência nula quando o inquilino não tem uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="c0450-1230">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="c0450-1231">Alteração de New-AzAdServicePrincipal para adicionar credenciais apenas a aplicações associadas.</span><span class="sxs-lookup"><span data-stu-id="c0450-1231">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-1232">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-1232">Az.Sql</span></span>
* <span data-ttu-id="c0450-1233">Adição de suporte para a base de dados ReadReplicaCount.</span><span class="sxs-lookup"><span data-stu-id="c0450-1233">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="c0450-1234">Correção de Set-AzSqlDatabase quando a redundância de zona não está definida</span><span class="sxs-lookup"><span data-stu-id="c0450-1234">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="c0450-1235">3.0.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-1235">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="c0450-1236">Geral</span><span class="sxs-lookup"><span data-stu-id="c0450-1236">General</span></span>
* <span data-ttu-id="c0450-1237">Disponibilização do Az.PrivateDns 1.0.0</span><span class="sxs-lookup"><span data-stu-id="c0450-1237">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c0450-1238">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-1238">Az.Accounts</span></span>
* <span data-ttu-id="c0450-1239">Adição de uma mensagem de descontinuação para o alias "Resolve-Error".</span><span class="sxs-lookup"><span data-stu-id="c0450-1239">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="c0450-1240">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="c0450-1240">Az.Advisor</span></span>
* <span data-ttu-id="c0450-1241">Adição da nova categoria "Excelência Operacional" ao cmdlet Get-AzAdvisorRecommendation.</span><span class="sxs-lookup"><span data-stu-id="c0450-1241">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c0450-1242">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c0450-1242">Az.Batch</span></span>
* <span data-ttu-id="c0450-1243">Mudança de nome de `CoreQuota` em `BatchAccountContext` para `DedicatedCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="c0450-1243">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="c0450-1244">Existe também um novo `LowPriorityCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="c0450-1244">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="c0450-1245">Isto afeta **Get-AzBatchAccount**.</span><span class="sxs-lookup"><span data-stu-id="c0450-1245">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="c0450-1246">O parâmetro **New-AzBatchTask** `-ResourceFile` assume agora uma coleção de objetos `PSResourceFile`, os quais podem ser construídos com o novo cmdlet **New-AzBatchResourceFile**.</span><span class="sxs-lookup"><span data-stu-id="c0450-1246">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="c0450-1247">Novo cmdlet **New-AzBatchResourceFile** para ajudar a criar objetos `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="c0450-1247">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="c0450-1248">Estes podem ser fornecidos a **New-AzBatchTask** no parâmetro `-ResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="c0450-1248">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="c0450-1249">Isto suporta dois novos tipos de ficheiro de recursos para além do caminho `HttpUrl` existente:</span><span class="sxs-lookup"><span data-stu-id="c0450-1249">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="c0450-1250">Os ficheiros de recursos baseados em `AutoStorageContainerName` transferem um contentor integral de armazenamento automático para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="c0450-1250">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="c0450-1251">Os ficheiros de recursos baseados em `StorageContainerUrl` transferem o contentor especificado no URL para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="c0450-1251">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="c0450-1252">Remoção da propriedade `ApplicationPackages` de `PSApplication` devolvida por **Get-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="c0450-1252">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="c0450-1253">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com **Get-AzBatchApplicationPackage**.</span><span class="sxs-lookup"><span data-stu-id="c0450-1253">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="c0450-1254">Por exemplo: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span><span class="sxs-lookup"><span data-stu-id="c0450-1254">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="c0450-1255">Mudança de nome de `ApplicationId` para `ApplicationName` em **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication** e **Set-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="c0450-1255">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="c0450-1256">`ApplicationId` é agora um alias de `ApplicationName`.</span><span class="sxs-lookup"><span data-stu-id="c0450-1256">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="c0450-1257">Adição da nova propriedade `PSWindowsUserConfiguration` a `PSUserAccount`.</span><span class="sxs-lookup"><span data-stu-id="c0450-1257">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="c0450-1258">Mudança de nome de `Version` para `Name` em `PSApplicationPackage`.</span><span class="sxs-lookup"><span data-stu-id="c0450-1258">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="c0450-1259">Mudança de nome de `BlobSource` para `HttpUrl` em `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="c0450-1259">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="c0450-1260">Remoção da propriedade `OSDisk` de `PSVirtualMachineConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="c0450-1260">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="c0450-1261">Remoção de **Set-AzBatchPoolOSVersion**.</span><span class="sxs-lookup"><span data-stu-id="c0450-1261">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="c0450-1262">Esta operação deixou de ser suportada.</span><span class="sxs-lookup"><span data-stu-id="c0450-1262">This operation is no longer supported.</span></span>
* <span data-ttu-id="c0450-1263">Remoção de `TargetOSVersion` de `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="c0450-1263">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="c0450-1264">Mudança de nome de `CurrentOSVersion` para `OSVersion` em `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="c0450-1264">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="c0450-1265">Remoção de `DataEgressGiB` e `DataIngressGiB` de `PSPoolUsageMetrics`.</span><span class="sxs-lookup"><span data-stu-id="c0450-1265">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="c0450-1266">Remoção de **Get-AzBatchNodeAgentSku** e substituição deste por **Get-AzBatchSupportedImage**.</span><span class="sxs-lookup"><span data-stu-id="c0450-1266">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span>
  - <span data-ttu-id="c0450-1267">**Get-AzBatchSupportedImage** devolve os mesmos dados de **Get-AzBatchNodeAgentSku**, mas num formato mais acessível.</span><span class="sxs-lookup"><span data-stu-id="c0450-1267">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="c0450-1268">As novas imagens não verificadas agora também são devolvidas.</span><span class="sxs-lookup"><span data-stu-id="c0450-1268">New non-verified images are also now returned.</span></span> <span data-ttu-id="c0450-1269">Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.</span><span class="sxs-lookup"><span data-stu-id="c0450-1269">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="c0450-1270">Adição da capacidade de montagem de sistemas de ficheiros remotos em cada nó de um conjunto através do novo parâmetro `MountConfiguration` de **New-AzBatchPool**.</span><span class="sxs-lookup"><span data-stu-id="c0450-1270">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="c0450-1271">Adição do suporte a regras de segurança de rede que bloqueiam o acesso de rede a um conjunto com base na porta de origem do tráfego.</span><span class="sxs-lookup"><span data-stu-id="c0450-1271">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="c0450-1272">Isto ocorre através da propriedade `SourcePortRanges` em `PSNetworkSecurityGroupRule`.</span><span class="sxs-lookup"><span data-stu-id="c0450-1272">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="c0450-1273">Ao executar um contentor, o Batch agora suporta a execução da tarefa no diretório de trabalho do contentor ou no diretório de trabalho da tarefa do Batch.</span><span class="sxs-lookup"><span data-stu-id="c0450-1273">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="c0450-1274">Isto é controlado pela propriedade `WorkingDirectory` em `PSTaskContainerSettings`.</span><span class="sxs-lookup"><span data-stu-id="c0450-1274">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="c0450-1275">Adição da capacidade de especificar uma coleção de IPs públicos em `PSNetworkConfiguration` através da nova propriedade `PublicIPs`.</span><span class="sxs-lookup"><span data-stu-id="c0450-1275">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="c0450-1276">Isto garante que os nós no Conjunto terão um IP da lista de IPs fornecidos pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="c0450-1276">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="c0450-1277">Quando não for especificado, o valor predefinido de `WaitForSuccess` em `PSSTartTask` é agora `$True` (era `$False`).</span><span class="sxs-lookup"><span data-stu-id="c0450-1277">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="c0450-1278">Quando não for especificado, o valor predefinido de `Scope` em `PSAutoUserSpecification` é agora `Pool` (era `Task` no Windows e `Pool` no Linux).</span><span class="sxs-lookup"><span data-stu-id="c0450-1278">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c0450-1279">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c0450-1279">Az.Cdn</span></span>
* <span data-ttu-id="c0450-1280">Introdução de UrlRewriteAction e CacheKeyQueryStringAction em RulesEngine.</span><span class="sxs-lookup"><span data-stu-id="c0450-1280">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="c0450-1281">Correção de vários erros como a falta da Entrada "Seletor" no cmdlet New-AzDeliveryRuleCondition.</span><span class="sxs-lookup"><span data-stu-id="c0450-1281">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-1282">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-1282">Az.Compute</span></span>
* <span data-ttu-id="c0450-1283">Funcionalidade Conjunto de Encriptação de Discos</span><span class="sxs-lookup"><span data-stu-id="c0450-1283">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="c0450-1284">Novos cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="c0450-1284">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="c0450-1285">Adição do parâmetro DiskEncryptionSetId aos seguintes cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="c0450-1285">DiskEncryptionSetId parameter is added to the following cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="c0450-1286">Adição dos parâmetros DiskEncryptionSetId e EncryptionType aos seguintes cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-1286">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="c0450-1287">Adição do parâmetro PublicIPAddressVersion a New-AzVmssIPConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-1287">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="c0450-1288">Movimentação de FileUris da extensão de script personalizado da definição pública para a definição protegida</span><span class="sxs-lookup"><span data-stu-id="c0450-1288">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="c0450-1289">Adição de ScaleInPolicy aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="c0450-1289">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="c0450-1290">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="c0450-1290">Breaking changes</span></span>
    - <span data-ttu-id="c0450-1291">Utilização do parâmetro UploadSizeInBytes em vez de DiskSizeGB para New-AzDiskConfig quando CreateOption é Carregar</span><span class="sxs-lookup"><span data-stu-id="c0450-1291">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="c0450-1292">Substituição de PublishingProfile.Source.ManagedImage.Id por StorageProfile.Source.Id no objeto GalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="c0450-1292">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c0450-1293">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c0450-1293">Az.DataFactory</span></span>
* <span data-ttu-id="c0450-1294">Atualização da versão do SDK .Net do ADF para 4.3.0</span><span class="sxs-lookup"><span data-stu-id="c0450-1294">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c0450-1295">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c0450-1295">Az.DataLakeStore</span></span>
* <span data-ttu-id="c0450-1296">Atualização da versão do SDK ADLS (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) ) com as seguintes correções</span><span class="sxs-lookup"><span data-stu-id="c0450-1296">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="c0450-1297">Evita a apresentação de uma exceção ao mesmo tempo que não consegue anular a serialização do creationtime do lixo ou da entrada de diretório.</span><span class="sxs-lookup"><span data-stu-id="c0450-1297">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="c0450-1298">Expõe a definição por tempo limite do pedido em adlsclient</span><span class="sxs-lookup"><span data-stu-id="c0450-1298">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="c0450-1299">Correção da passagem do syncflag original para a recuperação de badoffset</span><span class="sxs-lookup"><span data-stu-id="c0450-1299">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="c0450-1300">Correção de EnumerateDirectory para obter o token de continuação após a verificação da resposta</span><span class="sxs-lookup"><span data-stu-id="c0450-1300">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="c0450-1301">Correção do Erro de Concatenação</span><span class="sxs-lookup"><span data-stu-id="c0450-1301">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c0450-1302">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c0450-1302">Az.FrontDoor</span></span>
* <span data-ttu-id="c0450-1303">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="c0450-1303">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c0450-1304">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c0450-1304">Az.HDInsight</span></span>
* <span data-ttu-id="c0450-1305">Correção do erro em que o cliente recebe o erro "Não é uma cadeia Base 64 válida" quando utiliza Get-AzHDInsightCluster para obter o cluster com o armazenamento ADLSGen1.</span><span class="sxs-lookup"><span data-stu-id="c0450-1305">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="c0450-1306">Adição de um parâmetro com o nome "ApplicationId" a três cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig e New-AzHDInsightCluster para que o cliente consiga fornecer o ID da aplicação do principal de serviço que permite aceder ao Azure Data Lake.</span><span class="sxs-lookup"><span data-stu-id="c0450-1306">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="c0450-1307">Alteração de Microsoft.Azure.Management.HDInsight da versão 2.1.0 para a 5.1.0</span><span class="sxs-lookup"><span data-stu-id="c0450-1307">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="c0450-1308">Remoção de cinco cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c0450-1308">Removed five cmdlets:</span></span>
    - <span data-ttu-id="c0450-1309">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="c0450-1309">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="c0450-1310">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="c0450-1310">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="c0450-1311">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="c0450-1311">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="c0450-1312">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="c0450-1312">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="c0450-1313">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="c0450-1313">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="c0450-1314">Adição de três cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c0450-1314">Added three cmdlets:</span></span>
    - <span data-ttu-id="c0450-1315">Get-AzHDInsightMonitoring para substituir Get-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="c0450-1315">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="c0450-1316">Enable-AzHDInsightMonitoring para substituir Enable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="c0450-1316">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="c0450-1317">Disable-AzHDInsightMonitoring para substituir Disable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="c0450-1317">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="c0450-1318">Correção do cmdlet Get-AzHDInsightProperties para suportar a obtenção de informações sobre capacidades de uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="c0450-1318">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="c0450-1319">Remoção de conjuntos de parâmetros("Spark1", "Spark2") de Add-AzHDInsightConfigValue.</span><span class="sxs-lookup"><span data-stu-id="c0450-1319">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="c0450-1320">Adição de exemplos aos documentos de ajuda do cmdlet Add-AzHDInsightSecurityProfile.</span><span class="sxs-lookup"><span data-stu-id="c0450-1320">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="c0450-1321">Alteração do tipo de saída dos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c0450-1321">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="c0450-1322">Alteração do tipo de saída de Get-AzHDInsightProperties de CapabilitiesResponse para AzureHDInsightCapabilities.</span><span class="sxs-lookup"><span data-stu-id="c0450-1322">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="c0450-1323">Alteração do tipo de saída de Remove-AzHDInsightCluster de ClusterGetResponse para booleano.</span><span class="sxs-lookup"><span data-stu-id="c0450-1323">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="c0450-1324">Alteração do tipo de saída de Set-AzHDInsightGatewaySettings de HttpConnectivitySettings para GatewaySettings.</span><span class="sxs-lookup"><span data-stu-id="c0450-1324">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="c0450-1325">Adição de alguns casos de teste de cenários.</span><span class="sxs-lookup"><span data-stu-id="c0450-1325">Added some scenario test cases.</span></span>
* <span data-ttu-id="c0450-1326">Remoção de alguns alias: "Add-AzHDInsightConfigValues", "Get-AzHDInsightProperties".</span><span class="sxs-lookup"><span data-stu-id="c0450-1326">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c0450-1327">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c0450-1327">Az.IotHub</span></span>
* <span data-ttu-id="c0450-1328">Alterações interruptivas:</span><span class="sxs-lookup"><span data-stu-id="c0450-1328">Breaking changes:</span></span>
    - <span data-ttu-id="c0450-1329">O cmdlet "Add-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="c0450-1329">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="c0450-1330">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Add-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="c0450-1330">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="c0450-1331">O cmdlet "Get-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="c0450-1331">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="c0450-1332">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Get-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="c0450-1332">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="c0450-1333">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="c0450-1333">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="c0450-1334">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="c0450-1334">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="c0450-1335">O cmdlet "New-AzIotHubExportDevice" deixou de suportar o alias "New-AzIotHubExportDevices".</span><span class="sxs-lookup"><span data-stu-id="c0450-1335">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="c0450-1336">O cmdlet "New-AzIotHubImportDevice" deixou de suportar o alias "New-AzIotHubImportDevices".</span><span class="sxs-lookup"><span data-stu-id="c0450-1336">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="c0450-1337">O cmdlet "Remove-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="c0450-1337">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="c0450-1338">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Remove-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="c0450-1338">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="c0450-1339">O cmdlet "Set-AzIotHub" deixou de suportar o parâmetro "OperationsMonitoringProperties" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="c0450-1339">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="c0450-1340">O conjunto de parâmetros "UpdateOperationsMonitoringProperties" do cmdlet "Set-AzIotHub" foi removido.</span><span class="sxs-lookup"><span data-stu-id="c0450-1340">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-1341">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-1341">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-1342">Suporte do Azure Site Recovery para configurar recursos de rede como NSG, IP público e balanceadores de carga internos do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-1342">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="c0450-1343">Suporte do Azure Site Recovery para escrever para um disco gerido do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-1343">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="c0450-1344">Suporte do Azure Site Recovery para redução de NIC do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-1344">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="c0450-1345">Suporte do Azure Site Recovery para aceleração de rede do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-1345">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="c0450-1346">Suporte do Azure Site Recovery para a atualização automática do agente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-1346">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="c0450-1347">Suporte do Azure Site Recovery para SSD Standard do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-1347">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="c0450-1348">Suporte do Azure Site Recovery para a codificação em dois passos do Azure Disk Encryption do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-1348">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="c0450-1349">Suporte do Azure Site Recovery para a proteção de um disco adicionado recentemente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-1349">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="c0450-1350">Adição da funcionalidade SoftDelete para VM e de testes para softdelete</span><span class="sxs-lookup"><span data-stu-id="c0450-1350">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-1351">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-1351">Az.Resources</span></span>
* <span data-ttu-id="c0450-1352">Atualização da assemblagem de dependências Microsoft.Extensions.Caching.Memory da versão 1.1.1 para a 2.2</span><span class="sxs-lookup"><span data-stu-id="c0450-1352">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-1353">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-1353">Az.Network</span></span>
* <span data-ttu-id="c0450-1354">Alteração de todos os cmdlets para PrivateEndpointConnection para suportar o fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="c0450-1354">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="c0450-1355">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="c0450-1355">Updated cmdlet:</span></span>
        - <span data-ttu-id="c0450-1356">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-1356">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c0450-1357">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-1357">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c0450-1358">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-1358">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c0450-1359">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-1359">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c0450-1360">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-1360">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="c0450-1361">Adição de novo cmdlet para PrivateLinkResource também com suporte de fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="c0450-1361">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="c0450-1362">Novo cmdlet:</span><span class="sxs-lookup"><span data-stu-id="c0450-1362">New cmdlet:</span></span>
        - <span data-ttu-id="c0450-1363">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="c0450-1363">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="c0450-1364">Adição de novos campos e parâmetro para a funcionalidade Protocolo de Proxy V2.</span><span class="sxs-lookup"><span data-stu-id="c0450-1364">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="c0450-1365">Adição da propriedade EnableProxyProtocol em PrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="c0450-1365">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="c0450-1366">Adição da propriedade LinkIdentifier em PrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-1366">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="c0450-1367">Atualização de New-AzPrivateLinkService para adicionar um novo parâmetro adicional EnableProxyProtocol.</span><span class="sxs-lookup"><span data-stu-id="c0450-1367">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="c0450-1368">Correção da descrição incorreta do parâmetro na documentação de referência "New-AzApplicationGatewaySku"</span><span class="sxs-lookup"><span data-stu-id="c0450-1368">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="c0450-1369">Novos cmdlets para suportar a política de firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="c0450-1369">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="c0450-1370">Adição de suporte para o recurso subordinado RouteTables de VirtualHub</span><span class="sxs-lookup"><span data-stu-id="c0450-1370">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="c0450-1371">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c0450-1371">New cmdlets added:</span></span>
        - <span data-ttu-id="c0450-1372">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="c0450-1372">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="c0450-1373">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="c0450-1373">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="c0450-1374">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="c0450-1374">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="c0450-1375">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="c0450-1375">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="c0450-1376">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="c0450-1376">Set-AzVirtualHub</span></span>
* <span data-ttu-id="c0450-1377">Adição de suporte para o SKU de novas propriedades de VirtualHub e VirtualWANType de VirtualWan</span><span class="sxs-lookup"><span data-stu-id="c0450-1377">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="c0450-1378">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="c0450-1378">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="c0450-1379">New-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="c0450-1379">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="c0450-1380">Update-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="c0450-1380">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="c0450-1381">New-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="c0450-1381">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="c0450-1382">Update-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="c0450-1382">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="c0450-1383">Adição de suporte para a propriedade EnableInternetSecurity para HubVnetConnection, VpnConnection e ExpressRouteConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-1383">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="c0450-1384">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c0450-1384">New cmdlets added:</span></span>
        - <span data-ttu-id="c0450-1385">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-1385">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="c0450-1386">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="c0450-1386">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="c0450-1387">New-AzureRmVirtualHubVnetConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="c0450-1387">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="c0450-1388">New-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="c0450-1388">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="c0450-1389">Update-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="c0450-1389">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="c0450-1390">New-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="c0450-1390">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="c0450-1391">Set-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="c0450-1391">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="c0450-1392">Adição de suporte para Configurar a Política WebApplicationFirewall de Nível Superior</span><span class="sxs-lookup"><span data-stu-id="c0450-1392">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="c0450-1393">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c0450-1393">New cmdlets added:</span></span>
        - <span data-ttu-id="c0450-1394">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="c0450-1394">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="c0450-1395">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="c0450-1395">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="c0450-1396">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="c0450-1396">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="c0450-1397">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="c0450-1397">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="c0450-1398">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="c0450-1398">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="c0450-1399">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="c0450-1399">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="c0450-1400">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="c0450-1400">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="c0450-1401">New-AzApplicationGatewayFirewallPolicy : adição do parâmetro PolicySetting, ManagedRule</span><span class="sxs-lookup"><span data-stu-id="c0450-1401">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="c0450-1402">Adição de suporte para o operador GeoMatch em CustomRule</span><span class="sxs-lookup"><span data-stu-id="c0450-1402">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="c0450-1403">Adição de GeoMatch ao operador em FirewallCondition</span><span class="sxs-lookup"><span data-stu-id="c0450-1403">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="c0450-1404">Adição de suporte para a Política de firewall perListener e perSite</span><span class="sxs-lookup"><span data-stu-id="c0450-1404">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="c0450-1405">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="c0450-1405">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="c0450-1406">New-AzApplicationGatewayHttpListener : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="c0450-1406">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="c0450-1407">New-AzApplicationGatewayPathRuleConfig : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="c0450-1407">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="c0450-1408">Correção da sub-rede necessária com o nome AzureBastionSubnet em "PSBastion" pode não ser sensível às maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="c0450-1408">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="c0450-1409">Suporte para FQDNs de Destino nas Regras de Rede e para FQDN Traduzido em Regras NAT para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="c0450-1409">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="c0450-1410">Adição de suporte para o recurso de nível superior RouteTables de IpGroup</span><span class="sxs-lookup"><span data-stu-id="c0450-1410">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="c0450-1411">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c0450-1411">New cmdlets added:</span></span>
        - <span data-ttu-id="c0450-1412">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="c0450-1412">New-AzIpGroup</span></span>
        - <span data-ttu-id="c0450-1413">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="c0450-1413">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="c0450-1414">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="c0450-1414">Get-AzIpGroup</span></span>
        - <span data-ttu-id="c0450-1415">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="c0450-1415">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c0450-1416">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c0450-1416">Az.ServiceFabric</span></span>
* <span data-ttu-id="c0450-1417">Remoção do cmdlet Add-AzServiceFabricApplicationCertificate uma vez que este cenário é abrangido por Add-AzVmssSecret.</span><span class="sxs-lookup"><span data-stu-id="c0450-1417">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-1418">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-1418">Az.Sql</span></span>
* <span data-ttu-id="c0450-1419">Adição de suporte para o restauro de bases de dados removidas em Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="c0450-1419">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="c0450-1420">Descontinuação dos cmdlets de auditoria antigos do código.</span><span class="sxs-lookup"><span data-stu-id="c0450-1420">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="c0450-1421">Remoção de aliases descontinuados:</span><span class="sxs-lookup"><span data-stu-id="c0450-1421">Removed deprecated aliases:</span></span>
* <span data-ttu-id="c0450-1422">Get-AzSqlDatabaseIndexRecommendations (utilize antes Get-AzSqlDatabaseIndexRecommendation)</span><span class="sxs-lookup"><span data-stu-id="c0450-1422">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="c0450-1423">Get-AzSqlDatabaseRestorePoints (utilize antes Get-AzSqlDatabaseRestorePoint)</span><span class="sxs-lookup"><span data-stu-id="c0450-1423">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="c0450-1424">Remoção do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c0450-1424">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="c0450-1425">Remoção dos aliases dos cmdlets descontinuados das Definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="c0450-1425">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="c0450-1426">Descontinuação dos cmdlets das Definições de Deteção Avançada de Ameaças</span><span class="sxs-lookup"><span data-stu-id="c0450-1426">Deprecate Advanced Threat Detection Settings cmdlets</span></span>
* <span data-ttu-id="c0450-1427">Adição de cmdlets para Desativar e Ativar as recomendações de sensibilidade nas colunas de uma base de dados.</span><span class="sxs-lookup"><span data-stu-id="c0450-1427">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-1428">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-1428">Az.Storage</span></span>
* <span data-ttu-id="c0450-1429">Suporte à ativação da partilha de Ficheiros de Grandes Dimensões ao criar ou atualizar uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="c0450-1429">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="c0450-1430">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c0450-1430">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="c0450-1431">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c0450-1431">Set-AzStorageAccount</span></span>
* <span data-ttu-id="c0450-1432">Ao fechar/obter o Identificador de ficheiro, ignorar a verificação do caminho de entrada corresponde a Diretório de ficheiros ou Ficheiro, de forma a evitar a falha com o objeto no estado DeletePending</span><span class="sxs-lookup"><span data-stu-id="c0450-1432">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="c0450-1433">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="c0450-1433">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="c0450-1434">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="c0450-1434">Close-AzStorageFileHandle</span></span>

## <a name="280---october-2019"></a><span data-ttu-id="c0450-1435">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-1435">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="c0450-1436">Geral</span><span class="sxs-lookup"><span data-stu-id="c0450-1436">General</span></span>
* <span data-ttu-id="c0450-1437">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="c0450-1437">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c0450-1438">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-1438">Az.Accounts</span></span>
* <span data-ttu-id="c0450-1439">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="c0450-1439">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c0450-1440">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c0450-1440">Az.ApiManagement</span></span>
* <span data-ttu-id="c0450-1441">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="c0450-1441">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="c0450-1442">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="c0450-1442">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c0450-1443">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c0450-1443">Az.Automation</span></span>
* <span data-ttu-id="c0450-1444">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="c0450-1444">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c0450-1445">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c0450-1445">Az.Batch</span></span>
* <span data-ttu-id="c0450-1446">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="c0450-1446">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-1447">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-1447">Az.Compute</span></span>
* <span data-ttu-id="c0450-1448">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="c0450-1448">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="c0450-1449">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="c0450-1449">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="c0450-1450">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="c0450-1450">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span>
* <span data-ttu-id="c0450-1451">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="c0450-1451">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c0450-1452">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c0450-1452">Az.DataFactory</span></span>
* <span data-ttu-id="c0450-1453">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="c0450-1453">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="c0450-1454">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="c0450-1454">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="c0450-1455">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="c0450-1455">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c0450-1456">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c0450-1456">Az.DataLakeStore</span></span>
* <span data-ttu-id="c0450-1457">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="c0450-1457">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="c0450-1458">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="c0450-1458">Az.HealthcareApis</span></span>
* <span data-ttu-id="c0450-1459">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="c0450-1459">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="c0450-1460">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="c0450-1460">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="c0450-1461">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="c0450-1461">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="c0450-1462">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="c0450-1462">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c0450-1463">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c0450-1463">Az.IotHub</span></span>
* <span data-ttu-id="c0450-1464">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="c0450-1464">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="c0450-1465">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="c0450-1465">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c0450-1466">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c0450-1466">Az.Monitor</span></span>
* <span data-ttu-id="c0450-1467">Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="c0450-1467">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="c0450-1468">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="c0450-1468">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="c0450-1469">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="c0450-1469">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="c0450-1470">Os Webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c0450-1470">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-1471">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-1471">Az.Network</span></span>
* <span data-ttu-id="c0450-1472">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="c0450-1472">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="c0450-1473">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="c0450-1473">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="c0450-1474">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c0450-1474">New cmdlets added:</span></span>
        - <span data-ttu-id="c0450-1475">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="c0450-1475">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="c0450-1476">Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-1476">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="c0450-1477">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="c0450-1477">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="c0450-1478">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="c0450-1478">Updated cmdlets:</span></span>
        - <span data-ttu-id="c0450-1479">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-1479">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="c0450-1480">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-1480">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="c0450-1481">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-1481">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="c0450-1482">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="c0450-1482">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="c0450-1483">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="c0450-1483">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="c0450-1484">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="c0450-1484">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="c0450-1485">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="c0450-1485">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="c0450-1486">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="c0450-1486">Az.RedisCache</span></span>
* <span data-ttu-id="c0450-1487">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="c0450-1487">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-1488">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-1488">Az.Sql</span></span>
* <span data-ttu-id="c0450-1489">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="c0450-1489">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-1490">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-1490">Az.Storage</span></span>
* <span data-ttu-id="c0450-1491">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="c0450-1491">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="c0450-1492">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="c0450-1492">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="c0450-1493">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="c0450-1493">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="c0450-1494">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="c0450-1494">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="c0450-1495">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c0450-1495">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="c0450-1496">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="c0450-1496">Az.StorageSync</span></span>
* <span data-ttu-id="c0450-1497">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="c0450-1497">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c0450-1498">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-1498">Az.Websites</span></span>
* <span data-ttu-id="c0450-1499">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="c0450-1499">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="c0450-1500">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-1500">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="c0450-1501">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c0450-1501">Az.ApiManagement</span></span>
* <span data-ttu-id="c0450-1502">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="c0450-1502">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="c0450-1503">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="c0450-1503">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="c0450-1504">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="c0450-1504">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c0450-1505">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c0450-1505">Az.Automation</span></span>
* <span data-ttu-id="c0450-1506">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="c0450-1506">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="c0450-1507">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="c0450-1507">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="c0450-1508">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="c0450-1508">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-1509">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-1509">Az.Compute</span></span>
* <span data-ttu-id="c0450-1510">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-1510">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="c0450-1511">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-1511">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="c0450-1512">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="c0450-1512">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="c0450-1513">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="c0450-1513">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="c0450-1514">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="c0450-1514">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="c0450-1515">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="c0450-1515">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="c0450-1516">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="c0450-1516">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="c0450-1517">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="c0450-1517">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="c0450-1518">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="c0450-1518">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c0450-1519">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c0450-1519">Az.DataFactory</span></span>
* <span data-ttu-id="c0450-1520">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="c0450-1520">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="c0450-1521">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="c0450-1521">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c0450-1522">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c0450-1522">Az.HDInsight</span></span>
* <span data-ttu-id="c0450-1523">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="c0450-1523">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c0450-1524">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c0450-1524">Az.IotHub</span></span>
* <span data-ttu-id="c0450-1525">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="c0450-1525">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="c0450-1526">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="c0450-1526">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="c0450-1527">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="c0450-1527">New cmdlets are:</span></span>
    - <span data-ttu-id="c0450-1528">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="c0450-1528">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="c0450-1529">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="c0450-1529">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="c0450-1530">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="c0450-1530">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="c0450-1531">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="c0450-1531">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c0450-1532">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c0450-1532">Az.Monitor</span></span>
* <span data-ttu-id="c0450-1533">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="c0450-1533">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="c0450-1534">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="c0450-1534">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="c0450-1535">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="c0450-1535">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="c0450-1536">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="c0450-1536">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="c0450-1537">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="c0450-1537">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="c0450-1538">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="c0450-1538">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="c0450-1539">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="c0450-1539">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="c0450-1540">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="c0450-1540">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="c0450-1541">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="c0450-1541">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="c0450-1542">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="c0450-1542">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="c0450-1543">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="c0450-1543">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="c0450-1544">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="c0450-1544">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="c0450-1545">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="c0450-1545">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="c0450-1546">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="c0450-1546">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="c0450-1547">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="c0450-1547">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="c0450-1548">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="c0450-1548">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="c0450-1549">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="c0450-1549">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="c0450-1550">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="c0450-1550">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="c0450-1551">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="c0450-1551">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="c0450-1552">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="c0450-1552">Overall improved help files</span></span>
* <span data-ttu-id="c0450-1553">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="c0450-1553">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-1554">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-1554">Az.Network</span></span>
* <span data-ttu-id="c0450-1555">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="c0450-1555">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span>
* <span data-ttu-id="c0450-1556">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="c0450-1556">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="c0450-1557">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="c0450-1557">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="c0450-1558">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="c0450-1558">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="c0450-1559">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="c0450-1559">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="c0450-1560">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="c0450-1560">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="c0450-1561">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="c0450-1561">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="c0450-1562">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="c0450-1562">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="c0450-1563">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0450-1563">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="c0450-1564">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="c0450-1564">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="c0450-1565">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="c0450-1565">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="c0450-1566">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="c0450-1566">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="c0450-1567">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="c0450-1567">New cmdlets</span></span>
        - <span data-ttu-id="c0450-1568">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="c0450-1568">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="c0450-1569">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-1569">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="c0450-1570">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="c0450-1570">Updated cmdlet:</span></span>
        - <span data-ttu-id="c0450-1571">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="c0450-1571">New-VpnSite</span></span>
        - <span data-ttu-id="c0450-1572">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="c0450-1572">Update-VpnSite</span></span>
        - <span data-ttu-id="c0450-1573">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-1573">New-VpnConnection</span></span>
        - <span data-ttu-id="c0450-1574">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-1574">Update-VpnConnection</span></span>
* <span data-ttu-id="c0450-1575">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="c0450-1575">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-1576">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-1576">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-1577">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="c0450-1577">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="c0450-1578">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="c0450-1578">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-1579">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-1579">Az.Resources</span></span>
* <span data-ttu-id="c0450-1580">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="c0450-1580">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c0450-1581">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c0450-1581">Az.ServiceFabric</span></span>
* <span data-ttu-id="c0450-1582">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="c0450-1582">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="c0450-1583">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="c0450-1583">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="c0450-1584">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="c0450-1584">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="c0450-1585">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="c0450-1585">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="c0450-1586">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="c0450-1586">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="c0450-1587">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="c0450-1587">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="c0450-1588">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="c0450-1588">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="c0450-1589">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="c0450-1589">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="c0450-1590">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="c0450-1590">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="c0450-1591">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="c0450-1591">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="c0450-1592">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="c0450-1592">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="c0450-1593">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="c0450-1593">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="c0450-1594">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="c0450-1594">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="c0450-1595">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="c0450-1595">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="c0450-1596">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="c0450-1596">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="c0450-1597">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="c0450-1597">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="c0450-1598">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="c0450-1598">Az.SignalR</span></span>
* <span data-ttu-id="c0450-1599">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="c0450-1599">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-1600">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-1600">Az.Sql</span></span>
* <span data-ttu-id="c0450-1601">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="c0450-1601">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="c0450-1602">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="c0450-1602">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="c0450-1603">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c0450-1603">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="c0450-1604">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="c0450-1604">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="c0450-1605">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="c0450-1605">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-1606">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-1606">Az.Storage</span></span>
* <span data-ttu-id="c0450-1607">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="c0450-1607">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="c0450-1608">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="c0450-1608">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="c0450-1609">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="c0450-1609">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="c0450-1610">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="c0450-1610">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="c0450-1611">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="c0450-1611">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="c0450-1612">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="c0450-1612">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="c0450-1613">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="c0450-1613">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="c0450-1614">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="c0450-1614">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="c0450-1615">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="c0450-1615">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="c0450-1616">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="c0450-1616">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="c0450-1617">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="c0450-1617">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c0450-1618">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-1618">Az.Websites</span></span>
* <span data-ttu-id="c0450-1619">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="c0450-1619">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="c0450-1620">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="c0450-1620">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="c0450-1621">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="c0450-1621">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="c0450-1622">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-1622">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="c0450-1623">Geral</span><span class="sxs-lookup"><span data-stu-id="c0450-1623">General</span></span>
* <span data-ttu-id="c0450-1624">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="c0450-1624">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c0450-1625">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-1625">Az.Accounts</span></span>
* <span data-ttu-id="c0450-1626">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="c0450-1626">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="c0450-1627">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="c0450-1627">Az.Aks</span></span>
* <span data-ttu-id="c0450-1628">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="c0450-1628">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="c0450-1629">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="c0450-1629">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c0450-1630">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c0450-1630">Az.ApiManagement</span></span>
* <span data-ttu-id="c0450-1631">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="c0450-1631">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="c0450-1632">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="c0450-1632">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="c0450-1633">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="c0450-1633">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="c0450-1634">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="c0450-1634">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="c0450-1635">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="c0450-1635">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c0450-1636">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c0450-1636">Az.Batch</span></span>
* <span data-ttu-id="c0450-1637">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="c0450-1637">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c0450-1638">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c0450-1638">Az.Cdn</span></span>
* <span data-ttu-id="c0450-1639">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="c0450-1639">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-1640">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-1640">Az.Compute</span></span>
* <span data-ttu-id="c0450-1641">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-1641">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="c0450-1642">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="c0450-1642">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="c0450-1643">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="c0450-1643">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="c0450-1644">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="c0450-1644">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="c0450-1645">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="c0450-1645">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="c0450-1646">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="c0450-1646">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="c0450-1647">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="c0450-1647">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="c0450-1648">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="c0450-1648">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c0450-1649">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c0450-1649">Az.DataFactory</span></span>
* <span data-ttu-id="c0450-1650">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="c0450-1650">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="c0450-1651">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="c0450-1651">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="c0450-1652">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="c0450-1652">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="c0450-1653">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="c0450-1653">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c0450-1654">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c0450-1654">Az.DataLakeStore</span></span>
* <span data-ttu-id="c0450-1655">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="c0450-1655">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c0450-1656">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c0450-1656">Az.EventHub</span></span>
* <span data-ttu-id="c0450-1657">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="c0450-1657">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="c0450-1658">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="c0450-1658">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="c0450-1659">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="c0450-1659">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="c0450-1660">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="c0450-1660">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="c0450-1661">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="c0450-1661">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="c0450-1662">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="c0450-1662">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c0450-1663">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c0450-1663">Az.Monitor</span></span>
* <span data-ttu-id="c0450-1664">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="c0450-1664">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-1665">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-1665">Az.Network</span></span>
* <span data-ttu-id="c0450-1666">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="c0450-1666">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="c0450-1667">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="c0450-1667">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="c0450-1668">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="c0450-1668">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="c0450-1669">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="c0450-1669">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="c0450-1670">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="c0450-1670">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span>
* <span data-ttu-id="c0450-1671">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="c0450-1671">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="c0450-1672">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="c0450-1672">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c0450-1673">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-1673">Az.OperationalInsights</span></span>
* <span data-ttu-id="c0450-1674">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="c0450-1674">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="c0450-1675">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="c0450-1675">Added example</span></span>
    - <span data-ttu-id="c0450-1676">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="c0450-1676">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="c0450-1677">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="c0450-1677">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="c0450-1678">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="c0450-1678">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-1679">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-1679">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-1680">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="c0450-1680">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-1681">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-1681">Az.Resources</span></span>
* <span data-ttu-id="c0450-1682">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="c0450-1682">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="c0450-1683">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="c0450-1683">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="c0450-1684">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="c0450-1684">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="c0450-1685">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="c0450-1685">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="c0450-1686">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c0450-1686">Az.ServiceBus</span></span>
* <span data-ttu-id="c0450-1687">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="c0450-1687">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="c0450-1688">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="c0450-1688">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="c0450-1689">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="c0450-1689">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c0450-1690">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c0450-1690">Az.ServiceFabric</span></span>
* <span data-ttu-id="c0450-1691">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="c0450-1691">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="c0450-1692">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="c0450-1692">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="c0450-1693">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="c0450-1693">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="c0450-1694">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="c0450-1694">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="c0450-1695">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="c0450-1695">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="c0450-1696">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="c0450-1696">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-1697">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-1697">Az.Sql</span></span>
* <span data-ttu-id="c0450-1698">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="c0450-1698">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-1699">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-1699">Az.Storage</span></span>
* <span data-ttu-id="c0450-1700">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="c0450-1700">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="c0450-1701">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="c0450-1701">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="c0450-1702">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="c0450-1702">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="c0450-1703">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="c0450-1703">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="c0450-1704">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="c0450-1704">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="c0450-1705">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="c0450-1705">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c0450-1706">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-1706">Az.Websites</span></span>
* <span data-ttu-id="c0450-1707">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="c0450-1707">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="c0450-1708">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-1708">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c0450-1709">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-1709">Az.Accounts</span></span>
* <span data-ttu-id="c0450-1710">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="c0450-1710">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="c0450-1711">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-1711">Az.ApplicationInsights</span></span>
* <span data-ttu-id="c0450-1712">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="c0450-1712">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c0450-1713">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c0450-1713">Az.Automation</span></span>
* <span data-ttu-id="c0450-1714">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="c0450-1714">Fix typo in resource string</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c0450-1715">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c0450-1715">Az.CognitiveServices</span></span>
* <span data-ttu-id="c0450-1716">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="c0450-1716">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-1717">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-1717">Az.Compute</span></span>
* <span data-ttu-id="c0450-1718">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="c0450-1718">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="c0450-1719">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="c0450-1719">Az.ContainerRegistry</span></span>
* <span data-ttu-id="c0450-1720">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="c0450-1720">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="c0450-1721">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="c0450-1721">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c0450-1722">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c0450-1722">Az.DataFactory</span></span>
* <span data-ttu-id="c0450-1723">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="c0450-1723">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="c0450-1724">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="c0450-1724">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c0450-1725">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c0450-1725">Az.EventHub</span></span>
* <span data-ttu-id="c0450-1726">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="c0450-1726">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="c0450-1727">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="c0450-1727">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c0450-1728">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0450-1728">Az.KeyVault</span></span>
* <span data-ttu-id="c0450-1729">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="c0450-1729">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="c0450-1730">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="c0450-1730">Az.LogicApp</span></span>
* <span data-ttu-id="c0450-1731">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="c0450-1731">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="c0450-1732">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="c0450-1732">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="c0450-1733">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="c0450-1733">Az.ManagedServices</span></span>
* <span data-ttu-id="c0450-1734">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="c0450-1734">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-1735">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-1735">Az.Network</span></span>
* <span data-ttu-id="c0450-1736">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="c0450-1736">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="c0450-1737">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="c0450-1737">New cmdlets</span></span>
        - <span data-ttu-id="c0450-1738">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="c0450-1738">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="c0450-1739">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="c0450-1739">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="c0450-1740">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-1740">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c0450-1741">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-1741">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c0450-1742">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-1742">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c0450-1743">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-1743">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c0450-1744">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="c0450-1744">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="c0450-1745">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="c0450-1745">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="c0450-1746">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="c0450-1746">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="c0450-1747">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-1747">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="c0450-1748">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="c0450-1748">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="c0450-1749">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="c0450-1749">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="c0450-1750">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="c0450-1750">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="c0450-1751">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="c0450-1751">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="c0450-1752">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="c0450-1752">Updated cmdlets</span></span>
        - <span data-ttu-id="c0450-1753">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-1753">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="c0450-1754">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-1754">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="c0450-1755">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-1755">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="c0450-1756">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-1756">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="c0450-1757">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0450-1757">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="c0450-1758">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="c0450-1758">Updated cmdlet:</span></span>
        - <span data-ttu-id="c0450-1759">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-1759">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="c0450-1760">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-1760">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="c0450-1761">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-1761">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="c0450-1762">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="c0450-1762">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="c0450-1763">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="c0450-1763">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="c0450-1764">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="c0450-1764">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c0450-1765">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-1765">Az.OperationalInsights</span></span>
* <span data-ttu-id="c0450-1766">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="c0450-1766">Updated default version for saved searches to be 1.</span></span>
* <span data-ttu-id="c0450-1767">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="c0450-1767">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-1768">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-1768">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-1769">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="c0450-1769">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="c0450-1770">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="c0450-1770">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="c0450-1771">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="c0450-1771">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="c0450-1772">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="c0450-1772">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="c0450-1773">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="c0450-1773">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="c0450-1774">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="c0450-1774">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="c0450-1775">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="c0450-1775">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="c0450-1776">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="c0450-1776">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="c0450-1777">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="c0450-1777">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="c0450-1778">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="c0450-1778">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-1779">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-1779">Az.Resources</span></span>
- <span data-ttu-id="c0450-1780">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="c0450-1780">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="c0450-1781">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="c0450-1781">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="c0450-1782">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c0450-1782">Az.ServiceBus</span></span>
* <span data-ttu-id="c0450-1783">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="c0450-1783">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="c0450-1784">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="c0450-1784">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-1785">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-1785">Az.Sql</span></span>
* <span data-ttu-id="c0450-1786">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="c0450-1786">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="c0450-1787">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="c0450-1787">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="c0450-1788">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="c0450-1788">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-1789">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-1789">Az.Storage</span></span>
* <span data-ttu-id="c0450-1790">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="c0450-1790">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="c0450-1791">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="c0450-1791">Az.StorageSync</span></span>
* <span data-ttu-id="c0450-1792">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="c0450-1792">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="c0450-1793">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="c0450-1793">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c0450-1794">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-1794">Az.Websites</span></span>
* <span data-ttu-id="c0450-1795">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="c0450-1795">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="c0450-1796">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="c0450-1796">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="c0450-1797">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="c0450-1797">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="c0450-1798">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-1798">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c0450-1799">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-1799">Az.Accounts</span></span>
* <span data-ttu-id="c0450-1800">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="c0450-1800">Add support for profile cmdlets</span></span>
* <span data-ttu-id="c0450-1801">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="c0450-1801">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="c0450-1802">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="c0450-1802">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="c0450-1803">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="c0450-1803">Az.Advisor</span></span>
* <span data-ttu-id="c0450-1804">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="c0450-1804">GA release of Az.Advisor</span></span>
* <span data-ttu-id="c0450-1805">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="c0450-1805">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c0450-1806">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c0450-1806">Az.ApiManagement</span></span>
* <span data-ttu-id="c0450-1807">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="c0450-1807">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="c0450-1808">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="c0450-1808">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="c0450-1809">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="c0450-1809">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="c0450-1810">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="c0450-1810">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="c0450-1811">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="c0450-1811">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="c0450-1812">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="c0450-1812">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="c0450-1813">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="c0450-1813">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c0450-1814">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c0450-1814">Az.Automation</span></span>
* <span data-ttu-id="c0450-1815">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="c0450-1815">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-1816">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-1816">Az.Compute</span></span>
* <span data-ttu-id="c0450-1817">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-1817">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c0450-1818">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c0450-1818">Az.DataFactory</span></span>
* <span data-ttu-id="c0450-1819">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="c0450-1819">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="c0450-1820">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c0450-1820">Az.EventGrid</span></span>
* <span data-ttu-id="c0450-1821">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="c0450-1821">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c0450-1822">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c0450-1822">Az.IotHub</span></span>
* <span data-ttu-id="c0450-1823">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="c0450-1823">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-1824">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-1824">Az.Network</span></span>
* <span data-ttu-id="c0450-1825">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="c0450-1825">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="c0450-1826">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="c0450-1826">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c0450-1827">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-1827">Az.PolicyInsights</span></span>
* <span data-ttu-id="c0450-1828">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="c0450-1828">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="c0450-1829">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="c0450-1829">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c0450-1830">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-1830">Az.OperationalInsights</span></span>
* <span data-ttu-id="c0450-1831">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="c0450-1831">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-1832">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-1832">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-1833">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="c0450-1833">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-1834">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-1834">Az.Resources</span></span>
    - <span data-ttu-id="c0450-1835">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="c0450-1835">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="c0450-1836">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="c0450-1836">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="c0450-1837">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="c0450-1837">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="c0450-1838">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="c0450-1838">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="c0450-1839">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c0450-1839">Az.ServiceBus</span></span>
* <span data-ttu-id="c0450-1840">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="c0450-1840">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-1841">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-1841">Az.Sql</span></span>
* <span data-ttu-id="c0450-1842">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="c0450-1842">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="c0450-1843">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="c0450-1843">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="c0450-1844">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="c0450-1844">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="c0450-1845">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="c0450-1845">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="c0450-1846">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="c0450-1846">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="c0450-1847">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="c0450-1847">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="c0450-1848">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="c0450-1848">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="c0450-1849">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="c0450-1849">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="c0450-1850">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="c0450-1850">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-1851">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-1851">Az.Storage</span></span>
* <span data-ttu-id="c0450-1852">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="c0450-1852">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="c0450-1853">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="c0450-1853">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="c0450-1854">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="c0450-1854">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="c0450-1855">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="c0450-1855">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="c0450-1856">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="c0450-1856">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="c0450-1857">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c0450-1857">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="c0450-1858">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c0450-1858">Set-AzStorageAccount</span></span>
* <span data-ttu-id="c0450-1859">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="c0450-1859">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="c0450-1860">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="c0450-1860">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="c0450-1861">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="c0450-1861">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="c0450-1862">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="c0450-1862">Az.StorageSync</span></span>
* <span data-ttu-id="c0450-1863">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="c0450-1863">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="c0450-1864">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-1864">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c0450-1865">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-1865">Az.Accounts</span></span>
* <span data-ttu-id="c0450-1866">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="c0450-1866">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="c0450-1867">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="c0450-1867">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="c0450-1868">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="c0450-1868">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="c0450-1869">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="c0450-1869">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="c0450-1870">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="c0450-1870">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-1871">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-1871">Az.Compute</span></span>
* <span data-ttu-id="c0450-1872">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="c0450-1872">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="c0450-1873">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="c0450-1873">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="c0450-1874">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="c0450-1874">Az.Dns</span></span>
* <span data-ttu-id="c0450-1875">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="c0450-1875">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="c0450-1876">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c0450-1876">Az.EventGrid</span></span>
* <span data-ttu-id="c0450-1877">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="c0450-1877">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="c0450-1878">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c0450-1878">New cmdlets:</span></span>
    - <span data-ttu-id="c0450-1879">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="c0450-1879">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="c0450-1880">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="c0450-1880">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="c0450-1881">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="c0450-1881">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="c0450-1882">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-1882">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="c0450-1883">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="c0450-1883">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="c0450-1884">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="c0450-1884">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="c0450-1885">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="c0450-1885">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="c0450-1886">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="c0450-1886">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="c0450-1887">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="c0450-1887">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="c0450-1888">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="c0450-1888">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="c0450-1889">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="c0450-1889">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="c0450-1890">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="c0450-1890">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="c0450-1891">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="c0450-1891">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="c0450-1892">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="c0450-1892">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span>
    - <span data-ttu-id="c0450-1893">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="c0450-1893">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="c0450-1894">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="c0450-1894">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="c0450-1895">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="c0450-1895">Updated cmdlets:</span></span>
    - <span data-ttu-id="c0450-1896">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="c0450-1896">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="c0450-1897">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="c0450-1897">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="c0450-1898">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="c0450-1898">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="c0450-1899">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="c0450-1899">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="c0450-1900">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="c0450-1900">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="c0450-1901">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="c0450-1901">Event subscription expiration date,</span></span>
            - <span data-ttu-id="c0450-1902">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="c0450-1902">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="c0450-1903">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="c0450-1903">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="c0450-1904">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="c0450-1904">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span>
    - <span data-ttu-id="c0450-1905">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="c0450-1905">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="c0450-1906">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="c0450-1906">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="c0450-1907">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="c0450-1907">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="c0450-1908">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="c0450-1908">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="c0450-1909">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="c0450-1909">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c0450-1910">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c0450-1910">Az.FrontDoor</span></span>
* <span data-ttu-id="c0450-1911">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="c0450-1911">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="c0450-1912">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="c0450-1912">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="c0450-1913">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="c0450-1913">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="c0450-1914">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="c0450-1914">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-1915">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-1915">Az.Network</span></span>
* <span data-ttu-id="c0450-1916">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="c0450-1916">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="c0450-1917">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="c0450-1917">New cmdlets</span></span>
        - <span data-ttu-id="c0450-1918">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="c0450-1918">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="c0450-1919">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="c0450-1919">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="c0450-1920">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="c0450-1920">New cmdlets</span></span>
        - <span data-ttu-id="c0450-1921">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="c0450-1921">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="c0450-1922">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="c0450-1922">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="c0450-1923">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="c0450-1923">New cmdlets</span></span>
        - <span data-ttu-id="c0450-1924">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="c0450-1924">Get-AzPrivateLinkService</span></span>
        - <span data-ttu-id="c0450-1925">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="c0450-1925">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="c0450-1926">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="c0450-1926">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="c0450-1927">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-1927">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="c0450-1928">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-1928">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="c0450-1929">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="c0450-1929">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="c0450-1930">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="c0450-1930">New cmdlets</span></span>
        - <span data-ttu-id="c0450-1931">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="c0450-1931">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="c0450-1932">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="c0450-1932">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="c0450-1933">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="c0450-1933">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="c0450-1934">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-1934">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="c0450-1935">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="c0450-1935">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="c0450-1936">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="c0450-1936">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="c0450-1937">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="c0450-1937">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="c0450-1938">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="c0450-1938">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="c0450-1939">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="c0450-1939">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="c0450-1940">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="c0450-1940">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="c0450-1941">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0450-1941">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="c0450-1942">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="c0450-1942">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="c0450-1943">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0450-1943">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="c0450-1944">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="c0450-1944">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="c0450-1945">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="c0450-1945">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="c0450-1946">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="c0450-1946">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="c0450-1947">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="c0450-1947">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="c0450-1948">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="c0450-1948">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="c0450-1949">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="c0450-1949">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="c0450-1950">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="c0450-1950">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="c0450-1951">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="c0450-1951">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="c0450-1952">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="c0450-1952">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="c0450-1953">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="c0450-1953">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span>
* <span data-ttu-id="c0450-1954">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="c0450-1954">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span>
    - <span data-ttu-id="c0450-1955">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="c0450-1955">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="c0450-1956">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="c0450-1956">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="c0450-1957">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="c0450-1957">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c0450-1958">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-1958">Az.OperationalInsights</span></span>
* <span data-ttu-id="c0450-1959">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="c0450-1959">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-1960">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-1960">Az.Resources</span></span>
* <span data-ttu-id="c0450-1961">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="c0450-1961">Support for additional Template Export options</span></span>
    - <span data-ttu-id="c0450-1962">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="c0450-1962">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="c0450-1963">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="c0450-1963">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="c0450-1964">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="c0450-1964">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c0450-1965">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c0450-1965">Az.ServiceFabric</span></span>
* <span data-ttu-id="c0450-1966">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="c0450-1966">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-1967">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-1967">Az.Sql</span></span>
* <span data-ttu-id="c0450-1968">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="c0450-1968">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="c0450-1969">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="c0450-1969">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="c0450-1970">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="c0450-1970">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="c0450-1971">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="c0450-1971">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="c0450-1972">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="c0450-1972">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="c0450-1973">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="c0450-1973">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="c0450-1974">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="c0450-1974">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="c0450-1975">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="c0450-1975">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-1976">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-1976">Az.Storage</span></span>
* <span data-ttu-id="c0450-1977">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="c0450-1977">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="c0450-1978">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c0450-1978">New-AzStorageAccount</span></span>
* <span data-ttu-id="c0450-1979">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="c0450-1979">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="c0450-1980">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="c0450-1980">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c0450-1981">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-1981">Az.Websites</span></span>
* <span data-ttu-id="c0450-1982">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="c0450-1982">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="c0450-1983">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="c0450-1983">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="c0450-1984">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-1984">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="c0450-1985">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c0450-1985">Az.Cdn</span></span>
* <span data-ttu-id="c0450-1986">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="c0450-1986">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-1987">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-1987">Az.Compute</span></span>
* <span data-ttu-id="c0450-1988">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="c0450-1988">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="c0450-1989">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="c0450-1989">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c0450-1990">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c0450-1990">Az.EventHub</span></span>
* <span data-ttu-id="c0450-1991">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="c0450-1991">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="c0450-1992">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="c0450-1992">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-1993">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-1993">Az.Network</span></span>
* <span data-ttu-id="c0450-1994">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="c0450-1994">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="c0450-1995">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="c0450-1995">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c0450-1996">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-1996">Az.PolicyInsights</span></span>
* <span data-ttu-id="c0450-1997">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="c0450-1997">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-1998">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-1998">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-1999">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="c0450-1999">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="c0450-2000">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c0450-2000">Az.ServiceBus</span></span>
* <span data-ttu-id="c0450-2001">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="c0450-2001">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c0450-2002">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c0450-2002">Az.ServiceFabric</span></span>
* <span data-ttu-id="c0450-2003">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="c0450-2003">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="c0450-2004">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c0450-2004">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-2005">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-2005">Az.Sql</span></span>
* <span data-ttu-id="c0450-2006">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="c0450-2006">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="c0450-2007">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c0450-2007">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="c0450-2008">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="c0450-2008">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="c0450-2009">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="c0450-2009">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c0450-2010">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-2010">Az.Websites</span></span>
* <span data-ttu-id="c0450-2011">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="c0450-2011">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="c0450-2012">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-2012">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="c0450-2013">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c0450-2013">Az.ApiManagement</span></span>
* <span data-ttu-id="c0450-2014">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="c0450-2014">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="c0450-2015">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="c0450-2015">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="c0450-2016">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="c0450-2016">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="c0450-2017">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="c0450-2017">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="c0450-2018">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="c0450-2018">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="c0450-2019">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="c0450-2019">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="c0450-2020">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="c0450-2020">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="c0450-2021">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="c0450-2021">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="c0450-2022">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c0450-2022">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="c0450-2023">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="c0450-2023">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="c0450-2024">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="c0450-2024">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="c0450-2025">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="c0450-2025">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="c0450-2026">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="c0450-2026">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="c0450-2027">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="c0450-2027">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="c0450-2028">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="c0450-2028">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="c0450-2029">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="c0450-2029">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="c0450-2030">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="c0450-2030">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="c0450-2031">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="c0450-2031">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="c0450-2032">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="c0450-2032">Created new Cmdlet for generating a User Token.</span></span>
    - <span data-ttu-id="c0450-2033">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="c0450-2033">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="c0450-2034">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="c0450-2034">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="c0450-2035">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="c0450-2035">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="c0450-2036">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="c0450-2036">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="c0450-2037">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c0450-2037">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span>
    - <span data-ttu-id="c0450-2038">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="c0450-2038">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="c0450-2039">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="c0450-2039">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="c0450-2040">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="c0450-2040">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="c0450-2041">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="c0450-2041">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="c0450-2042">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="c0450-2042">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="c0450-2043">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="c0450-2043">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="c0450-2044">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="c0450-2044">Updated the cmdlet to display Error Messages inline</span></span>
     > <span data-ttu-id="c0450-2045">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="c0450-2045">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="c0450-2046">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="c0450-2046">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="c0450-2047">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="c0450-2047">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="c0450-2048">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="c0450-2048">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="c0450-2049">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="c0450-2049">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="c0450-2050">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="c0450-2050">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="c0450-2051">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="c0450-2051">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="c0450-2052">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="c0450-2052">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="c0450-2053">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="c0450-2053">Updated cmdlet **New-AzApiManagementApi**</span></span>
    - <span data-ttu-id="c0450-2054">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="c0450-2054">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="c0450-2055">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="c0450-2055">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="c0450-2056">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="c0450-2056">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="c0450-2057">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="c0450-2057">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="c0450-2058">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="c0450-2058">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="c0450-2059">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="c0450-2059">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="c0450-2060">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="c0450-2060">To updated an API into an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="c0450-2061">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="c0450-2061">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="c0450-2062">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="c0450-2062">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="c0450-2063">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="c0450-2063">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="c0450-2064">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="c0450-2064">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="c0450-2065">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="c0450-2065">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="c0450-2066">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="c0450-2066">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="c0450-2067">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="c0450-2067">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="c0450-2068">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="c0450-2068">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="c0450-2069">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="c0450-2069">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="c0450-2070">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="c0450-2070">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="c0450-2071">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="c0450-2071">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="c0450-2072">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="c0450-2072">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="c0450-2073">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="c0450-2073">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="c0450-2074">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="c0450-2074">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="c0450-2075">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="c0450-2075">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="c0450-2076">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="c0450-2076">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="c0450-2077">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="c0450-2077">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="c0450-2078">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="c0450-2078">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="c0450-2079">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="c0450-2079">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="c0450-2080">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="c0450-2080">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="c0450-2081">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="c0450-2081">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="c0450-2082">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="c0450-2082">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="c0450-2083">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="c0450-2083">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="c0450-2084">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="c0450-2084">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="c0450-2085">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="c0450-2085">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="c0450-2086">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="c0450-2086">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="c0450-2087">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="c0450-2087">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="c0450-2088">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="c0450-2088">'Get-AzApiManagementCertificate'</span></span>
    - <span data-ttu-id="c0450-2089">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="c0450-2089">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="c0450-2090">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="c0450-2090">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c0450-2091">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c0450-2091">Az.Automation</span></span>
* <span data-ttu-id="c0450-2092">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="c0450-2092">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="c0450-2093">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="c0450-2093">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="c0450-2094">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="c0450-2094">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="c0450-2095">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="c0450-2095">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="c0450-2096">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="c0450-2096">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="c0450-2097">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="c0450-2097">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="c0450-2098">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="c0450-2098">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-2099">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-2099">Az.Compute</span></span>
* <span data-ttu-id="c0450-2100">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="c0450-2100">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="c0450-2101">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="c0450-2101">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c0450-2102">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c0450-2102">Az.DataLakeStore</span></span>
* <span data-ttu-id="c0450-2103">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="c0450-2103">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c0450-2104">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c0450-2104">Az.Monitor</span></span>
* <span data-ttu-id="c0450-2105">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="c0450-2105">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-2106">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-2106">Az.Network</span></span>
* <span data-ttu-id="c0450-2107">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="c0450-2107">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="c0450-2108">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="c0450-2108">Updated cmdlet:</span></span>
        - <span data-ttu-id="c0450-2109">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="c0450-2109">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="c0450-2110">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="c0450-2110">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-2111">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-2111">Az.Resources</span></span>
* <span data-ttu-id="c0450-2112">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="c0450-2112">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-2113">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-2113">Az.Sql</span></span>
* <span data-ttu-id="c0450-2114">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="c0450-2114">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="c0450-2115">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-2115">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c0450-2116">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-2116">Az.Accounts</span></span>
* <span data-ttu-id="c0450-2117">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="c0450-2117">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c0450-2118">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c0450-2118">Az.CognitiveServices</span></span>
* <span data-ttu-id="c0450-2119">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="c0450-2119">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="c0450-2120">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="c0450-2120">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-2121">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-2121">Az.Compute</span></span>
* <span data-ttu-id="c0450-2122">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="c0450-2122">Proximity placement group feature.</span></span>
    - <span data-ttu-id="c0450-2123">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="c0450-2123">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="c0450-2124">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-2124">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="c0450-2125">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="c0450-2125">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="c0450-2126">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="c0450-2126">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="c0450-2127">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="c0450-2127">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>
* <span data-ttu-id="c0450-2128">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="c0450-2128">Breaking changes</span></span>
    - <span data-ttu-id="c0450-2129">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="c0450-2129">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="c0450-2130">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="c0450-2130">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="c0450-2131">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="c0450-2131">Az.DeploymentManager</span></span>
* <span data-ttu-id="c0450-2132">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="c0450-2132">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="c0450-2133">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="c0450-2133">Az.Dns</span></span>
* <span data-ttu-id="c0450-2134">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="c0450-2134">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="c0450-2135">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="c0450-2135">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="c0450-2136">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="c0450-2136">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c0450-2137">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c0450-2137">Az.FrontDoor</span></span>
* <span data-ttu-id="c0450-2138">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="c0450-2138">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="c0450-2139">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="c0450-2139">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="c0450-2140">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c0450-2140">Az.HDInsight</span></span>
* <span data-ttu-id="c0450-2141">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c0450-2141">Removed two cmdlets:</span></span>
    - <span data-ttu-id="c0450-2142">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="c0450-2142">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="c0450-2143">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="c0450-2143">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="c0450-2144">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="c0450-2144">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="c0450-2145">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="c0450-2145">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="c0450-2146">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="c0450-2146">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="c0450-2147">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="c0450-2147">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c0450-2148">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c0450-2148">Az.Monitor</span></span>
* <span data-ttu-id="c0450-2149">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="c0450-2149">New cmdlets for SQR API (Scheduled Query Rule)</span></span>
    - <span data-ttu-id="c0450-2150">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="c0450-2150">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="c0450-2151">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="c0450-2151">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="c0450-2152">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="c0450-2152">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="c0450-2153">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="c0450-2153">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="c0450-2154">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="c0450-2154">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="c0450-2155">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="c0450-2155">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="c0450-2156">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="c0450-2156">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="c0450-2157">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="c0450-2157">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="c0450-2158">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="c0450-2158">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="c0450-2159">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="c0450-2159">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="c0450-2160">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="c0450-2160">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="c0450-2161">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="c0450-2161">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="c0450-2162">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="c0450-2162">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-2163">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-2163">Az.Network</span></span>
* <span data-ttu-id="c0450-2164">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="c0450-2164">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="c0450-2165">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="c0450-2165">New cmdlets</span></span>
        - <span data-ttu-id="c0450-2166">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="c0450-2166">New-AzNatGateway</span></span>
        - <span data-ttu-id="c0450-2167">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="c0450-2167">Get-AzNatGateway</span></span>
        - <span data-ttu-id="c0450-2168">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="c0450-2168">Set-AzNatGateway</span></span>
        - <span data-ttu-id="c0450-2169">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="c0450-2169">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="c0450-2170">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="c0450-2170">Updated cmdlets</span></span>
        - <span data-ttu-id="c0450-2171">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="c0450-2171">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="c0450-2172">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="c0450-2172">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="c0450-2173">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="c0450-2173">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="c0450-2174">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="c0450-2174">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="c0450-2175">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="c0450-2175">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c0450-2176">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-2176">Az.PolicyInsights</span></span>
* <span data-ttu-id="c0450-2177">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="c0450-2177">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="c0450-2178">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="c0450-2178">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="c0450-2179">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="c0450-2179">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-2180">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-2180">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-2181">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="c0450-2181">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="c0450-2182">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="c0450-2182">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="c0450-2183">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="c0450-2183">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="c0450-2184">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-2184">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="c0450-2185">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="c0450-2185">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="c0450-2186">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="c0450-2186">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="c0450-2187">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="c0450-2187">Az.Relay</span></span>
* <span data-ttu-id="c0450-2188">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="c0450-2188">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="c0450-2189">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c0450-2189">Az.ServiceBus</span></span>
* <span data-ttu-id="c0450-2190">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="c0450-2190">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-2191">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-2191">Az.Storage</span></span>
* <span data-ttu-id="c0450-2192">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="c0450-2192">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="c0450-2193">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="c0450-2193">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="c0450-2194">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="c0450-2194">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="c0450-2195">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c0450-2195">New-AzStorageAccount</span></span>
* <span data-ttu-id="c0450-2196">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="c0450-2196">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="c0450-2197">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c0450-2197">New-AzStorageAccount</span></span>
    - <span data-ttu-id="c0450-2198">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c0450-2198">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="c0450-2199">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c0450-2199">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c0450-2200">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-2200">Az.Websites</span></span>
* <span data-ttu-id="c0450-2201">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="c0450-2201">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="c0450-2202">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="c0450-2202">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="c0450-2203">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-2203">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c0450-2204">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="c0450-2204">Highlights since the last major release</span></span>
* <span data-ttu-id="c0450-2205">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="c0450-2205">General availability of `Az` module</span></span>
* <span data-ttu-id="c0450-2206">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="c0450-2206">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="c0450-2207">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="c0450-2207">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="c0450-2208">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-2208">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="c0450-2209">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="c0450-2209">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="c0450-2210">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c0450-2210">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="c0450-2211">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="c0450-2211">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c0450-2212">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-2212">Az.Accounts</span></span>
* <span data-ttu-id="c0450-2213">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="c0450-2213">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c0450-2214">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c0450-2214">Az.Batch</span></span>
* <span data-ttu-id="c0450-2215">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c0450-2215">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c0450-2216">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c0450-2216">Az.Cdn</span></span>
* <span data-ttu-id="c0450-2217">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c0450-2217">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c0450-2218">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c0450-2218">Az.CognitiveServices</span></span>
* <span data-ttu-id="c0450-2219">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c0450-2219">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-2220">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-2220">Az.Compute</span></span>
* <span data-ttu-id="c0450-2221">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="c0450-2221">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="c0450-2222">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c0450-2222">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c0450-2223">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="c0450-2223">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c0450-2224">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c0450-2224">Az.DataFactory</span></span>
* <span data-ttu-id="c0450-2225">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="c0450-2225">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c0450-2226">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c0450-2226">Az.DataLakeStore</span></span>
* <span data-ttu-id="c0450-2227">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c0450-2227">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="c0450-2228">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c0450-2228">Az.EventGrid</span></span>
* <span data-ttu-id="c0450-2229">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="c0450-2229">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c0450-2230">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c0450-2230">Az.EventHub</span></span>
* <span data-ttu-id="c0450-2231">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="c0450-2231">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c0450-2232">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c0450-2232">Az.HDInsight</span></span>
* <span data-ttu-id="c0450-2233">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c0450-2233">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c0450-2234">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c0450-2234">Az.IotHub</span></span>
* <span data-ttu-id="c0450-2235">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c0450-2235">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c0450-2236">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0450-2236">Az.KeyVault</span></span>
* <span data-ttu-id="c0450-2237">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c0450-2237">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c0450-2238">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="c0450-2238">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="c0450-2239">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="c0450-2239">Az.MachineLearning</span></span>
* <span data-ttu-id="c0450-2240">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c0450-2240">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="c0450-2241">Az.Media</span><span class="sxs-lookup"><span data-stu-id="c0450-2241">Az.Media</span></span>
* <span data-ttu-id="c0450-2242">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c0450-2242">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c0450-2243">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c0450-2243">Az.Monitor</span></span>
  * <span data-ttu-id="c0450-2244">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="c0450-2244">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="c0450-2245">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="c0450-2245">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="c0450-2246">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="c0450-2246">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="c0450-2247">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="c0450-2247">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="c0450-2248">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="c0450-2248">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="c0450-2249">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="c0450-2249">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="c0450-2250">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="c0450-2250">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-2251">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-2251">Az.Network</span></span>
* <span data-ttu-id="c0450-2252">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c0450-2252">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c0450-2253">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="c0450-2253">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="c0450-2254">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="c0450-2254">Az.NotificationHubs</span></span>
* <span data-ttu-id="c0450-2255">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c0450-2255">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c0450-2256">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-2256">Az.OperationalInsights</span></span>
* <span data-ttu-id="c0450-2257">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c0450-2257">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="c0450-2258">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="c0450-2258">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="c0450-2259">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c0450-2259">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-2260">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-2260">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-2261">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c0450-2261">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c0450-2262">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="c0450-2262">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="c0450-2263">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="c0450-2263">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="c0450-2264">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="c0450-2264">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="c0450-2265">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="c0450-2265">Az.RedisCache</span></span>
* <span data-ttu-id="c0450-2266">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c0450-2266">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-2267">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-2267">Az.Resources</span></span>
* <span data-ttu-id="c0450-2268">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="c0450-2268">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-2269">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-2269">Az.Sql</span></span>
* <span data-ttu-id="c0450-2270">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="c0450-2270">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="c0450-2271">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c0450-2271">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c0450-2272">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="c0450-2272">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="c0450-2273">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="c0450-2273">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="c0450-2274">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="c0450-2274">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="c0450-2275">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="c0450-2275">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="c0450-2276">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="c0450-2276">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c0450-2277">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-2277">Az.Websites</span></span>
* <span data-ttu-id="c0450-2278">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="c0450-2278">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="c0450-2279">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c0450-2279">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c0450-2280">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="c0450-2280">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="c0450-2281">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="c0450-2281">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="c0450-2282">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-2282">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c0450-2283">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="c0450-2283">Highlights since the last major release</span></span>
* <span data-ttu-id="c0450-2284">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="c0450-2284">General availability of `Az` module</span></span>
* <span data-ttu-id="c0450-2285">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="c0450-2285">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="c0450-2286">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="c0450-2286">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="c0450-2287">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-2287">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="c0450-2288">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="c0450-2288">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="c0450-2289">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c0450-2289">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="c0450-2290">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="c0450-2290">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c0450-2291">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-2291">Az.Accounts</span></span>
* <span data-ttu-id="c0450-2292">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="c0450-2292">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="c0450-2293">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c0450-2293">Az.AnalysisServices</span></span>
* <span data-ttu-id="c0450-2294">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="c0450-2294">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="c0450-2295">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="c0450-2295">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c0450-2296">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c0450-2296">Az.Automation</span></span>
* <span data-ttu-id="c0450-2297">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="c0450-2297">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="c0450-2298">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="c0450-2298">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="c0450-2299">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="c0450-2299">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-2300">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-2300">Az.Compute</span></span>
* <span data-ttu-id="c0450-2301">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-2301">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="c0450-2302">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="c0450-2302">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="c0450-2303">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="c0450-2303">Az.ContainerInstance</span></span>
* <span data-ttu-id="c0450-2304">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="c0450-2304">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c0450-2305">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c0450-2305">Az.DataFactory</span></span>
* <span data-ttu-id="c0450-2306">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="c0450-2306">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="c0450-2307">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c0450-2307">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-2308">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-2308">Az.Resources</span></span>
* <span data-ttu-id="c0450-2309">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="c0450-2309">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="c0450-2310">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="c0450-2310">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="c0450-2311">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="c0450-2311">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="c0450-2312">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="c0450-2312">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="c0450-2313">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="c0450-2313">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="c0450-2314">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="c0450-2314">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-2315">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-2315">Az.Sql</span></span>
* <span data-ttu-id="c0450-2316">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="c0450-2316">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-2317">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-2317">Az.Storage</span></span>
* <span data-ttu-id="c0450-2318">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="c0450-2318">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="c0450-2319">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="c0450-2319">New-AzStorageContext</span></span>
* <span data-ttu-id="c0450-2320">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="c0450-2320">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="c0450-2321">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="c0450-2321">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="c0450-2322">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="c0450-2322">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="c0450-2323">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="c0450-2323">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="c0450-2324">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="c0450-2324">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="c0450-2325">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="c0450-2325">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="c0450-2326">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="c0450-2326">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="c0450-2327">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="c0450-2327">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="c0450-2328">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="c0450-2328">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="c0450-2329">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="c0450-2329">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="c0450-2330">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-2330">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c0450-2331">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="c0450-2331">Highlights since the last major release</span></span>
* <span data-ttu-id="c0450-2332">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="c0450-2332">General availability of `Az` module</span></span>
* <span data-ttu-id="c0450-2333">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="c0450-2333">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="c0450-2334">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="c0450-2334">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="c0450-2335">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-2335">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="c0450-2336">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="c0450-2336">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="c0450-2337">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c0450-2337">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="c0450-2338">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="c0450-2338">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c0450-2339">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c0450-2339">Az.Automation</span></span>
* <span data-ttu-id="c0450-2340">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="c0450-2340">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="c0450-2341">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="c0450-2341">Dynamic grouping</span></span>
    * <span data-ttu-id="c0450-2342">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="c0450-2342">Pre-Post script</span></span>
    * <span data-ttu-id="c0450-2343">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="c0450-2343">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-2344">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-2344">Az.Compute</span></span>
* <span data-ttu-id="c0450-2345">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="c0450-2345">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="c0450-2346">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="c0450-2346">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c0450-2347">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0450-2347">Az.KeyVault</span></span>
* <span data-ttu-id="c0450-2348">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0450-2348">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-2349">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-2349">Az.Network</span></span>
* <span data-ttu-id="c0450-2350">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="c0450-2350">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="c0450-2351">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="c0450-2351">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-2352">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-2352">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-2353">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="c0450-2353">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="c0450-2354">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="c0450-2354">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-2355">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-2355">Az.Resources</span></span>
* <span data-ttu-id="c0450-2356">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="c0450-2356">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="c0450-2357">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="c0450-2357">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-2358">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-2358">Az.Sql</span></span>
* <span data-ttu-id="c0450-2359">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="c0450-2359">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-2360">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-2360">Az.Storage</span></span>
* <span data-ttu-id="c0450-2361">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="c0450-2361">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="c0450-2362">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="c0450-2362">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="c0450-2363">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="c0450-2363">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="c0450-2364">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="c0450-2364">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="c0450-2365">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="c0450-2365">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="c0450-2366">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="c0450-2366">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="c0450-2367">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="c0450-2367">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c0450-2368">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-2368">Az.Websites</span></span>
* <span data-ttu-id="c0450-2369">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="c0450-2369">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="c0450-2370">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-2370">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c0450-2371">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-2371">Az.Accounts</span></span>
* <span data-ttu-id="c0450-2372">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="c0450-2372">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="c0450-2373">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="c0450-2373">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c0450-2374">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c0450-2374">Az.Automation</span></span>
* <span data-ttu-id="c0450-2375">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="c0450-2375">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="c0450-2376">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="c0450-2376">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="c0450-2377">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="c0450-2377">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c0450-2378">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c0450-2378">Az.Cdn</span></span>
* <span data-ttu-id="c0450-2379">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="c0450-2379">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-2380">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-2380">Az.Compute</span></span>
* <span data-ttu-id="c0450-2381">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="c0450-2381">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c0450-2382">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c0450-2382">Az.DataFactory</span></span>
* <span data-ttu-id="c0450-2383">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="c0450-2383">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="c0450-2384">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="c0450-2384">Az.LogicApp</span></span>
* <span data-ttu-id="c0450-2385">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="c0450-2385">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-2386">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-2386">Az.Network</span></span>
* <span data-ttu-id="c0450-2387">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="c0450-2387">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-2388">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-2388">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-2389">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="c0450-2389">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="c0450-2390">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="c0450-2390">SDK Update</span></span>
* <span data-ttu-id="c0450-2391">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="c0450-2391">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="c0450-2392">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="c0450-2392">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-2393">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-2393">Az.Resources</span></span>
* <span data-ttu-id="c0450-2394">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="c0450-2394">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="c0450-2395">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="c0450-2395">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="c0450-2396">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="c0450-2396">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="c0450-2397">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="c0450-2397">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="c0450-2398">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="c0450-2398">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="c0450-2399">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="c0450-2399">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-2400">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-2400">Az.Sql</span></span>
* <span data-ttu-id="c0450-2401">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="c0450-2401">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="c0450-2402">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="c0450-2402">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-2403">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-2403">Az.Storage</span></span>
* <span data-ttu-id="c0450-2404">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c0450-2404">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="c0450-2405">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-2405">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="c0450-2406">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c0450-2406">Az.AnalysisServices</span></span>
* <span data-ttu-id="c0450-2407">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="c0450-2407">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c0450-2408">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c0450-2408">Az.Automation</span></span>
* <span data-ttu-id="c0450-2409">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0450-2409">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="c0450-2410">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0450-2410">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="c0450-2411">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0450-2411">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c0450-2412">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c0450-2412">Az.CognitiveServices</span></span>
* <span data-ttu-id="c0450-2413">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="c0450-2413">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-2414">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-2414">Az.Compute</span></span>
* <span data-ttu-id="c0450-2415">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="c0450-2415">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="c0450-2416">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="c0450-2416">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="c0450-2417">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="c0450-2417">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="c0450-2418">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="c0450-2418">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c0450-2419">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c0450-2419">Az.DataLakeStore</span></span>
* <span data-ttu-id="c0450-2420">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="c0450-2420">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c0450-2421">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c0450-2421">Az.EventHub</span></span>
* <span data-ttu-id="c0450-2422">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="c0450-2422">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c0450-2423">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0450-2423">Az.KeyVault</span></span>
* <span data-ttu-id="c0450-2424">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="c0450-2424">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="c0450-2425">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="c0450-2425">Az.LogicApp</span></span>
* <span data-ttu-id="c0450-2426">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="c0450-2426">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="c0450-2427">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="c0450-2427">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="c0450-2428">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="c0450-2428">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="c0450-2429">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="c0450-2429">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="c0450-2430">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="c0450-2430">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="c0450-2431">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="c0450-2431">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="c0450-2432">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="c0450-2432">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="c0450-2433">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="c0450-2433">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="c0450-2434">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0450-2434">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="c0450-2435">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0450-2435">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="c0450-2436">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0450-2436">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="c0450-2437">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0450-2437">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="c0450-2438">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="c0450-2438">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c0450-2439">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c0450-2439">Az.Monitor</span></span>
* <span data-ttu-id="c0450-2440">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="c0450-2440">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-2441">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-2441">Az.Network</span></span>
* <span data-ttu-id="c0450-2442">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="c0450-2442">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c0450-2443">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-2443">Az.OperationalInsights</span></span>
* <span data-ttu-id="c0450-2444">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="c0450-2444">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="c0450-2445">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c0450-2445">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="c0450-2446">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="c0450-2446">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-2447">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-2447">Az.Resources</span></span>
* <span data-ttu-id="c0450-2448">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="c0450-2448">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="c0450-2449">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="c0450-2449">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="c0450-2450">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="c0450-2450">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="c0450-2451">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="c0450-2451">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-2452">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-2452">Az.Sql</span></span>
* <span data-ttu-id="c0450-2453">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="c0450-2453">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="c0450-2454">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="c0450-2454">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c0450-2455">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-2455">Az.Websites</span></span>
* <span data-ttu-id="c0450-2456">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="c0450-2456">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="c0450-2457">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-2457">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c0450-2458">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-2458">Az.Accounts</span></span>
* <span data-ttu-id="c0450-2459">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="c0450-2459">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="c0450-2460">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c0450-2460">Az.AnalysisServices</span></span>
<span data-ttu-id="c0450-2461">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="c0450-2461">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-2462">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-2462">Az.Compute</span></span>
* <span data-ttu-id="c0450-2463">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="c0450-2463">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="c0450-2464">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="c0450-2464">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="c0450-2465">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="c0450-2465">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-2466">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-2466">Az.RecoveryServices</span></span>
<span data-ttu-id="c0450-2467">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="c0450-2467">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-2468">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-2468">Az.Resources</span></span>
* <span data-ttu-id="c0450-2469">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="c0450-2469">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="c0450-2470">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="c0450-2470">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="c0450-2471">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="c0450-2471">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="c0450-2472">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="c0450-2472">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-2473">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-2473">Az.Sql</span></span>
* <span data-ttu-id="c0450-2474">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="c0450-2474">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="c0450-2475">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="c0450-2475">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="c0450-2476">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="c0450-2476">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="c0450-2477">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-2477">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c0450-2478">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-2478">Az.Accounts</span></span>
* <span data-ttu-id="c0450-2479">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="c0450-2479">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="c0450-2480">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c0450-2480">Az.AnalysisServices</span></span>
* <span data-ttu-id="c0450-2481">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="c0450-2481">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-2482">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-2482">Az.RecoveryServices</span></span>
* <span data-ttu-id="c0450-2483">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="c0450-2483">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="c0450-2484">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-2484">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c0450-2485">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-2485">Az.Accounts</span></span>
* <span data-ttu-id="c0450-2486">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="c0450-2486">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="c0450-2487">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c0450-2487">Update incorrect online help URLs</span></span>
* <span data-ttu-id="c0450-2488">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="c0450-2488">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="c0450-2489">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="c0450-2489">Az.Aks</span></span>
* <span data-ttu-id="c0450-2490">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c0450-2490">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c0450-2491">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c0450-2491">Az.Automation</span></span>
* <span data-ttu-id="c0450-2492">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="c0450-2492">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="c0450-2493">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c0450-2493">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c0450-2494">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c0450-2494">Az.Cdn</span></span>
* <span data-ttu-id="c0450-2495">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c0450-2495">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-2496">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-2496">Az.Compute</span></span>
* <span data-ttu-id="c0450-2497">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="c0450-2497">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="c0450-2498">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="c0450-2498">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="c0450-2499">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="c0450-2499">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="c0450-2500">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="c0450-2500">Az.ContainerRegistry</span></span>
* <span data-ttu-id="c0450-2501">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c0450-2501">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c0450-2502">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c0450-2502">Az.DataFactory</span></span>
* <span data-ttu-id="c0450-2503">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="c0450-2503">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c0450-2504">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c0450-2504">Az.DataLakeStore</span></span>
* <span data-ttu-id="c0450-2505">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="c0450-2505">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="c0450-2506">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="c0450-2506">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="c0450-2507">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c0450-2507">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c0450-2508">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c0450-2508">Az.IotHub</span></span>
* <span data-ttu-id="c0450-2509">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="c0450-2509">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c0450-2510">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0450-2510">Az.KeyVault</span></span>
* <span data-ttu-id="c0450-2511">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c0450-2511">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-2512">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-2512">Az.Network</span></span>
* <span data-ttu-id="c0450-2513">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c0450-2513">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-2514">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-2514">Az.Resources</span></span>
* <span data-ttu-id="c0450-2515">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="c0450-2515">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="c0450-2516">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="c0450-2516">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="c0450-2517">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="c0450-2517">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="c0450-2518">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="c0450-2518">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="c0450-2519">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="c0450-2519">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="c0450-2520">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="c0450-2520">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="c0450-2521">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="c0450-2521">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c0450-2522">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c0450-2522">Az.ServiceFabric</span></span>
* <span data-ttu-id="c0450-2523">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="c0450-2523">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="c0450-2524">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="c0450-2524">Fix some error messages.</span></span>
* <span data-ttu-id="c0450-2525">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="c0450-2525">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="c0450-2526">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="c0450-2526">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="c0450-2527">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="c0450-2527">Az.SignalR</span></span>
* <span data-ttu-id="c0450-2528">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c0450-2528">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-2529">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-2529">Az.Sql</span></span>
* <span data-ttu-id="c0450-2530">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c0450-2530">Update incorrect online help URLs</span></span>
* <span data-ttu-id="c0450-2531">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="c0450-2531">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="c0450-2532">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="c0450-2532">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="c0450-2533">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="c0450-2533">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-2534">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-2534">Az.Storage</span></span>
* <span data-ttu-id="c0450-2535">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c0450-2535">Update incorrect online help URLs</span></span>
* <span data-ttu-id="c0450-2536">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="c0450-2536">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="c0450-2537">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="c0450-2537">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="c0450-2538">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="c0450-2538">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="c0450-2539">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c0450-2539">Az.TrafficManager</span></span>
* <span data-ttu-id="c0450-2540">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c0450-2540">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c0450-2541">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-2541">Az.Websites</span></span>
* <span data-ttu-id="c0450-2542">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c0450-2542">Update incorrect online help URLs</span></span>
* <span data-ttu-id="c0450-2543">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="c0450-2543">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="c0450-2544">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="c0450-2544">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="c0450-2545">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="c0450-2545">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c0450-2546">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-2546">Az.Accounts</span></span>
* <span data-ttu-id="c0450-2547">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="c0450-2547">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-2548">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-2548">Az.Compute</span></span>
* <span data-ttu-id="c0450-2549">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="c0450-2549">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="c0450-2550">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="c0450-2550">Updated the description of ID in help files</span></span>
* <span data-ttu-id="c0450-2551">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-2551">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c0450-2552">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c0450-2552">Az.DataLakeStore</span></span>
* <span data-ttu-id="c0450-2553">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="c0450-2553">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="c0450-2554">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="c0450-2554">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="c0450-2555">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c0450-2555">Az.EventGrid</span></span>
* <span data-ttu-id="c0450-2556">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="c0450-2556">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="c0450-2557">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="c0450-2557">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="c0450-2558">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="c0450-2558">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="c0450-2559">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="c0450-2559">Event Time-To-Live,</span></span>
        - <span data-ttu-id="c0450-2560">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="c0450-2560">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="c0450-2561">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="c0450-2561">Dead letter endpoint.</span></span>
    - <span data-ttu-id="c0450-2562">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="c0450-2562">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="c0450-2563">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="c0450-2563">Event Time-To-Live,</span></span>
        - <span data-ttu-id="c0450-2564">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="c0450-2564">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="c0450-2565">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="c0450-2565">Dead letter endpoint.</span></span>
* <span data-ttu-id="c0450-2566">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="c0450-2566">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="c0450-2567">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="c0450-2567">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c0450-2568">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c0450-2568">Az.IotHub</span></span>
* <span data-ttu-id="c0450-2569">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="c0450-2569">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="c0450-2570">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="c0450-2570">Az.LogicApp</span></span>
* <span data-ttu-id="c0450-2571">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="c0450-2571">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-2572">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-2572">Az.Resources</span></span>
* <span data-ttu-id="c0450-2573">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="c0450-2573">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="c0450-2574">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="c0450-2574">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="c0450-2575">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="c0450-2575">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="c0450-2576">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="c0450-2576">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="c0450-2577">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="c0450-2577">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="c0450-2578">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="c0450-2578">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="c0450-2579">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="c0450-2579">Az.SignalR</span></span>
* <span data-ttu-id="c0450-2580">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-2580">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-2581">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-2581">Az.Sql</span></span>
* <span data-ttu-id="c0450-2582">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="c0450-2582">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c0450-2583">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-2583">Az.Storage</span></span>
* <span data-ttu-id="c0450-2584">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="c0450-2584">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="c0450-2585">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="c0450-2585">New-AzStorageContext</span></span>
* <span data-ttu-id="c0450-2586">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="c0450-2586">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="c0450-2587">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="c0450-2587">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c0450-2588">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-2588">Az.Websites</span></span>
* <span data-ttu-id="c0450-2589">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="c0450-2589">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="c0450-2590">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-2590">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="c0450-2591">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="c0450-2591">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="c0450-2592">Geral</span><span class="sxs-lookup"><span data-stu-id="c0450-2592">General</span></span>

- <span data-ttu-id="c0450-2593">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="c0450-2593">General Availability of Az Module</span></span>
- <span data-ttu-id="c0450-2594">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="c0450-2594">Online help for each module</span></span>
- <span data-ttu-id="c0450-2595">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="c0450-2595">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="c0450-2596">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="c0450-2596">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="c0450-2597">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-2597">Az.Accounts</span></span>
- <span data-ttu-id="c0450-2598">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="c0450-2598">Changed from Az.Profile</span></span>
- <span data-ttu-id="c0450-2599">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="c0450-2599">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="c0450-2600">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c0450-2600">Az.ApiManagement</span></span>
- <span data-ttu-id="c0450-2601">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="c0450-2601">Fixes for #7002</span></span>
- <span data-ttu-id="c0450-2602">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c0450-2602">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="c0450-2603">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c0450-2603">Az.Batch</span></span>
- <span data-ttu-id="c0450-2604">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="c0450-2604">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="c0450-2605">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="c0450-2605">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="c0450-2606">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c0450-2606">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="c0450-2607">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="c0450-2607">Az.Billing</span></span>
- <span data-ttu-id="c0450-2608">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c0450-2608">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="c0450-2609">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="c0450-2609">Az.CognitivServices</span></span>
- <span data-ttu-id="c0450-2610">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="c0450-2610">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="c0450-2611">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="c0450-2611">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="c0450-2612">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="c0450-2612">Az.ContainerInstance</span></span>
- <span data-ttu-id="c0450-2613">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="c0450-2613">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="c0450-2614">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="c0450-2614">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="c0450-2615">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c0450-2615">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="c0450-2616">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c0450-2616">Az.DataLakeStore</span></span>
- <span data-ttu-id="c0450-2617">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c0450-2617">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="c0450-2618">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c0450-2618">Az.Monitor</span></span>
- <span data-ttu-id="c0450-2619">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c0450-2619">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="c0450-2620">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c0450-2620">Az.KeyVault</span></span>
- <span data-ttu-id="c0450-2621">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="c0450-2621">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="c0450-2622">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="c0450-2622">Az.MachineLearning</span></span>
- <span data-ttu-id="c0450-2623">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="c0450-2623">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="c0450-2624">Az.Media</span><span class="sxs-lookup"><span data-stu-id="c0450-2624">Az.Media</span></span>
- <span data-ttu-id="c0450-2625">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="c0450-2625">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="c0450-2626">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-2626">Az.Network</span></span>
<span data-ttu-id="c0450-2627">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="c0450-2627">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="c0450-2628">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c0450-2628">New cmdlets added:</span></span>
        - <span data-ttu-id="c0450-2629">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c0450-2629">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="c0450-2630">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c0450-2630">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="c0450-2631">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c0450-2631">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="c0450-2632">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c0450-2632">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="c0450-2633">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c0450-2633">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="c0450-2634">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="c0450-2634">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="c0450-2635">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="c0450-2635">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="c0450-2636">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0450-2636">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="c0450-2637">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c0450-2637">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="c0450-2638">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="c0450-2638">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="c0450-2639">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="c0450-2639">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="c0450-2640">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="c0450-2640">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="c0450-2641">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-2641">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="c0450-2642">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-2642">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="c0450-2643">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="c0450-2643">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="c0450-2644">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="c0450-2644">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="c0450-2645">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="c0450-2645">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="c0450-2646">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="c0450-2646">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="c0450-2647">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="c0450-2647">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="c0450-2648">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="c0450-2648">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="c0450-2649">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c0450-2649">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="c0450-2650">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-2650">Az.OperationalInsights</span></span>
- <span data-ttu-id="c0450-2651">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c0450-2651">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="c0450-2652">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="c0450-2652">Az.Profile</span></span>
- <span data-ttu-id="c0450-2653">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c0450-2653">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-2654">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-2654">Az.RecoveryServices</span></span>
- <span data-ttu-id="c0450-2655">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c0450-2655">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="c0450-2656">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-2656">Az.Resources</span></span>
- <span data-ttu-id="c0450-2657">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c0450-2657">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="c0450-2658">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c0450-2658">Az.ServiceFabric</span></span>
- <span data-ttu-id="c0450-2659">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="c0450-2659">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="c0450-2660">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c0450-2660">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="c0450-2661">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="c0450-2661">Az.SIgnalR</span></span>
- <span data-ttu-id="c0450-2662">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="c0450-2662">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="c0450-2663">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-2663">Az.Sql</span></span>
- <span data-ttu-id="c0450-2664">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="c0450-2664">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="c0450-2665">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="c0450-2665">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="c0450-2666">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c0450-2666">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="c0450-2667">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-2667">Az.Storage</span></span>
- <span data-ttu-id="c0450-2668">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c0450-2668">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="c0450-2669">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-2669">Az.Websites</span></span>
- <span data-ttu-id="c0450-2670">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c0450-2670">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="c0450-2671">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="c0450-2671">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="c0450-2672">Geral</span><span class="sxs-lookup"><span data-stu-id="c0450-2672">General</span></span>

* <span data-ttu-id="c0450-2673">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="c0450-2673">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="c0450-2674">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-2674">Az.Compute</span></span>

* <span data-ttu-id="c0450-2675">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="c0450-2675">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="c0450-2676">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c0450-2676">Az.DataLakeStore</span></span>

* <span data-ttu-id="c0450-2677">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="c0450-2677">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="c0450-2678">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c0450-2678">Az.FrontDoor</span></span>

* <span data-ttu-id="c0450-2679">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="c0450-2679">Fixed some broken links</span></span>
    - <span data-ttu-id="c0450-2680">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="c0450-2680">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="c0450-2681">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="c0450-2681">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="c0450-2682">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c0450-2682">Az.RecoveryServices</span></span>

* <span data-ttu-id="c0450-2683">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-2683">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="c0450-2684">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="c0450-2684">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="c0450-2685">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-2685">Az.Resources</span></span>

* <span data-ttu-id="c0450-2686">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="c0450-2686">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="c0450-2687">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="c0450-2687">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="c0450-2688">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-2688">Az.Sql</span></span>

* <span data-ttu-id="c0450-2689">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="c0450-2689">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="c0450-2690">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="c0450-2690">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="c0450-2691">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="c0450-2691">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="c0450-2692">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-2692">Az.Storage</span></span>

* <span data-ttu-id="c0450-2693">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c0450-2693">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="c0450-2694">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="c0450-2694">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="c0450-2695">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="c0450-2695">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="c0450-2696">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="c0450-2696">Support Static Website configuration</span></span>
    - <span data-ttu-id="c0450-2697">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="c0450-2697">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="c0450-2698">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="c0450-2698">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="c0450-2699">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-2699">Az.Websites</span></span>

* <span data-ttu-id="c0450-2700">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="c0450-2700">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="c0450-2701">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="c0450-2701">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="c0450-2702">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-2702">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="c0450-2703">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="c0450-2703">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="c0450-2704">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c0450-2704">Az.ApiManagement</span></span>
* <span data-ttu-id="c0450-2705">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="c0450-2705">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="c0450-2706">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c0450-2706">Az.Automation</span></span>
* <span data-ttu-id="c0450-2707">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="c0450-2707">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="c0450-2708">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="c0450-2708">Added Update Management cmdlets</span></span>
* <span data-ttu-id="c0450-2709">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="c0450-2709">Added Source Control cmdlets</span></span>
* <span data-ttu-id="c0450-2710">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="c0450-2710">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="c0450-2711">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="c0450-2711">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="c0450-2712">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-2712">Az.Compute</span></span>
* <span data-ttu-id="c0450-2713">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="c0450-2713">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="c0450-2714">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="c0450-2714">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="c0450-2715">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="c0450-2715">Az.ContainerInstance</span></span>
* <span data-ttu-id="c0450-2716">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="c0450-2716">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="c0450-2717">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="c0450-2717">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="c0450-2718">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="c0450-2718">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="c0450-2719">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-2719">Az.Network</span></span>
* <span data-ttu-id="c0450-2720">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="c0450-2720">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="c0450-2721">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="c0450-2721">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="c0450-2722">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="c0450-2722">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="c0450-2723">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="c0450-2723">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="c0450-2724">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="c0450-2724">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="c0450-2725">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="c0450-2725">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="c0450-2726">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="c0450-2726">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="c0450-2727">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="c0450-2727">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="c0450-2728">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="c0450-2728">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="c0450-2729">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="c0450-2729">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="c0450-2730">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="c0450-2730">Az.Relay</span></span>
* <span data-ttu-id="c0450-2731">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="c0450-2731">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="c0450-2732">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-2732">Az.Resources</span></span>
* <span data-ttu-id="c0450-2733">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="c0450-2733">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="c0450-2734">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="c0450-2734">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="c0450-2735">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="c0450-2735">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="c0450-2736">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c0450-2736">Az.ServiceFabric</span></span>
* <span data-ttu-id="c0450-2737">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="c0450-2737">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="c0450-2738">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-2738">Az.Sql</span></span>
* <span data-ttu-id="c0450-2739">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="c0450-2739">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="c0450-2740">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="c0450-2740">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="c0450-2741">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="c0450-2741">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="c0450-2742">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="c0450-2742">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="c0450-2743">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="c0450-2743">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="c0450-2744">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="c0450-2744">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="c0450-2745">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="c0450-2745">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="c0450-2746">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="c0450-2746">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="c0450-2747">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="c0450-2747">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="c0450-2748">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="c0450-2748">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="c0450-2749">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="c0450-2749">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="c0450-2750">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="c0450-2750">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="c0450-2751">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="c0450-2751">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="c0450-2752">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="c0450-2752">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="c0450-2753">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="c0450-2753">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="c0450-2754">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="c0450-2754">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="c0450-2755">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="c0450-2755">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="c0450-2756">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="c0450-2756">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="c0450-2757">Geral</span><span class="sxs-lookup"><span data-stu-id="c0450-2757">General</span></span>
* <span data-ttu-id="c0450-2758">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="c0450-2758">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="c0450-2759">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="c0450-2759">Az.Profile</span></span>
* <span data-ttu-id="c0450-2760">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="c0450-2760">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="c0450-2761">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="c0450-2761">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="c0450-2762">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="c0450-2762">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="c0450-2763">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="c0450-2763">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="c0450-2764">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="c0450-2764">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="c0450-2765">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="c0450-2765">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="c0450-2766">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="c0450-2766">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="c0450-2767">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c0450-2767">Az.CognitiveServices</span></span>
* <span data-ttu-id="c0450-2768">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="c0450-2768">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-2769">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-2769">Az.Compute</span></span>
* <span data-ttu-id="c0450-2770">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="c0450-2770">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="c0450-2771">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="c0450-2771">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="c0450-2772">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="c0450-2772">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c0450-2773">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c0450-2773">Az.DataLakeStore</span></span>
* <span data-ttu-id="c0450-2774">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="c0450-2774">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="c0450-2775">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="c0450-2775">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="c0450-2776">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="c0450-2776">Az.Insights</span></span>
* <span data-ttu-id="c0450-2777">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="c0450-2777">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="c0450-2778">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="c0450-2778">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="c0450-2779">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="c0450-2779">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="c0450-2780">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="c0450-2780">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-2781">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-2781">Az.Network</span></span>
* <span data-ttu-id="c0450-2782">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="c0450-2782">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="c0450-2783">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="c0450-2783">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="c0450-2784">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="c0450-2784">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="c0450-2785">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="c0450-2785">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="c0450-2786">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="c0450-2786">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="c0450-2787">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="c0450-2787">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="c0450-2788">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="c0450-2788">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c0450-2789">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c0450-2789">Az.PolicyInsights</span></span>
* <span data-ttu-id="c0450-2790">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="c0450-2790">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-2791">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-2791">Az.Resources</span></span>
* <span data-ttu-id="c0450-2792">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="c0450-2792">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="c0450-2793">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="c0450-2793">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="c0450-2794">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c0450-2794">Az.ServiceBus</span></span>
* <span data-ttu-id="c0450-2795">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="c0450-2795">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c0450-2796">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c0450-2796">Az.ServiceFabric</span></span>
* <span data-ttu-id="c0450-2797">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="c0450-2797">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="c0450-2798">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="c0450-2798">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="c0450-2799">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="c0450-2799">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="c0450-2800">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="c0450-2800">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="c0450-2801">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="c0450-2801">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="c0450-2802">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="c0450-2802">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="c0450-2803">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="c0450-2803">Az.Profile</span></span>
* <span data-ttu-id="c0450-2804">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="c0450-2804">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="c0450-2805">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="c0450-2805">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-2806">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-2806">Az.Compute</span></span>
* <span data-ttu-id="c0450-2807">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="c0450-2807">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="c0450-2808">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="c0450-2808">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c0450-2809">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c0450-2809">Az.DataLakeStore</span></span>
* <span data-ttu-id="c0450-2810">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="c0450-2810">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="c0450-2811">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-2811">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="c0450-2812">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="c0450-2812">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="c0450-2813">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="c0450-2813">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="c0450-2814">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="c0450-2814">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-2815">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-2815">Az.Network</span></span>
* <span data-ttu-id="c0450-2816">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="c0450-2816">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="c0450-2817">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="c0450-2817">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-2818">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-2818">Az.Resources</span></span>
* <span data-ttu-id="c0450-2819">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="c0450-2819">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="c0450-2820">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="c0450-2820">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="c0450-2821">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="c0450-2821">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="c0450-2822">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="c0450-2822">Azure.Storage</span></span>
* <span data-ttu-id="c0450-2823">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="c0450-2823">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="c0450-2824">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="c0450-2824">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="c0450-2825">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="c0450-2825">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="c0450-2826">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="c0450-2826">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="c0450-2827">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="c0450-2827">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c0450-2828">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c0450-2828">Az.CognitiveServices</span></span>
* <span data-ttu-id="c0450-2829">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="c0450-2829">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c0450-2830">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c0450-2830">Az.Compute</span></span>
* <span data-ttu-id="c0450-2831">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="c0450-2831">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="c0450-2832">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="c0450-2832">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="c0450-2833">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="c0450-2833">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="c0450-2834">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="c0450-2834">Az.DataFactoryV2</span></span>
* <span data-ttu-id="c0450-2835">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="c0450-2835">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c0450-2836">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c0450-2836">Az.Network</span></span>
* <span data-ttu-id="c0450-2837">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="c0450-2837">Added NetworkProfile functionality.</span></span> <span data-ttu-id="c0450-2838">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="c0450-2838">new cmdlets added</span></span>
    - <span data-ttu-id="c0450-2839">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c0450-2839">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="c0450-2840">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c0450-2840">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="c0450-2841">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c0450-2841">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="c0450-2842">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c0450-2842">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="c0450-2843">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-2843">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="c0450-2844">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-2844">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="c0450-2845">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="c0450-2845">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="c0450-2846">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="c0450-2846">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="c0450-2847">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="c0450-2847">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="c0450-2848">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="c0450-2848">Az.RedisCache</span></span>
* <span data-ttu-id="c0450-2849">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="c0450-2849">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="c0450-2850">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="c0450-2850">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="c0450-2851">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c0450-2851">Az.Resources</span></span>
* <span data-ttu-id="c0450-2852">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="c0450-2852">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="c0450-2853">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="c0450-2853">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="c0450-2854">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c0450-2854">Az.Sql</span></span>
* <span data-ttu-id="c0450-2855">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="c0450-2855">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c0450-2856">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c0450-2856">Az.Websites</span></span>
* <span data-ttu-id="c0450-2857">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="c0450-2857">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="c0450-2858">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="c0450-2858">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="c0450-2859">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="c0450-2859">0.2.0 - September 2018</span></span>
 <span data-ttu-id="c0450-2860">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="c0450-2860">Initial Release</span></span>
