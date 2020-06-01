---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.openlocfilehash: 60827fe7b4f8c351655046e3711660cdf7ce0513
ms.sourcegitcommit: 10ec909100a70acec94d42f6084e7bf0342c6854
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2020
ms.locfileid: "83631069"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="11aab-103">Notas de versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="11aab-103">Azure PowerShell release notes</span></span>

## <a name="410---may-2020"></a><span data-ttu-id="11aab-104">4.1.0 - Maio de 2020</span><span class="sxs-lookup"><span data-stu-id="11aab-104">4.1.0 - May 2020</span></span>
### <a name="highlights-since-the-last-release"></a><span data-ttu-id="11aab-105">Destaques desde a última versão</span><span class="sxs-lookup"><span data-stu-id="11aab-105">Highlights since the last release</span></span>
* <span data-ttu-id="11aab-106">Versões do PowerShell suportadas: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span><span class="sxs-lookup"><span data-stu-id="11aab-106">Supported PowerShell versions: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span></span>
* <span data-ttu-id="11aab-107">Disponibilidade geral de Az.Functions</span><span class="sxs-lookup"><span data-stu-id="11aab-107">General availability of Az.Functions</span></span> 
* <span data-ttu-id="11aab-108">Az.ApiManagement, Az.Batch, Az.Compute, Az.KeyVault, Az.Monitor, Az.Network, Az.OperationalInsights, Az.Resources e Az.Storage são alvo de grandes versões</span><span class="sxs-lookup"><span data-stu-id="11aab-108">Az.ApiManagement, Az.Batch, Az.Compute, Az.KeyVault, Az.Monitor, Az.Network, Az.OperationalInsights, Az.Resources, and Az.Storage have major release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="11aab-109">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-109">Az.Accounts</span></span>
* <span data-ttu-id="11aab-110">"Add-AzEnvironment" e "Set-AzEnvironment" foram atualizados para aceitar os parâmetros "AzureSynapseAnalyticsEndpointResourceId" e "AzureSynapseAnalyticsEndpointSuffix"</span><span class="sxs-lookup"><span data-stu-id="11aab-110">Updated 'Add-AzEnvironment' and 'Set-AzEnvironment' to accept parameters 'AzureSynapseAnalyticsEndpointResourceId' and 'AzureSynapseAnalyticsEndpointSuffix'</span></span>
* <span data-ttu-id="11aab-111">Foram adicionadas assemblagens relacionadas ao Azure.Core em Az.Accounts; as plataformas suportadas do PowerShell incluem Windows PowerShell 5.1, PowerShell Core 6.2.4, PowerShell 7+</span><span class="sxs-lookup"><span data-stu-id="11aab-111">Added Azure.Core related assemblies into Az.Accounts, supported PowerShell platforms include Windows PowerShell 5.1, PowerShell Core 6.2.4, PowerShell 7+</span></span>

#### <a name="azaks"></a><span data-ttu-id="11aab-112">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="11aab-112">Az.Aks</span></span>
* <span data-ttu-id="11aab-113">Versão da API atualizada para 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="11aab-113">Upgraded API Version to 2019-10-01</span></span>
* <span data-ttu-id="11aab-114">Suportado para criar o AKS com contentores do Windows</span><span class="sxs-lookup"><span data-stu-id="11aab-114">Supported to create AKS using Windows container</span></span>
* <span data-ttu-id="11aab-115">Novos cmdlets fornecidos: "New-AzAksNodePool", "Update-AzAksNodePool", "Remove-AzAksNodePool",        "Get-AzAksNodePool", "Install-AzAksKubectl", "Get-AzAksVersion"</span><span class="sxs-lookup"><span data-stu-id="11aab-115">Provided new cmdlets: 'New-AzAksNodePool', 'Update-AzAksNodePool', 'Remove-AzAksNodePool',        'Get-AzAksNodePool', 'Install-AzAksKubectl', 'Get-AzAksVersion'</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="11aab-116">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="11aab-116">Az.ApiManagement</span></span>
* <span data-ttu-id="11aab-117">"New-AzApiManagement" e "Set-AzApiManagement": o nome do parâmetro [-AssignIdentity] foi mudado para [-SystemAssignedIdentity]</span><span class="sxs-lookup"><span data-stu-id="11aab-117">'New-AzApiManagement' and 'Set-AzApiManagement': [-AssignIdentity] parameter renamed as [-SystemAssignedIdentity]</span></span>
* <span data-ttu-id="11aab-118">"New-AzApiManagement" e "Set-AzApiManagement": Novo parâmetro adicionado: [-UserAssignedIdentity <String[]>]</span><span class="sxs-lookup"><span data-stu-id="11aab-118">'New-AzApiManagement' and 'Set-AzApiManagement': New parameter added: [-UserAssignedIdentity <String[]>]</span></span>
* <span data-ttu-id="11aab-119">"Get-AzApiManagementProperty": o nome foi mudado para "Get-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="11aab-119">'Get-AzApiManagementProperty': renamed as 'Get-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="11aab-120">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="11aab-120">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="11aab-121">"New-AzApiManagementProperty": o nome foi mudado para "New-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="11aab-121">'New-AzApiManagementProperty': renamed as 'New-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="11aab-122">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="11aab-122">PropertyId parameter renamed as NamedValueId.</span></span> 
* <span data-ttu-id="11aab-123">"Set-AzApiManagementProperty": o nome foi mudado para "Set-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="11aab-123">'Set-AzApiManagementProperty': renamed as 'Set-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="11aab-124">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="11aab-124">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="11aab-125">"Remove-AzApiManagementProperty": o nome foi mudado para "Remove-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="11aab-125">'Remove-AzApiManagementProperty': renamed as 'Remove-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="11aab-126">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="11aab-126">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="11aab-127">Foi adicionado o cmdlet novo "Get-AzApiManagementAuthorizationServerClientSecret" e "Get-AzApiManagementAuthorizationServer" vai deixar de devolver o segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="11aab-127">Added new 'Get-AzApiManagementAuthorizationServerClientSecret' cmdlet and 'Get-AzApiManagementAuthorizationServer' will not return client secret anymore.</span></span>
* <span data-ttu-id="11aab-128">Foi adicionado o cmdlet novo "Get-AzApiManagementNamedValueSecretValue" e "Get-AzApiManagementNamedValue" vai deixar de devolver o valor do segredo.</span><span class="sxs-lookup"><span data-stu-id="11aab-128">Added new 'Get-AzApiManagementNamedValueSecretValue' cmdlet and 'Get-AzApiManagementNamedValue' will not return secret value.</span></span>
* <span data-ttu-id="11aab-129">Foi adicionado o cmdlet novo "Get-AzApiManagementOpenIdConnectProviderClientSecret" e "Get-AzApiManagementOpenIdConnectProvider" vai deixar de devolver o segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="11aab-129">Added new 'Get-AzApiManagementOpenIdConnectProviderClientSecret' cmdlet and 'Get-AzApiManagementOpenIdConnectProvider' will not return client secret anymore.</span></span>
* <span data-ttu-id="11aab-130">Foi adicionado o cmdlet "Get-AzApiManagementSubscriptionKey" e "Get-AzApiManagementSubscription" vai deixar de devolver chaves de subscrições.</span><span class="sxs-lookup"><span data-stu-id="11aab-130">Added new 'Get-AzApiManagementSubscriptionKey' cmdlet and 'Get-AzApiManagementSubscription' will not return subscription keys anymore.</span></span>
* <span data-ttu-id="11aab-131">Foi adicionado o cmdlet novo "Get-AzApiManagementTenantAccessSecret" e "Get-AzApiManagementTenantAccess" vai deixar de devolver chaves.</span><span class="sxs-lookup"><span data-stu-id="11aab-131">Added new 'Get-AzApiManagementTenantAccessSecret' cmdlet and 'Get-AzApiManagementTenantAccess' will not return keys anymore.</span></span>
* <span data-ttu-id="11aab-132">Foi adicionado o cmdlet novo "Get-AzApiManagementTenantGitAccessSecret" e "Get-AzApiManagementTenantGitAccess" vai deixar de devolver chaves.</span><span class="sxs-lookup"><span data-stu-id="11aab-132">Added new 'Get-AzApiManagementTenantGitAccessSecret' cmdlet and 'Get-AzApiManagementTenantGitAccess' will not return keys anymore.</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="11aab-133">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="11aab-133">Az.ApplicationInsights</span></span>
* <span data-ttu-id="11aab-134">Parâmetros adicionados: "RetentionInDays" "PublicNetworkAccessForIngestion" "PublicNetworkAccessForQuery" a "New-AzApplicationInsights"</span><span class="sxs-lookup"><span data-stu-id="11aab-134">Added Parameters: 'RetentionInDays' 'PublicNetworkAccessForIngestion' 'PublicNetworkAccessForQuery' for 'New-AzApplicationInsights'</span></span>
* <span data-ttu-id="11aab-135">Foi criado o cmdlet "Update-AzApplicationInsights”</span><span class="sxs-lookup"><span data-stu-id="11aab-135">Created cmdlet 'Update-AzApplicationInsights'</span></span>
* <span data-ttu-id="11aab-136">Foram criados cmdlets para a Conta de Armazenamento Associada</span><span class="sxs-lookup"><span data-stu-id="11aab-136">Created cmdlets for Linked Storage Account</span></span>

#### <a name="azbatch"></a><span data-ttu-id="11aab-137">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="11aab-137">Az.Batch</span></span>
* <span data-ttu-id="11aab-138">Az.Batch foi atualizado para utilizar a versão do SDK "Microsoft.Azure.Batc" 13.0.0 e a versão do SDK "Microsoft.Azure.Management.Batch" 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="11aab-138">Updated Az.Batch to use 'Microsoft.Azure.Batch' SDK version 13.0.0 and 'Microsoft.Azure.Management.Batch' SDK version 9.0.0.</span></span>
* <span data-ttu-id="11aab-139">Foi adicionada a capacidade de selecionar o tipo de certificado que vai ser adicionado mediante a utilização do novo parâmetro "-CertificateKind" para "New-AzBatchCertificate".</span><span class="sxs-lookup"><span data-stu-id="11aab-139">Added the ability to select the kind of certificate being added using the new '-CertificateKind' parameter to 'New-AzBatchCertificate'.</span></span>
* <span data-ttu-id="11aab-140">A propriedade "ApplicationPackages" foi removida de "PSApplication", que anteriormente era sempre ''.</span><span class="sxs-lookup"><span data-stu-id="11aab-140">Removed 'ApplicationPackages' property from 'PSApplication' which was previously always ''.</span></span>
  - <span data-ttu-id="11aab-141">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com "Get-AzBatchApplicationPackage".</span><span class="sxs-lookup"><span data-stu-id="11aab-141">The specific packages inside of an application now can be retrieved using 'Get-AzBatchApplicationPackage'.</span></span> <span data-ttu-id="11aab-142">Por exemplo: "Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication".</span><span class="sxs-lookup"><span data-stu-id="11aab-142">For example: 'Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication'.</span></span>
* <span data-ttu-id="11aab-143">Agora, ao utilizar "New-AzBatchPool" para criar um conjunto, a propriedade "VirtualMachineImageId" de "PSImageReference" só pode fazer referência a uma imagem do Shared Image Gallery.</span><span class="sxs-lookup"><span data-stu-id="11aab-143">When creating a pool using 'New-AzBatchPool', the 'VirtualMachineImageId' property of 'PSImageReference' can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="11aab-144">Ao utilizar "New-AzBatchPool" para criar um conjunto, o conjunto pode ser aprovisionado sem um IP público mediante a utilização da nova propriedade "PublicIPAddressConfiguration" de "PSNetworkConfiguration".</span><span class="sxs-lookup"><span data-stu-id="11aab-144">When creating a pool using 'New-AzBatchPool', the pool can be provisioned without a public IP using the new 'PublicIPAddressConfiguration' property of 'PSNetworkConfiguration'.</span></span>
  - <span data-ttu-id="11aab-145">A propriedade "PublicIPs" de "PSNetworkConfiguration" foi igualmente movida para "PSPublicIPAddressConfiguration".</span><span class="sxs-lookup"><span data-stu-id="11aab-145">The 'PublicIPs' property of 'PSNetworkConfiguration' has moved in to 'PSPublicIPAddressConfiguration' as well.</span></span> <span data-ttu-id="11aab-146">Esta propriedade só pode ser especificada se "IPAddressProvisioningType" for "UserManaged".</span><span class="sxs-lookup"><span data-stu-id="11aab-146">This property can only be specified if 'IPAddressProvisioningType' is 'UserManaged'.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-147">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-147">Az.Compute</span></span>
* <span data-ttu-id="11aab-148">Foi adicionado o parâmetro HostId ao cmdlet "Update-AzVM"</span><span class="sxs-lookup"><span data-stu-id="11aab-148">Added HostId parameter to 'Update-AzVM' cmdlet</span></span>
* <span data-ttu-id="11aab-149">Os documentos de Ajuda para os cmdlets "New-AzVMConfig", "New-AzVmssConfig", "Update-AzVmss", "Set-AzVMOperatingSystem" e "Set-AzVmssOsProfile" foram atualizados.</span><span class="sxs-lookup"><span data-stu-id="11aab-149">Updated Help documents for 'New-AzVMConfig', 'New-AzVmssConfig', 'Update-AzVmss', 'Set-AzVMOperatingSystem' and 'Set-AzVmssOsProfile' cmdlets.</span></span>
* <span data-ttu-id="11aab-150">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="11aab-150">Breaking changes</span></span>
    - <span data-ttu-id="11aab-151">O parâmetro FilterExpression foi removido do cmdlet "Get-AzVMImage".</span><span class="sxs-lookup"><span data-stu-id="11aab-151">FilterExpression parameter is removed from 'Get-AzVMImage' cmdlet.</span></span>
    - <span data-ttu-id="11aab-152">O parâmetro AssignIdentity foi removido dos cmdlets "New-AzVmssConfig", "New-AzVMConfig" e "Update-AzVM".</span><span class="sxs-lookup"><span data-stu-id="11aab-152">AssignIdentity parameter is removed from 'New-AzVmssConfig', 'New-AzVMConfig' and 'Update-AzVM' cmdlets.</span></span>
    - <span data-ttu-id="11aab-153">AutomaticRepairMaxInstanceRepairsPercent foi removido dos cmdlets "New-AzVmssConfig" e "Update-AzVmss".</span><span class="sxs-lookup"><span data-stu-id="11aab-153">AutomaticRepairMaxInstanceRepairsPercent is removed from 'New-AzVmssConfig' and 'Update-AzVmss' cmdlets.</span></span>
    - <span data-ttu-id="11aab-154">As propriedades AvailabilitySetsColocationStatus, VirtualMachinesColocationStatus e VirtualMachineScaleSetsColocationStatus foram removidas de ProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="11aab-154">AvailabilitySetsColocationStatus, VirtualMachinesColocationStatus and VirtualMachineScaleSetsColocationStatus properties are removed from ProximityPlacementGroup.</span></span>
    - <span data-ttu-id="11aab-155">A propriedade MaxInstanceRepairsPercent foi removida de AutomaticRepairsPolicy.</span><span class="sxs-lookup"><span data-stu-id="11aab-155">MaxInstanceRepairsPercent property is removed from AutomaticRepairsPolicy.</span></span>
    - <span data-ttu-id="11aab-156">Os tipos de AvailabilitySets, VirtualMachines e VirtualMachineScaleSets foram alterados de IList<SubResource> para IList<SubResourceWithColocationStatus>.</span><span class="sxs-lookup"><span data-stu-id="11aab-156">The types of AvailabilitySets, VirtualMachines and VirtualMachineScaleSets are changed from IList<SubResource> to IList<SubResourceWithColocationStatus>.</span></span>
* <span data-ttu-id="11aab-157">A descrição do cmdlet "Get-AzVM" foi atualizada para o descrever melhor.</span><span class="sxs-lookup"><span data-stu-id="11aab-157">Description for 'Get-AzVM' cmdlet has been updated to better describe it.</span></span> 

#### <a name="azdatafactory"></a><span data-ttu-id="11aab-158">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="11aab-158">Az.DataFactory</span></span>
* <span data-ttu-id="11aab-159">CRUD suportado das propriedades de fluxo de dados no IR Gerido.</span><span class="sxs-lookup"><span data-stu-id="11aab-159">Supported CRUD of data flow runtime properties in Managed IR.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="11aab-160">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="11aab-160">Az.FrontDoor</span></span>
* <span data-ttu-id="11aab-161">Foram adicionados cmdlets novos para criação, atualização, obtenção e eliminação do objeto de Motor de Regras do Front Door</span><span class="sxs-lookup"><span data-stu-id="11aab-161">Added new cmdlets for creation, update, retreival, and deletion of Front Door Rules Engine object</span></span>
* <span data-ttu-id="11aab-162">Foram adicionados cmdlets de programas auxiliares para construção do objeto de Motor de Regras do Front Door</span><span class="sxs-lookup"><span data-stu-id="11aab-162">Added helper cmdlets for construction of Front Door Rules Engine object</span></span>
* <span data-ttu-id="11aab-163">Foi adicionada a referência ao Motor de Regras ao objeto Regra de Encaminhamento do Front Door.</span><span class="sxs-lookup"><span data-stu-id="11aab-163">Added Rules Engine reference to Front Door Routing Rule object.</span></span>
* <span data-ttu-id="11aab-164">Foram adicionados parâmetros do Private Link ao objeto de Back-end do Front Door</span><span class="sxs-lookup"><span data-stu-id="11aab-164">Added Private Link parameters to Front Door Backend object</span></span>

#### <a name="azfunctions"></a><span data-ttu-id="11aab-165">Az.Functions</span><span class="sxs-lookup"><span data-stu-id="11aab-165">Az.Functions</span></span>
* <span data-ttu-id="11aab-166">Disponibilidade geral do módulo Az.Functions</span><span class="sxs-lookup"><span data-stu-id="11aab-166">General availability of ''Az.Functions'' module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="11aab-167">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="11aab-167">Az.HDInsight</span></span>
* <span data-ttu-id="11aab-168">Encriptação de discos de chave gerida pelo cliente suportada</span><span class="sxs-lookup"><span data-stu-id="11aab-168">Supported Customer-managed key disk encryption.</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="11aab-169">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="11aab-169">Az.HealthcareApis</span></span>
* <span data-ttu-id="11aab-170">As políticas de acesso já não são predefinidas para o principal atual</span><span class="sxs-lookup"><span data-stu-id="11aab-170">Access policies are no longer defaulted to the current principal</span></span>

#### <a name="aziothub"></a><span data-ttu-id="11aab-171">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="11aab-171">Az.IotHub</span></span>
* <span data-ttu-id="11aab-172">Foi adicionado um cmdlet para invocar uma consulta num hub IoT para obter informações mediante a utilização de uma linguagem tipo SQL.</span><span class="sxs-lookup"><span data-stu-id="11aab-172">Added cmdlet to invoke a query in an IoT hub to retrieve information using a SQL-like language.</span></span>
* <span data-ttu-id="11aab-173">Foi corrigido um problema em que "Add-AzIotHubDevice" falha ao criar um Dispositivo Compatível com o Edge sem dispositivos subordinados [#11597]</span><span class="sxs-lookup"><span data-stu-id="11aab-173">Fix issue that 'Add-AzIotHubDevice' fails to create Edge Enabled Device without child devices [#11597]</span></span>
* <span data-ttu-id="11aab-174">Foi adicionado o cmdlet para gerar o token de SAS para o Hub IoT, um dispositivo ou um módulo.</span><span class="sxs-lookup"><span data-stu-id="11aab-174">Added cmdlet to generate SAS token for Iot Hub, device or module.</span></span>
* <span data-ttu-id="11aab-175">Foi adicionado um cmdlet para invocar a consulta de métricas de configuração.</span><span class="sxs-lookup"><span data-stu-id="11aab-175">Added cmdlet to invoke configuration metrics query.</span></span>
* <span data-ttu-id="11aab-176">Gerir implementações automáticas do IoT Edge em escala.</span><span class="sxs-lookup"><span data-stu-id="11aab-176">Manage IoT Edge automatic deployment at scale.</span></span> <span data-ttu-id="11aab-177">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="11aab-177">New cmdlets are:</span></span>
    - <span data-ttu-id="11aab-178">"Add-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="11aab-178">'Add-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="11aab-179">"Get-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="11aab-179">'Get-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="11aab-180">"Remove-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="11aab-180">'Remove-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="11aab-181">"Set-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="11aab-181">'Set-AzIotHubDeployment'</span></span>
* <span data-ttu-id="11aab-182">Foi adicionado um cmdlet para invocar uma consulta de métricas de implementação do IoT Edge.</span><span class="sxs-lookup"><span data-stu-id="11aab-182">Added cmdlet to invoke an IoT Edge deployment metrics query.</span></span>
* <span data-ttu-id="11aab-183">Foi adicionado um cmdlet para aplicar o conteúdo da configuração ao dispositivo edge especificado.</span><span class="sxs-lookup"><span data-stu-id="11aab-183">Added cmdlet to apply the configuration content to the specified edge device.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="11aab-184">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="11aab-184">Az.KeyVault</span></span>
* <span data-ttu-id="11aab-185">Foram removidos dois aliases: "New-AzKeyVaultCertificateAdministratorDetails" e "New-AzKeyVaultCertificateOrganizationDetails"</span><span class="sxs-lookup"><span data-stu-id="11aab-185">Removed two aliases: 'New-AzKeyVaultCertificateAdministratorDetails' and 'New-AzKeyVaultCertificateOrganizationDetails'</span></span>
* <span data-ttu-id="11aab-186">A eliminação recuperável foi ativada por predefinição ao criar um cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="11aab-186">Enabled soft delete by default when creating a key vault</span></span>
* <span data-ttu-id="11aab-187">Podem ser definidas regras de rede para governar a acessibilidade a partir de localizações na rede ao criar um cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="11aab-187">Network rules can be set to govern the accessibility from specific network locations when creating a key vault</span></span>
* <span data-ttu-id="11aab-188">Foi adicionado suporte para Bring Your Own Key (BYOK)</span><span class="sxs-lookup"><span data-stu-id="11aab-188">Added support to bring your own key (BYOK)</span></span>
    - <span data-ttu-id="11aab-189">"Add-AzKeyVaultKey" suporta a geração de chaves de intercâmbio de chaves</span><span class="sxs-lookup"><span data-stu-id="11aab-189">'Add-AzKeyVaultKey' supports generating a key exchange key</span></span>
    - <span data-ttu-id="11aab-190">"Get-AzKeyVaultKey" suporta a transferência de chaves públicas no formato PEM</span><span class="sxs-lookup"><span data-stu-id="11aab-190">'Get-AzKeyVaultKey' supports downloading a public key in PEM format</span></span>
* <span data-ttu-id="11aab-191">"KeyOps" foi atualizado como parte do documento de ajuda de "Add-AzKeyVaultKey"</span><span class="sxs-lookup"><span data-stu-id="11aab-191">Updated the 'KeyOps' part of the help document of 'Add-AzKeyVaultKey'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="11aab-192">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="11aab-192">Az.Monitor</span></span>
* <span data-ttu-id="11aab-193">Foi corrigido um erro em "Set-AzDiagnosticSettings"; a política de retenção não se aplicará a todas as categorias [#11589]</span><span class="sxs-lookup"><span data-stu-id="11aab-193">Fixed bug for 'Set-AzDiagnosticSettings', retention policy won't apply to all categories [#11589]</span></span>
* <span data-ttu-id="11aab-194">Suporte para critérios de disponibilidade de WebTest para alertas de métricas V2</span><span class="sxs-lookup"><span data-stu-id="11aab-194">Supported WebTest availability criteria for metric alert V2</span></span>
    - <span data-ttu-id="11aab-195">Novo "New-AzMetricAlertRuleV2Criteria": foi adicionada uma opção para criar critérios de disponibilidade WebTest</span><span class="sxs-lookup"><span data-stu-id="11aab-195">'New-AzMetricAlertRuleV2Criteria': an option to create webtest availability criteria was added</span></span>
    - <span data-ttu-id="11aab-196">"Add-AzMetricAlertRuleV2": suporta os novos critérios de disponibilidade de WebTest</span><span class="sxs-lookup"><span data-stu-id="11aab-196">'Add-AzMetricAlertRuleV2': supports the new webtest availability criteria</span></span>
* <span data-ttu-id="11aab-197">Foi removida a definição redundante de RetentionPolicy em PSLogProfile [#7608]</span><span class="sxs-lookup"><span data-stu-id="11aab-197">Removed redundant definition for RetentionPolicy in PSLogProfile [#7608]</span></span>
* <span data-ttu-id="11aab-198">Foram removidas as propriedades redundantes definidas em PSEventData [#11353]</span><span class="sxs-lookup"><span data-stu-id="11aab-198">Removed redundant properties difined in PSEventData [#11353]</span></span>
* <span data-ttu-id="11aab-199">O nome de "Get-AzLog" foi mudado para "Get-AzActivityLog"</span><span class="sxs-lookup"><span data-stu-id="11aab-199">Renamed 'Get-AzLog' to 'Get-AzActivityLog'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-200">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-200">Az.Network</span></span>
* <span data-ttu-id="11aab-201">Foi adicionado um atributo de alteração interruptiva para notificar que o comportamento predefinido da Zona vai ser alterado</span><span class="sxs-lookup"><span data-stu-id="11aab-201">Added breaking change attribute to notify that Zone default behaviour will be changed</span></span>
    - <span data-ttu-id="11aab-202">"New-AzPublicIpAddress"</span><span class="sxs-lookup"><span data-stu-id="11aab-202">'New-AzPublicIpAddress'</span></span>
    - <span data-ttu-id="11aab-203">"New-AzPublicIpPrefix"</span><span class="sxs-lookup"><span data-stu-id="11aab-203">'New-AzPublicIpPrefix'</span></span>
    - <span data-ttu-id="11aab-204">"New-AzLoadBalancerFrontendIpConfig"</span><span class="sxs-lookup"><span data-stu-id="11aab-204">'New-AzLoadBalancerFrontendIpConfig'</span></span>
* <span data-ttu-id="11aab-205">Foi adicionado suportado para um recurso de nível superior novo SecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="11aab-205">Added support for a new top level resource SecurityPartnerProvider</span></span>
    - <span data-ttu-id="11aab-206">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="11aab-206">New cmdlets added:</span></span>
        - <span data-ttu-id="11aab-207">New-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="11aab-207">New-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="11aab-208">Remove-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="11aab-208">Remove-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="11aab-209">Get-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="11aab-209">Get-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="11aab-210">Set-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="11aab-210">Set-AzSecurityPartnerProvider</span></span>
* <span data-ttu-id="11aab-211">Foi adicionado "RequiredZoneNames" em "PSPrivateLinkResource" e "GroupId" em "PSPrivateEndpointConnection”</span><span class="sxs-lookup"><span data-stu-id="11aab-211">Added 'RequiredZoneNames' on 'PSPrivateLinkResource' and 'GroupId' on 'PSPrivateEndpointConnection'</span></span>
* <span data-ttu-id="11aab-212">Foi corrigido o tipo incorreto do parâmetro SuccessThresholdRoundTripTimeMs para New-AzNetworkWatcherConnectionMonitorTestConfigurationObject</span><span class="sxs-lookup"><span data-stu-id="11aab-212">Fixed incorrect type of SuccessThresholdRoundTripTimeMs parameter for New-AzNetworkWatcherConnectionMonitorTestConfigurationObject</span></span>
* <span data-ttu-id="11aab-213">Foram atualizados os cmdlets VirtualWan para definir o valor predefinido do argumento AllowVnetToVnetTraffic como Verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="11aab-213">Updated VirtualWan cmdlets to set default value of AllowVnetToVnetTraffic argument to True.</span></span>
    - <span data-ttu-id="11aab-214">"New-AzVirtualWan"</span><span class="sxs-lookup"><span data-stu-id="11aab-214">'New-AzVirtualWan'</span></span>
    - <span data-ttu-id="11aab-215">"Update-AzVirtualWan"</span><span class="sxs-lookup"><span data-stu-id="11aab-215">'Update-AzVirtualWan'</span></span>
* <span data-ttu-id="11aab-216">Foram adicionados cmdlets para suportar o grupo de zonas DNS para pontos finais privados</span><span class="sxs-lookup"><span data-stu-id="11aab-216">Added new cmdlets to support DNS zone group for private endpoint</span></span>
    - <span data-ttu-id="11aab-217">"New-AzPrivateDnsZoneConfig"</span><span class="sxs-lookup"><span data-stu-id="11aab-217">'New-AzPrivateDnsZoneConfig'</span></span>
    - <span data-ttu-id="11aab-218">"Get-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="11aab-218">'Get-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="11aab-219">"New-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="11aab-219">'New-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="11aab-220">"Set-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="11aab-220">'Set-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="11aab-221">"Remove-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="11aab-221">'Remove-AzPrivateDnsZoneGroup'</span></span>
* <span data-ttu-id="11aab-222">Foram adicionados os parâmetros "DNSEnableProxy", "DNSRequireProxyForNetworkRules" e "DNSServers" a "AzureFirewall"</span><span class="sxs-lookup"><span data-stu-id="11aab-222">Added 'DNSEnableProxy', 'DNSRequireProxyForNetworkRules' and 'DNSServers' parameters to 'AzureFirewall'</span></span>
* <span data-ttu-id="11aab-223">Foram adicionados os parâmetros "EnableDnsProxy", "DnsProxyNotRequiredForNetworkRule" e "DnsServer" a "AzureFirewall"</span><span class="sxs-lookup"><span data-stu-id="11aab-223">Added 'EnableDnsProxy', 'DnsProxyNotRequiredForNetworkRule' and 'DnsServer' parameters to 'AzureFirewall'</span></span>
    - <span data-ttu-id="11aab-224">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="11aab-224">Updated cmdlet:</span></span>
        - <span data-ttu-id="11aab-225">New-AzFirewall</span><span class="sxs-lookup"><span data-stu-id="11aab-225">New-AzFirewall</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="11aab-226">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="11aab-226">Az.OperationalInsights</span></span>
* <span data-ttu-id="11aab-227">O código legado foi atualizado para aplicar o SDK recém-gerado</span><span class="sxs-lookup"><span data-stu-id="11aab-227">Updated legacy code to apply new generated SDK</span></span>
* <span data-ttu-id="11aab-228">Foram eliminados cmdlets devido a APIs preteridas</span><span class="sxs-lookup"><span data-stu-id="11aab-228">Deleted cmdlets due to deprecated APIs</span></span>
    - <span data-ttu-id="11aab-229">"Get-AzOperationalInsightsSavedSearchResult" (alias "Get-AzOperationalInsightsSavedSearchResults")</span><span class="sxs-lookup"><span data-stu-id="11aab-229">'Get-AzOperationalInsightsSavedSearchResult' (alias 'Get-AzOperationalInsightsSavedSearchResults')</span></span>
    - <span data-ttu-id="11aab-230">"Get-AzOperationalInsightsSearchResult" (alias "Get-AzOperationalInsightsSearchResults")</span><span class="sxs-lookup"><span data-stu-id="11aab-230">'Get-AzOperationalInsightsSearchResult' (alias 'Get-AzOperationalInsightsSearchResults')</span></span>
    - <span data-ttu-id="11aab-231">"Get-AzOperationalInsightsLinkTarget" (alias "Get-AzOperationalInsightsLinkTargets")</span><span class="sxs-lookup"><span data-stu-id="11aab-231">'Get-AzOperationalInsightsLinkTarget' (alias 'Get-AzOperationalInsightsLinkTargets')</span></span>
* <span data-ttu-id="11aab-232">Foram adicionados parâmetros para "Set-AzOperationalInsightsWorkspace" e "New-AzOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="11aab-232">Added parameters for 'Set-AzOperationalInsightsWorkspace' and 'New-AzOperationalInsightsWorkspace'</span></span>
* <span data-ttu-id="11aab-233">Foram criados cmdlets para a Conta de Armazenamento Associada</span><span class="sxs-lookup"><span data-stu-id="11aab-233">Created cmdlets for Linked Stoarge Account</span></span>
* <span data-ttu-id="11aab-234">Foram criados cmdlets para Clusters e para o Serviço Associado</span><span class="sxs-lookup"><span data-stu-id="11aab-234">Created cmdlets for Clusters and Linked Service</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="11aab-235">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="11aab-235">Az.RecoveryServices</span></span>
* <span data-ttu-id="11aab-236">O Azure Site Recovery adicionou suporte para proteger máquinas virtuais de grupo de colocação por proximidade para fornecedor do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-236">Azure Site Recovery added support for protecting proximity placement group virtual machines for Azure to Azure provider.</span></span>
* <span data-ttu-id="11aab-237">O Azure Site Recovery adicionou suporte para a replicação de zona para zona.</span><span class="sxs-lookup"><span data-stu-id="11aab-237">Azure Site Recovery added support for zone to zone replication.</span></span>
* <span data-ttu-id="11aab-238">O Azure Backup adicionou suporte para a retenção de longo prazo para Pontos de Recuperação de Partilhas de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-238">Azure Backup Added Long term retention support for Azure FileShare Recovery Points.</span></span>
* <span data-ttu-id="11aab-239">O Azure Backup adicionou propriedades de exclusão de discos à saída do cmdlet "Get-AzRecoveryServicesBackupItem".</span><span class="sxs-lookup"><span data-stu-id="11aab-239">Azure Backup Added disk exclusion properties to 'Get-AzRecoveryServicesBackupItem' cmdlet output.</span></span>
* <span data-ttu-id="11aab-240">Foi adicionado o ponto final privado para o ficheiro de credenciais de Cofre para o Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="11aab-240">Added private endpoint for Vault credential file for site recovery service.</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-241">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-241">Az.Resources</span></span>
* <span data-ttu-id="11aab-242">Foi adicionado um aviso de mensagem relativo a um atraso na vista ao criar uma Definição de Função nova</span><span class="sxs-lookup"><span data-stu-id="11aab-242">Added message warning about view delay when creating a new Role Definition</span></span>
* <span data-ttu-id="11aab-243">Os cmdlets de política foram alterados para produzir objetos de tipos compatíveis</span><span class="sxs-lookup"><span data-stu-id="11aab-243">Changed policy cmdlets to output strongly-typed objects</span></span>
* <span data-ttu-id="11aab-244">Foi removido o parâmetro "-TenantLevel" utilizado no cmdlet "Get-AzResourceLock" [#11335]</span><span class="sxs-lookup"><span data-stu-id="11aab-244">Removed '-TenantLevel' parameter used for on the 'Get-AzResourceLock' cmdlet [#11335]</span></span>
* <span data-ttu-id="11aab-245">"Remove-AzResourceGroup -Id ResourceId" foi corrigido [#9882]</span><span class="sxs-lookup"><span data-stu-id="11aab-245">Fixed 'Remove-AzResourceGroup -Id ResourceId'[#9882]</span></span>
* <span data-ttu-id="11aab-246">Foi adicionado um cmdlet novo para obter resultados de What-If de modelos do ARM no âmbito de um grupo de recursos: "Get-AzDeploymentResourceGroupWhatIfResult"</span><span class="sxs-lookup"><span data-stu-id="11aab-246">Added new cmdlet for getting ARM template What-If results at resource group scope: 'Get-AzDeploymentResourceGroupWhatIfResult'</span></span>
* <span data-ttu-id="11aab-247">Foi adicionado um cmdlet novo para obter resultados de What-If de modelos do ARM no âmbito de uma subscrição: "Get-AzDeploymentWhatIfResult"</span><span class="sxs-lookup"><span data-stu-id="11aab-247">Added new cmdlet for getting ARM template What-If results at subscription scope: 'Get-AzDeploymentWhatIfResult'</span></span>
   - <span data-ttu-id="11aab-248">Alias: "Get-AzSubscriptionDeploymentWhatIf"</span><span class="sxs-lookup"><span data-stu-id="11aab-248">Alias: 'Get-AzSubscriptionDeploymentWhatIf'</span></span>
* <span data-ttu-id="11aab-249">Os parâmetros "-WhatIf" e "-Confirm" foram substituídos para "New-AzDeployment" e "New-AzResourceGroupDeployment" para utilizar resultados de What-If de modelos do ARM</span><span class="sxs-lookup"><span data-stu-id="11aab-249">Overrode '-WhatIf' and '-Confirm' parameters for 'New-AzDeployment' and 'New-AzResourceGroupDeployment' to use ARM template What-If results</span></span>
* <span data-ttu-id="11aab-250">Foi adicionada a mensagem de descontinuação para o parâmetro "ApiVersion" em cmdlets implementados</span><span class="sxs-lookup"><span data-stu-id="11aab-250">Added deprecation message for 'ApiVersion' parameter in deployment cmdlets</span></span>
* <span data-ttu-id="11aab-251">Foi adicionada a capacidade para mostrar mensagens de erro melhoradas relativas a falhas em implementações</span><span class="sxs-lookup"><span data-stu-id="11aab-251">Added capability to show improved error messages for deployment failures</span></span>
* <span data-ttu-id="11aab-252">Foi adicionado o registo de correlationId para falhas em implementações</span><span class="sxs-lookup"><span data-stu-id="11aab-252">Added correlationId logging for deployment failures</span></span>
* <span data-ttu-id="11aab-253">Foi adicionada a propriedade "error" à saída do script de implementação</span><span class="sxs-lookup"><span data-stu-id="11aab-253">Added 'error' property to the deployment script output</span></span>
* <span data-ttu-id="11aab-254">O nuget Microsoft.Azure.Management.ResourceManager foi atualizado para "3.7.1-preview"</span><span class="sxs-lookup"><span data-stu-id="11aab-254">Updated nuget Microsoft.Azure.Management.ResourceManager to '3.7.1-preview'</span></span>
* <span data-ttu-id="11aab-255">Foram removidos casos de teste específicos, uma vez que a propriedade Error em DeploymentValidateResult foi alterada para apenas de leitura a partir de 3.7.1-preview</span><span class="sxs-lookup"><span data-stu-id="11aab-255">Removed specific test cases as Error property in DeploymentValidateResult has changed to readonly from nuget 3.7.1-preview</span></span>
* <span data-ttu-id="11aab-256">GenericResourceExpanded foi importado do SDK ResourceManager 3.7.1-preview</span><span class="sxs-lookup"><span data-stu-id="11aab-256">Brought GenericResourceExpanded from SDK ResourceManager 3.7.1-preview</span></span>
* <span data-ttu-id="11aab-257">Foi adicionado suporte para etiquetas a todos os cmdlets Get para implementação, bem como</span><span class="sxs-lookup"><span data-stu-id="11aab-257">Added tag support for all Get cmdlets for deployment, as well as</span></span>
    - <span data-ttu-id="11aab-258">"New-AzDeployment"</span><span class="sxs-lookup"><span data-stu-id="11aab-258">'New-AzDeployment'</span></span>
    - <span data-ttu-id="11aab-259">"New-AzManagementGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="11aab-259">'New-AzManagementGroupDeployment'</span></span>
    - <span data-ttu-id="11aab-260">"New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="11aab-260">'New-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="11aab-261">"New-AzTenantDeployment"</span><span class="sxs-lookup"><span data-stu-id="11aab-261">'New-AzTenantDeployment'</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="11aab-262">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="11aab-262">Az.ServiceFabric</span></span>
* <span data-ttu-id="11aab-263">Foi corrigido um erro na adição de certificados mediante a utilização de --SecretIdentifier que obtinha o thumbprint de certificado incorreto</span><span class="sxs-lookup"><span data-stu-id="11aab-263">Fixed bug in add certificate using --SecretIdentifier that was getting the wrong certificate thumbprint</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-264">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-264">Az.Sql</span></span>
* <span data-ttu-id="11aab-265">Foi melhorado o desempenho de:</span><span class="sxs-lookup"><span data-stu-id="11aab-265">Enhance performance of:</span></span>
    - <span data-ttu-id="11aab-266">"Set-AzSqlDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="11aab-266">'Set-AzSqlDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="11aab-267">"Set-AzSqlInstanceDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="11aab-267">'Set-AzSqlInstanceDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="11aab-268">"Remove-AzSqlDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="11aab-268">'Remove-AzSqlDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="11aab-269">"Remove-AzSqlInstanceDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="11aab-269">'Remove-AzSqlInstanceDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="11aab-270">"Enable-AzSqlDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="11aab-270">'Enable-AzSqlDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="11aab-271">"Enable-AzSqlInstanceDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="11aab-271">'Enable-AzSqlInstanceDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="11aab-272">"Disable-AzSqlDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="11aab-272">'Disable-AzSqlDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="11aab-273">"Disable-AzSqlInstanceDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="11aab-273">'Disable-AzSqlInstanceDatabaseSensitivityRecommendation'</span></span>
* <span data-ttu-id="11aab-274">Foi removida a validação do lado do cliente do parâmetro "RetentionDays" do cmdlet "Set-AzSqlDatabaseBackupShortTermRetentionPolicy"</span><span class="sxs-lookup"><span data-stu-id="11aab-274">Removed client-side validation of 'RetentionDays' parameter from cmdlet 'Set-AzSqlDatabaseBackupShortTermRetentionPolicy'</span></span>
* <span data-ttu-id="11aab-275">Auditoria a uma conta de armazenamento na Vnet; corrigido um erro ao criar uma função de Contribuidor de Dados de Blobs de Armazenamento.</span><span class="sxs-lookup"><span data-stu-id="11aab-275">Auditing to a storage account in Vnet, fixing a bug when creating a Storage Blob Data Contributor role.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="11aab-276">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-276">Az.Storage</span></span>
* <span data-ttu-id="11aab-277">Foi adicionado "-AsJob" ao cmdlet para obter/listar contas "Get-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="11aab-277">Added '-AsJob' to get/list account cmdlet 'Get-AzStorageAccount'</span></span>
* <span data-ttu-id="11aab-278">KeyVersion foi tornado opcional ao atualizar a conta de Armazenamento com KeyvaultEncryption, para suportar a rotação automática de chaves</span><span class="sxs-lookup"><span data-stu-id="11aab-278">Make KeyVersion to optional when update Storage account with KeyvaultEncryption, to support key auto-rotation</span></span>
    - <span data-ttu-id="11aab-279">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="11aab-279">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="11aab-280">Corrigida a remoção de falha do Diretório de Ficheiros do Azure com o pipeline</span><span class="sxs-lookup"><span data-stu-id="11aab-280">Fixed remove Azure File Directory fail with pipeline</span></span>
    - <span data-ttu-id="11aab-281">"Remove-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="11aab-281">'Remove-AzStorageDirectory'</span></span>
* <span data-ttu-id="11aab-282">Corrigido [#9880]: A definição do valor DefaultAction de NetWorkRule foi alterado para estar alinhado com o swagger.</span><span class="sxs-lookup"><span data-stu-id="11aab-282">Fixed [#9880]: Change NetWorkRule DefaultAction value defination to align with swagger.</span></span>
    - <span data-ttu-id="11aab-283">"Update-AzStorageAccountNetworkRuleSet"</span><span class="sxs-lookup"><span data-stu-id="11aab-283">'Update-AzStorageAccountNetworkRuleSet'</span></span>
    - <span data-ttu-id="11aab-284">"Get-AzStorageAccountNetworkRuleSet"</span><span class="sxs-lookup"><span data-stu-id="11aab-284">'Get-AzStorageAccountNetworkRuleSet'</span></span>
* <span data-ttu-id="11aab-285">Corrigido [#11624]: Ignorar regras duplicadas ao adicionar NetworkRules, para evitar falhas de servidores</span><span class="sxs-lookup"><span data-stu-id="11aab-285">Fixed [#11624]: Skip duplicated rules when add NetworkRules, to avoid server failure</span></span>
    - <span data-ttu-id="11aab-286">"Add-AzStorageAccountNetworkRule"</span><span class="sxs-lookup"><span data-stu-id="11aab-286">'Add-AzStorageAccountNetworkRule'</span></span>
* <span data-ttu-id="11aab-287">O SDK Microsoft.Azure.Cosmos.Table foi atualizado para 1.0.7</span><span class="sxs-lookup"><span data-stu-id="11aab-287">Upgraded Microsoft.Azure.Cosmos.Table SDK to 1.0.7</span></span>
* <span data-ttu-id="11aab-288">Foi adicionada uma mensagem de aviso para relembrar o utilizador para listar novamente com ContinuationToken apenas quando são devolvidos itens de peças na lista DataLake Gen2 Items,</span><span class="sxs-lookup"><span data-stu-id="11aab-288">Added a warning message to remind user to list again with ContinuationToken when only part items are returned in list DataLake Gen2 Items,</span></span>
    - <span data-ttu-id="11aab-289">"Get-AzDataLakeGen2ChildItem"</span><span class="sxs-lookup"><span data-stu-id="11aab-289">'Get-AzDataLakeGen2ChildItem'</span></span>
* <span data-ttu-id="11aab-290">Suportado para criar ou atualizar a conta de Armazenamento com a Autenticação do Active Directory Domain Service dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="11aab-290">Supported to create or update Storage account with Azure Files Active Directory Domain Service Authentication</span></span>
    -  <span data-ttu-id="11aab-291">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="11aab-291">'New-AzStorageAccount'</span></span>
    -  <span data-ttu-id="11aab-292">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="11aab-292">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="11aab-293">Suportado para os comandos "new" ou "list" de chaves de Kerberos da conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="11aab-293">Supported to new or list Kerberos keys of Storage account</span></span>
    -  <span data-ttu-id="11aab-294">"New-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="11aab-294">'New-AzStorageAccountKey'</span></span>
    -  <span data-ttu-id="11aab-295">"Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="11aab-295">'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="11aab-296">Suportada conta de Armazenamento de ativação pós-falha</span><span class="sxs-lookup"><span data-stu-id="11aab-296">Supported failover Storage account</span></span>
    - <span data-ttu-id="11aab-297">"Invoke-AzStorageAccountFailover"</span><span class="sxs-lookup"><span data-stu-id="11aab-297">'Invoke-AzStorageAccountFailover'</span></span>
* <span data-ttu-id="11aab-298">Ajuda de "Get-AzStorageBlobCopyState" atualizada</span><span class="sxs-lookup"><span data-stu-id="11aab-298">Updated help of 'Get-AzStorageBlobCopyState'</span></span>
* <span data-ttu-id="11aab-299">Ajuda de "Get-AzStorageFileCopyState" e "Start-AzStorageBlobCopy" atualizada</span><span class="sxs-lookup"><span data-stu-id="11aab-299">Updated help of 'Get-AzStorageFileCopyState' and 'Start-AzStorageBlobCopy'</span></span>
* <span data-ttu-id="11aab-300">Integração da biblioteca de cliente do Armazenamento v12 para cmdlets de Filas e Ficheiros</span><span class="sxs-lookup"><span data-stu-id="11aab-300">Integrated Storage client library v12 to Queue and File cmdlets</span></span>
* <span data-ttu-id="11aab-301">Alteração ao tipo de saída de CloudFile para AzureStorageFile; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="11aab-301">Changed output type from CloudFile to AzureStorageFile, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="11aab-302">"Get-AzStorageFile"</span><span class="sxs-lookup"><span data-stu-id="11aab-302">'Get-AzStorageFile'</span></span>
    - <span data-ttu-id="11aab-303">"Remove-AzStorageFile"</span><span class="sxs-lookup"><span data-stu-id="11aab-303">'Remove-AzStorageFile'</span></span>
    - <span data-ttu-id="11aab-304">"Get-AzStorageFileContent"</span><span class="sxs-lookup"><span data-stu-id="11aab-304">'Get-AzStorageFileContent'</span></span>
    - <span data-ttu-id="11aab-305">"Set-AzStorageFileContent"</span><span class="sxs-lookup"><span data-stu-id="11aab-305">'Set-AzStorageFileContent'</span></span>
    - <span data-ttu-id="11aab-306">"Start-AzStorageFileCopy"</span><span class="sxs-lookup"><span data-stu-id="11aab-306">'Start-AzStorageFileCopy'</span></span>
* <span data-ttu-id="11aab-307">Alteração ao tipo de saída de CloudFileDirectory para AzureStorageFileDirectory; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="11aab-307">Changed output type from CloudFileDirectory to AzureStorageFileDirectory, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="11aab-308">"New-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="11aab-308">'New-AzStorageDirectory'</span></span>
    - <span data-ttu-id="11aab-309">"Remove-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="11aab-309">'Remove-AzStorageDirectory'</span></span>
* <span data-ttu-id="11aab-310">Alteração ao tipo de saída de CloudFileShare para AzureStorageFileShare; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="11aab-310">Changed output type from CloudFileShare to AzureStorageFileShare, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="11aab-311">"Get-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="11aab-311">'Get-AzStorageShare'</span></span>
    - <span data-ttu-id="11aab-312">"New-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="11aab-312">'New-AzStorageShare'</span></span>
    - <span data-ttu-id="11aab-313">"Remove-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="11aab-313">'Remove-AzStorageShare'</span></span>
* <span data-ttu-id="11aab-314">Alteração ao tipo de saída de FileShareProperties para AzureStorageFileShare; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="11aab-314">Changed output type from FileShareProperties to AzureStorageFileShare, the original output will become a sub child property of the new output</span></span>
    - <span data-ttu-id="11aab-315">"Set-AzStorageShareQuota"</span><span class="sxs-lookup"><span data-stu-id="11aab-315">'Set-AzStorageShareQuota'</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="11aab-316">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="11aab-316">Az.TrafficManager</span></span>
* <span data-ttu-id="11aab-317">Corrigido o nome de perfil errado na saída verbosa de "DisableAzureTrafficManagerEndpoint"</span><span class="sxs-lookup"><span data-stu-id="11aab-317">Fixed incorrect profile name in 'DisableAzureTrafficManagerEndpoint' verbose output</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="11aab-318">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="11aab-318">Az.Websites</span></span>
* <span data-ttu-id="11aab-319">Corrigido um erro ortográfico na ajuda de "Update-AzWebAppAccessRestrictionConfig".</span><span class="sxs-lookup"><span data-stu-id="11aab-319">Fixed typo on help of 'Update-AzWebAppAccessRestrictionConfig'.</span></span>

## <a name="380---april-2020"></a><span data-ttu-id="11aab-320">3.8.0 - Abril de 2020</span><span class="sxs-lookup"><span data-stu-id="11aab-320">3.8.0 - April 2020</span></span>
### <a name="highlights-since-the-last-release"></a><span data-ttu-id="11aab-321">Destaques desde a última versão</span><span class="sxs-lookup"><span data-stu-id="11aab-321">Highlights since the last release</span></span>
* <span data-ttu-id="11aab-322">Versões do Powershell suportadas pelo Az.Storage: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span><span class="sxs-lookup"><span data-stu-id="11aab-322">PowerShell versions that Az.Storage supports: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="11aab-323">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-323">Az.Accounts</span></span>
* <span data-ttu-id="11aab-324">Atualização do URL de inquérito do Azure PowerShell em "Resolve-AzError" [#11507]</span><span class="sxs-lookup"><span data-stu-id="11aab-324">Updated Azure PowerShell survey URL in 'Resolve-AzError' [#11507]</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="11aab-325">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="11aab-325">Az.ApiManagement</span></span>
* <span data-ttu-id="11aab-326">Adicionado aviso de alteração interruptiva para a alteração de resultados de cmdlets de Ficheiro do Azure numa versão futura</span><span class="sxs-lookup"><span data-stu-id="11aab-326">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="11aab-327">Documentação atualizada de "Set-AzApiManagementGroup" para especificar o parâmetro GroupId</span><span class="sxs-lookup"><span data-stu-id="11aab-327">'Set-AzApiManagementGroup' Updated documentation to specify the GroupId parameter</span></span>

#### <a name="azcdn"></a><span data-ttu-id="11aab-328">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="11aab-328">Az.Cdn</span></span>
* <span data-ttu-id="11aab-329">Correção da apresentação do SKU de preços relacionados com ChinaCDN</span><span class="sxs-lookup"><span data-stu-id="11aab-329">Fixed ChinaCDN related pricing SKU display</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="11aab-330">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="11aab-330">Az.CognitiveServices</span></span>
* <span data-ttu-id="11aab-331">Suporte para Identidade, Encriptação, UserOwnedStorage</span><span class="sxs-lookup"><span data-stu-id="11aab-331">Supported Identity, Encryption, UserOwnedStorage</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-332">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-332">Az.Compute</span></span>
* <span data-ttu-id="11aab-333">Adicionado o cmdlet "Set-AzVmssOrchestrationServiceState".</span><span class="sxs-lookup"><span data-stu-id="11aab-333">Added 'Set-AzVmssOrchestrationServiceState' cmdlet.</span></span>
* <span data-ttu-id="11aab-334">"Get-AzVmss" com -InstanceView mostra os estados de OrchestrationService.</span><span class="sxs-lookup"><span data-stu-id="11aab-334">'Get-AzVmss' with -InstanceView shows OrchestrationService states.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="11aab-335">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="11aab-335">Az.IotHub</span></span>
* <span data-ttu-id="11aab-336">Gestão da configuração do dispositivo duplo de IoT. Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="11aab-336">Manage IoT device twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="11aab-337">"Get-AzIotHubDeviceTwin"</span><span class="sxs-lookup"><span data-stu-id="11aab-337">'Get-AzIotHubDeviceTwin'</span></span>
    - <span data-ttu-id="11aab-338">"Update-AzIotHubDeviceTwin"</span><span class="sxs-lookup"><span data-stu-id="11aab-338">'Update-AzIotHubDeviceTwin'</span></span>
* <span data-ttu-id="11aab-339">Adicionado cmdlet para invocar o método direto num dispositivo num hub IoT.</span><span class="sxs-lookup"><span data-stu-id="11aab-339">Added cmdlet to invoke direct method on a device in an Iot Hub.</span></span>
* <span data-ttu-id="11aab-340">Gestão da configuração do módulo duplo do dispositivo de IoT. Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="11aab-340">Manage IoT device module twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="11aab-341">"Get-AzIotHubModuleTwin"</span><span class="sxs-lookup"><span data-stu-id="11aab-341">'Get-AzIotHubModuleTwin'</span></span>
    - <span data-ttu-id="11aab-342">"Update-AzIotHubModuleTwin"</span><span class="sxs-lookup"><span data-stu-id="11aab-342">'Update-AzIotHubModuleTwin'</span></span>
* <span data-ttu-id="11aab-343">Gestão da configuração da gestão automática de dispositivos IoT em escala.</span><span class="sxs-lookup"><span data-stu-id="11aab-343">Manage IoT automatic device management configuration at scale.</span></span> <span data-ttu-id="11aab-344">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="11aab-344">New cmdlets are:</span></span>
    - <span data-ttu-id="11aab-345">"Add-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="11aab-345">'Add-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="11aab-346">"Get-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="11aab-346">'Get-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="11aab-347">"Remove-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="11aab-347">'Remove-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="11aab-348">"Set-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="11aab-348">'Set-AzIotHubConfiguration'</span></span>
* <span data-ttu-id="11aab-349">Adicionado cmdlet para invocar um método de módulo de periferia num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="11aab-349">Added cmdlet to invoke an edge module method in an Iot Hub.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="11aab-350">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="11aab-350">Az.KeyVault</span></span>
* <span data-ttu-id="11aab-351">Adicionado um novo cmdlet "Update-AzKeyVault" que pode permitir a eliminação recuperável e a proteção contra remoções num cofre</span><span class="sxs-lookup"><span data-stu-id="11aab-351">Added a new cmdlet 'Update-AzKeyVault' that can enable soft delete and purge protection on a vault</span></span>
* <span data-ttu-id="11aab-352">Adicionado suporte para Microsoft.PowerShell.SecretManagement [#11178]</span><span class="sxs-lookup"><span data-stu-id="11aab-352">Added support to Microsoft.PowerShell.SecretManagement [#11178]</span></span>
* <span data-ttu-id="11aab-353">Correção do erro nos exemplos de "Remove-AzKeyVaultManagedStorageSasDefinition" [#11479]</span><span class="sxs-lookup"><span data-stu-id="11aab-353">Fixed error in the examples of 'Remove-AzKeyVaultManagedStorageSasDefinition' [#11479]</span></span>
* <span data-ttu-id="11aab-354">Adicionado suporte para o ponto final privado</span><span class="sxs-lookup"><span data-stu-id="11aab-354">Added support to private endpoint</span></span>

#### <a name="azmaintenance"></a><span data-ttu-id="11aab-355">Az.Maintenance</span><span class="sxs-lookup"><span data-stu-id="11aab-355">Az.Maintenance</span></span>
* <span data-ttu-id="11aab-356">Publicação da versão de lançamento dos cmdlets de Manutenção para Disponibilidade Geral</span><span class="sxs-lookup"><span data-stu-id="11aab-356">Publishing release version of Maintenance cmdlets for GA</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="11aab-357">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="11aab-357">Az.Monitor</span></span>
* <span data-ttu-id="11aab-358">Adicionados cmdlets para o âmbito de ligação privada</span><span class="sxs-lookup"><span data-stu-id="11aab-358">Added cmdlets for private link scope</span></span>
    - <span data-ttu-id="11aab-359">"Get-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="11aab-359">'Get-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="11aab-360">"Remove-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="11aab-360">'Remove-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="11aab-361">"New-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="11aab-361">'New-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="11aab-362">"Update-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="11aab-362">'Update-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="11aab-363">"Get-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="11aab-363">'Get-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="11aab-364">"New-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="11aab-364">'New-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="11aab-365">"Remove-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="11aab-365">'Remove-AzInsightsPrivateLinkScopedResource'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-366">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-366">Az.Network</span></span>
* <span data-ttu-id="11aab-367">Atualização dos cmdlets para permitir a ligação num IP privado para o Gateway de Rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="11aab-367">Updated cmdlets to enable connection on private IP for Virtual Network Gateway.</span></span>
    - <span data-ttu-id="11aab-368">"New-AzVirtualNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="11aab-368">'New-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="11aab-369">"Set-AzVirtualNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="11aab-369">'Set-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="11aab-370">"New-AzVirtualNetworkGatewayConnection"</span><span class="sxs-lookup"><span data-stu-id="11aab-370">'New-AzVirtualNetworkGatewayConnection'</span></span>
    - <span data-ttu-id="11aab-371">"Set-AzVirtualNetworkGatewayConnection"</span><span class="sxs-lookup"><span data-stu-id="11aab-371">'Set-AzVirtualNetworkGatewayConnection'</span></span>
* <span data-ttu-id="11aab-372">Atualização dos cmdlets para permitir LocalNetworkGateways e VpnSites com base em FQDN</span><span class="sxs-lookup"><span data-stu-id="11aab-372">Updated cmdlets to enable FQDN based LocalNetworkGateways and VpnSites</span></span>
    - <span data-ttu-id="11aab-373">"New-AzLocalNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="11aab-373">'New-AzLocalNetworkGateway'</span></span>
    - <span data-ttu-id="11aab-374">"New-AzVpnSiteLink"</span><span class="sxs-lookup"><span data-stu-id="11aab-374">'New-AzVpnSiteLink'</span></span>
* <span data-ttu-id="11aab-375">Adicionado suporte para a família de endereços IPv6 em ExpressRouteCircuitConnectionConfig (Alcance Global)</span><span class="sxs-lookup"><span data-stu-id="11aab-375">Added support for IPv6 address family in ExpressRouteCircuitConnectionConfig (Global Reach)</span></span>
    - <span data-ttu-id="11aab-376">Adicionado "Set-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="11aab-376">Added 'Set-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="11aab-377">permite a definição de todas as propriedades existentes, incluindo o IPv6CircuitConnectionProperties</span><span class="sxs-lookup"><span data-stu-id="11aab-377">allows setting of all the existing properties including the IPv6CircuitConnectionProperties</span></span>
    - <span data-ttu-id="11aab-378">Atualização de "Add-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="11aab-378">Updated 'Add-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="11aab-379">Adicionado outro parâmetro opcional AddressPrefixType para especificar a família de endereços do prefixo de endereço</span><span class="sxs-lookup"><span data-stu-id="11aab-379">Added another optional parameter AddressPrefixType to specify the address family of address prefix</span></span>
* <span data-ttu-id="11aab-380">Atualização dos cmdlets para permitir a definição do Tempo Limite de DPD nas Ligações do Gateway de Rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="11aab-380">Updated cmdlets to enable setting of DPD Timeout on Virtual Network Gateway Connections.</span></span>
    - <span data-ttu-id="11aab-381">New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-381">New-AzVirtualNetworkGatewayConnection</span></span>
    - <span data-ttu-id="11aab-382">Set-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-382">Set-AzVirtualNetworkGatewayConnection</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="11aab-383">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="11aab-383">Az.PolicyInsights</span></span>
* <span data-ttu-id="11aab-384">Adicionado o cmdlet "Start-AzPolicyComplianceScan" para acionar análises de conformidade de políticas</span><span class="sxs-lookup"><span data-stu-id="11aab-384">Added 'Start-AzPolicyComplianceScan' cmdlet for triggering policy compliance scans</span></span>
* <span data-ttu-id="11aab-385">Adição de definição de políticas, definição de conjuntos e versões de atribuição ao resultado de "Get-AzPolicyState"</span><span class="sxs-lookup"><span data-stu-id="11aab-385">Added policy definition, set definition, and assignment versions to 'Get-AzPolicyState' output</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="11aab-386">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="11aab-386">Az.ServiceFabric</span></span>
* <span data-ttu-id="11aab-387">Melhorias da formatação e usabilidade do código dos exemplos de "New-AzServiceFabricCluster"</span><span class="sxs-lookup"><span data-stu-id="11aab-387">Improved code formatting and usability of 'New-AzServiceFabricCluster' examples</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-388">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-388">Az.Sql</span></span>
* <span data-ttu-id="11aab-389">Adicionados os cmdlets "Get-AzSqlInstanceOperation" e "Stop-AzSqlInstanceOperation"</span><span class="sxs-lookup"><span data-stu-id="11aab-389">Added cmdlets 'Get-AzSqlInstanceOperation' and 'Stop-AzSqlInstanceOperation'</span></span>
* <span data-ttu-id="11aab-390">Suporte de auditorias a uma conta de armazenamento numa VNet.</span><span class="sxs-lookup"><span data-stu-id="11aab-390">Supported auditing to a storage account in VNet.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="11aab-391">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-391">Az.Storage</span></span>
* <span data-ttu-id="11aab-392">Adicionado aviso de alteração interruptiva para a alteração de resultados de cmdlets de Ficheiro do Azure numa versão futura</span><span class="sxs-lookup"><span data-stu-id="11aab-392">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="11aab-393">Suportado novo SkuName StandardGZRS, StandardRAGZRS ao criar/atualizar a Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="11aab-393">Supported new SkuName StandardGZRS, StandardRAGZRS when create/update Storage account</span></span>
    - <span data-ttu-id="11aab-394">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="11aab-394">'New-AzStorageAccount'</span></span>
    - <span data-ttu-id="11aab-395">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="11aab-395">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="11aab-396">Suportado o DataLake Gen2</span><span class="sxs-lookup"><span data-stu-id="11aab-396">Supported DataLake Gen2</span></span>
    - <span data-ttu-id="11aab-397">"New-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="11aab-397">'New-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="11aab-398">"Get-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="11aab-398">'Get-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="11aab-399">"Get-AzDataLakeGen2ChildItem"</span><span class="sxs-lookup"><span data-stu-id="11aab-399">'Get-AzDataLakeGen2ChildItem'</span></span>
    - <span data-ttu-id="11aab-400">"Move-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="11aab-400">'Move-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="11aab-401">"Set-AzDataLakeGen2ItemAclObject"</span><span class="sxs-lookup"><span data-stu-id="11aab-401">'Set-AzDataLakeGen2ItemAclObject'</span></span>
    - <span data-ttu-id="11aab-402">"Update-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="11aab-402">'Update-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="11aab-403">"Get-AzDataLakeGen2ItemContent"</span><span class="sxs-lookup"><span data-stu-id="11aab-403">'Get-AzDataLakeGen2ItemContent'</span></span>
    - <span data-ttu-id="11aab-404">"Remove-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="11aab-404">'Remove-AzDataLakeGen2Item'</span></span>

## <a name="0100-preview---april-2020"></a><span data-ttu-id="11aab-405">0.10.0-preview - Abril de 2020</span><span class="sxs-lookup"><span data-stu-id="11aab-405">0.10.0-preview - April 2020</span></span>
### <a name="general"></a><span data-ttu-id="11aab-406">Geral</span><span class="sxs-lookup"><span data-stu-id="11aab-406">General</span></span>
* <span data-ttu-id="11aab-407">Os módulos Az já estão disponíveis em pré-visualização no Azure Stack Hub.</span><span class="sxs-lookup"><span data-stu-id="11aab-407">Az modules is now available in preview on Azure Stack Hub.</span></span> <span data-ttu-id="11aab-408">Isto permite a compatibilidade entre plataformas diferentes com o Linux e macOS.</span><span class="sxs-lookup"><span data-stu-id="11aab-408">This allows for cross-platform compatibility with Linux and macOs.</span></span> <span data-ttu-id="11aab-409">Agora, o Azure Stack Hub suporta o PowerShell Core com os módulos Az. Obtenha mais informações [aqui](https://aka.ms/az4AzureStack)</span><span class="sxs-lookup"><span data-stu-id="11aab-409">Azure Stack Hub now supports PowerShell core with the Az modules, more information [here](https://aka.ms/az4AzureStack)</span></span>
* <span data-ttu-id="11aab-410">Os módulos Az suportam o perfil 2019-03-01-hybrid:</span><span class="sxs-lookup"><span data-stu-id="11aab-410">Az modules support profile 2019-03-01-hybrid:</span></span>
  - <span data-ttu-id="11aab-411">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="11aab-411">Az.Billing</span></span>
  - <span data-ttu-id="11aab-412">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-412">Az.Compute</span></span>
  - <span data-ttu-id="11aab-413">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="11aab-413">Az.DataBoxEdge</span></span>
  - <span data-ttu-id="11aab-414">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="11aab-414">Az.EventHub</span></span>
  - <span data-ttu-id="11aab-415">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="11aab-415">Az.IotHub</span></span>
  - <span data-ttu-id="11aab-416">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="11aab-416">Az.KeyVault</span></span>
  - <span data-ttu-id="11aab-417">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="11aab-417">Az.Monitor</span></span>
  - <span data-ttu-id="11aab-418">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-418">Az.Network</span></span>
  - <span data-ttu-id="11aab-419">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-419">Az.Resources</span></span>
  - <span data-ttu-id="11aab-420">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-420">Az.Storage</span></span>
  - <span data-ttu-id="11aab-421">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="11aab-421">Az.Websites</span></span>
* <span data-ttu-id="11aab-422">Foram introduzidos três novos módulos do PowerShell para Az que funcionam com o Azure Stack Hub. São eles o Az.Databox, Az.IotHub e Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="11aab-422">Three new PowerShell modules for az have been introduced that work with Azure Stack Hub, which are Az.Databox, Az.IotHub, and Az.EventHub</span></span>
* <span data-ttu-id="11aab-423">Os comandos permanecem sensivelmente iguais, com pequenas alterações como, por exemplo, a alteração do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="11aab-423">Commands remain relatively the same, with minor changes such as changing AzureRM to Az</span></span>
* <span data-ttu-id="11aab-424">Veja uma ligação atualizada à documentação do PowerShell para o Azure Stack Hub [aqui](https://aka.ms/InstallASHPowerShell)</span><span class="sxs-lookup"><span data-stu-id="11aab-424">Updated link to PowerShell documentation for Azure Stack Hub can be found [here](https://aka.ms/InstallASHPowerShell)</span></span>

## <a name="370---march-2020"></a><span data-ttu-id="11aab-425">3.7.0 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="11aab-425">3.7.0 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="11aab-426">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-426">Az.Accounts</span></span>
* <span data-ttu-id="11aab-427">Foram corrigidos os parâmetros "Get-AzTenant"/"Get-AzDefault"/"Set-AzDefault" que emitiam uma NullReferenceException quando a sessão não estava iniciada [#10292]</span><span class="sxs-lookup"><span data-stu-id="11aab-427">Fixed 'Get-AzTenant'/'Get-AzDefault'/'Set-AzDefault' throw NullReferenceException when not login [#10292]</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-428">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-428">Az.Compute</span></span>
* <span data-ttu-id="11aab-429">Foram adicionados os seguintes parâmetros ao cmdlet "New-AzDiskConfig":</span><span class="sxs-lookup"><span data-stu-id="11aab-429">Added the following parameters to 'New-AzDiskConfig' cmdlet:</span></span>
    - <span data-ttu-id="11aab-430">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span><span class="sxs-lookup"><span data-stu-id="11aab-430">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span></span>
* <span data-ttu-id="11aab-431">A propriedade Encryption foi permitida para o parâmetro Target do cmdlet "New-AzGalleryImageVersion".</span><span class="sxs-lookup"><span data-stu-id="11aab-431">Allowed Encryption property to Target parameter of 'New-AzGalleryImageVersion' cmdlet.</span></span>
* <span data-ttu-id="11aab-432">Foi corrigido o problema de tempDisk para os cmdlets "Set-AzVmss" -Reimage e "Invoke-AzVMReimage".</span><span class="sxs-lookup"><span data-stu-id="11aab-432">Fixed tempDisk issue for 'Set-AzVmss' -Reimage and 'Invoke-AzVMReimage' cmdlets.</span></span> <span data-ttu-id="11aab-433">[#11354]</span><span class="sxs-lookup"><span data-stu-id="11aab-433">[#11354]</span></span>
* <span data-ttu-id="11aab-434">Foi adicionado suporte aos cmdlets abaixo para a nova Extensão SAP</span><span class="sxs-lookup"><span data-stu-id="11aab-434">Added support to below cmdlets for new SAP Extension</span></span>
    - <span data-ttu-id="11aab-435">"Set-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="11aab-435">'Set-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="11aab-436">"Get-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="11aab-436">'Get-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="11aab-437">"Remove-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="11aab-437">'Remove-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="11aab-438">"Update-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="11aab-438">'Update-AzVMAEMExtension'</span></span>
* <span data-ttu-id="11aab-439">Foram corrigidos os erros em exemplos do documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="11aab-439">Fixed errors in examples of help document</span></span>
* <span data-ttu-id="11aab-440">É apresentado o valor de cadeia exato para o PowerState da VM no formato de tabela.</span><span class="sxs-lookup"><span data-stu-id="11aab-440">Showed the exact string value for VM PowerState in the table format.</span></span>
* <span data-ttu-id="11aab-441">"New-AzVmssConfig": foi corrigida a serialização da propriedade AutomaticRepairs quando a opção SinglePlacementGroup está desativada.</span><span class="sxs-lookup"><span data-stu-id="11aab-441">'New-AzVmssConfig': fixed serialization of AutomaticRepairs property when SinglePlacementGroup is disabled.</span></span> <span data-ttu-id="11aab-442">[#11257]</span><span class="sxs-lookup"><span data-stu-id="11aab-442">[#11257]</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="11aab-443">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="11aab-443">Az.DataFactory</span></span>
* <span data-ttu-id="11aab-444">Atualização da versão do SDK .Net do ADF para 4.8.0</span><span class="sxs-lookup"><span data-stu-id="11aab-444">Updated ADF .Net SDK version to 4.8.0</span></span>
* <span data-ttu-id="11aab-445">Foram adicionados parâmetros opcionais ao comando "Invoke-AzDataFactoryV2Pipeline" para suportar uma nova execução</span><span class="sxs-lookup"><span data-stu-id="11aab-445">Added optional parameters to 'Invoke-AzDataFactoryV2Pipeline' command to support rerun</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="11aab-446">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="11aab-446">Az.DataLakeStore</span></span>
* <span data-ttu-id="11aab-447">Foi adicionada a descrição da alteração interruptiva para "Export-AzDataLakeStoreItem" e "Import-AzDataLakeStoreItem"</span><span class="sxs-lookup"><span data-stu-id="11aab-447">Added breaking change description for 'Export-AzDataLakeStoreItem' and 'Import-AzDataLakeStoreItem'</span></span>
* <span data-ttu-id="11aab-448">Foi adicionada a opção de codificação de bytes para "New-AzDataLakeStoreItem", "Add-AzDAtaLakeStoreItemContent" e "Get-AzDAtaLakeStoreItemContent"</span><span class="sxs-lookup"><span data-stu-id="11aab-448">Added option of Byte encoding for 'New-AzDataLakeStoreItem', 'Add-AzDAtaLakeStoreItemContent', and 'Get-AzDAtaLakeStoreItemContent'</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="11aab-449">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="11aab-449">Az.HDInsight</span></span>
* <span data-ttu-id="11aab-450">É suportada a versão de TLS mínima suportada ao criar o cluster.</span><span class="sxs-lookup"><span data-stu-id="11aab-450">Supported specifying minimal supported TLS version when creating cluster.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="11aab-451">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="11aab-451">Az.IotHub</span></span>
* <span data-ttu-id="11aab-452">Foi adicionado suporte para gerir as definições distribuídas por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="11aab-452">Added support to manage distributed settings per-device.</span></span> <span data-ttu-id="11aab-453">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="11aab-453">New Cmdlets are:</span></span>
    - <span data-ttu-id="11aab-454">"Get-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="11aab-454">'Get-AzIotHubDistributedTracing'</span></span>
    - <span data-ttu-id="11aab-455">"Set-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="11aab-455">'Set-AzIotHubDistributedTracing'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="11aab-456">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="11aab-456">Az.KeyVault</span></span>
* <span data-ttu-id="11aab-457">Foram adicionados os atributos da alteração interruptiva a "New-AzKeyVault"</span><span class="sxs-lookup"><span data-stu-id="11aab-457">Added breaking change attributes to 'New-AzKeyVault'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="11aab-458">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="11aab-458">Az.Monitor</span></span>
* <span data-ttu-id="11aab-459">Foi atualizada a documentação de "New-AzScheduledQueryRuleLogMetricTrigger"</span><span class="sxs-lookup"><span data-stu-id="11aab-459">Updated documentation for 'New-AzScheduledQueryRuleLogMetricTrigger'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-460">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-460">Az.Network</span></span>
* <span data-ttu-id="11aab-461">Foram atualizados os cmdlets para permitir VirtualHubVnetConnections entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="11aab-461">Updated cmdlets to allow cross-tenant VirtualHubVnetConnections</span></span>
    - <span data-ttu-id="11aab-462">"New-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="11aab-462">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="11aab-463">"Update-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="11aab-463">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="11aab-464">"New-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="11aab-464">'New-AzVirtualHub'</span></span>
    - <span data-ttu-id="11aab-465">"Update-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="11aab-465">'Update-AzVirtualHub'</span></span>
* <span data-ttu-id="11aab-466">Foi removida a dependência do SDK do SQL Management</span><span class="sxs-lookup"><span data-stu-id="11aab-466">Removed Sql Management SDK dependency</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="11aab-467">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="11aab-467">Az.PolicyInsights</span></span>
* <span data-ttu-id="11aab-468">Mensagens de erro melhoradas</span><span class="sxs-lookup"><span data-stu-id="11aab-468">Improved error messages</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="11aab-469">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="11aab-469">Az.RecoveryServices</span></span>
* <span data-ttu-id="11aab-470">O Azure Site Recovery adicionou suporte para nova proteção e atualização das propriedades de VM para Máquinas Virtuais encriptadas em disco do Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-470">Azure Site Recovery added support for doing reprotect and updated vm properties for Azure disk encrypted Virtual Machines.</span></span>
* <span data-ttu-id="11aab-471">Foi adicionada monitorização DR das propriedades VmwareToAzure ao Azure Site Recovery</span><span class="sxs-lookup"><span data-stu-id="11aab-471">Added Azure Site Recovery VmwareToAzure properties DR monitoring</span></span>
* <span data-ttu-id="11aab-472">O Azure Backup adicionou suporte para repetir a atualização de políticas para itens falhados.</span><span class="sxs-lookup"><span data-stu-id="11aab-472">Azure Backup added support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="11aab-473">O Azure Backup adicionou suporte para definições de exclusão do disco durante a cópia de segurança e o restauro.</span><span class="sxs-lookup"><span data-stu-id="11aab-473">Azure Backup Added support for disk exclusion settings during backup and restore.</span></span>
* <span data-ttu-id="11aab-474">O Azure Backup adicionou suporte para restaurar vários ficheiros/pastas no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="11aab-474">Azure Backup Added Support for Restoring Multiple files/folders in AzureFileShare</span></span>
* <span data-ttu-id="11aab-475">O Azure Backup adicionou suporte para o Resourcegroup especificado pelo utilizador durante a atualização da Política IaasVM</span><span class="sxs-lookup"><span data-stu-id="11aab-475">Azure Backup Added support for User-specified Resourcegroup support while updating IaasVM Policy</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-476">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-476">Az.Resources</span></span>
* <span data-ttu-id="11aab-477">Foi corrigido o parâmetro "Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType" para utilizar a apiVersion real dos recursos em vez da apiVersion predefinida [#11267]</span><span class="sxs-lookup"><span data-stu-id="11aab-477">Fixed 'Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType' to use actual apiVersion of resources instead of default apiVersion [#11267]</span></span>
* <span data-ttu-id="11aab-478">Foi adicionado o registo de correlationId para cenários de erro</span><span class="sxs-lookup"><span data-stu-id="11aab-478">Added correlationId logging for error scenarios</span></span>
* <span data-ttu-id="11aab-479">Pequena alteração à documentação referente a "Get-AzResourceLock".</span><span class="sxs-lookup"><span data-stu-id="11aab-479">Small documentation change to 'Get-AzResourceLock'.</span></span> <span data-ttu-id="11aab-480">Exemplo adicionado.</span><span class="sxs-lookup"><span data-stu-id="11aab-480">Added example.</span></span>
* <span data-ttu-id="11aab-481">Aspas com caráter de escape no valor de parâmetro "Get-AzADUser" [#11317]</span><span class="sxs-lookup"><span data-stu-id="11aab-481">Escaped single quote in parameter value of 'Get-AzADUser' [#11317]</span></span>
* <span data-ttu-id="11aab-482">Foram adicionados novos cmdlets aos Scripts de Implementação ("Get-AzDeploymentScript", "Get-AzDeploymentScriptLog", "Save-AzDeploymentScriptLog", "Remove-AzDeploymentScript")</span><span class="sxs-lookup"><span data-stu-id="11aab-482">Added new cmdlets for Deployment Scripts ('Get-AzDeploymentScript', 'Get-AzDeploymentScriptLog', 'Save-AzDeploymentScriptLog', 'Remove-AzDeploymentScript')</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-483">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-483">Az.Sql</span></span>
* <span data-ttu-id="11aab-484">Foi adicionado um parâmetro secundário legível a "Invoke-AzSqlDatabaseFailover"</span><span class="sxs-lookup"><span data-stu-id="11aab-484">Added readable secondary parameter to 'Invoke-AzSqlDatabaseFailover'</span></span>
* <span data-ttu-id="11aab-485">Foi adicionado o cmdlet "Disable-AzSqlServerActiveDirectoryOnlyAuthentication"</span><span class="sxs-lookup"><span data-stu-id="11aab-485">Added cmdlet 'Disable-AzSqlServerActiveDirectoryOnlyAuthentication'</span></span>
* <span data-ttu-id="11aab-486">Classificação de sensibilidade guardada ao classificar as colunas na base de dados.</span><span class="sxs-lookup"><span data-stu-id="11aab-486">Saved sensitivity rank when classifying columns in the database.</span></span>

#### <a name="azsupport"></a><span data-ttu-id="11aab-487">Az.Support</span><span class="sxs-lookup"><span data-stu-id="11aab-487">Az.Support</span></span>
* <span data-ttu-id="11aab-488">Disponibilidade geral do módulo "Az.Support"</span><span class="sxs-lookup"><span data-stu-id="11aab-488">General availability of 'Az.Support' module</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="11aab-489">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="11aab-489">Az.Websites</span></span>
* <span data-ttu-id="11aab-490">Foi adicionado suporte para utilizar Regras de Encaminhamento de Tráfego webapp através dos novos cmdlets abaixo</span><span class="sxs-lookup"><span data-stu-id="11aab-490">Added support for working with webapp Traffic Routing Rules via below new cmdlets</span></span>
    - <span data-ttu-id="11aab-491">"Get-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="11aab-491">'Get-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="11aab-492">"Update-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="11aab-492">'Update-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="11aab-493">"Add-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="11aab-493">'Add-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="11aab-494">"Remove-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="11aab-494">'Remove-AzWebAppTrafficRouting'</span></span>

## <a name="361---march-2020"></a><span data-ttu-id="11aab-495">3.6.1 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="11aab-495">3.6.1 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="11aab-496">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-496">Az.Accounts</span></span>
* <span data-ttu-id="11aab-497">Abrir a página de inquérito do Azure PowerShell em "Send-Feedback" [#11020]</span><span class="sxs-lookup"><span data-stu-id="11aab-497">Open Azure PowerShell survey page in 'Send-Feedback' [#11020]</span></span>
* <span data-ttu-id="11aab-498">Apresentar o URL de inquérito do Azure PowerShell em "Resolve-Error" [#11021]</span><span class="sxs-lookup"><span data-stu-id="11aab-498">Display Azure PowerShell survey URL in 'Resolve-Error' [#11021]</span></span>
* <span data-ttu-id="11aab-499">Adicionada versão de Az em UserAgent</span><span class="sxs-lookup"><span data-stu-id="11aab-499">Added Az version in UserAgent</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="11aab-500">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="11aab-500">Az.ApiManagement</span></span>
* <span data-ttu-id="11aab-501">Adicionado suporte para a obtenção e configuração do Domínio Personalizado no Ponto Final do DeveloperPortal [#11007]</span><span class="sxs-lookup"><span data-stu-id="11aab-501">Added support for retrieving and configuring Custom Domain on the DeveloperPortal Endpoint [#11007]</span></span>
* <span data-ttu-id="11aab-502">"Export-AzApiManagementApi" Adicionado suporte para a transferência da definição da API no formato JSON [#9987]</span><span class="sxs-lookup"><span data-stu-id="11aab-502">'Export-AzApiManagementApi' Added support for downloading Api Definition in Json format [#9987]</span></span>
* <span data-ttu-id="11aab-503">"Import-AzApiManagementApi" Adicionado suporte para a importação da definição de OpenApi 3.0 a partir de documento JSON</span><span class="sxs-lookup"><span data-stu-id="11aab-503">'Import-AzApiManagementApi' Added support for importing OpenApi 3.0 definition from Json document</span></span>
* <span data-ttu-id="11aab-504">"New-AzApiManagementIdentityProvider" e "Set-AzApiManagementIdentityProvider" Adicionado suporte para a configuração de "Inquilino de Início de Sessão" para Fornecedor de AAD B2C [#9784]</span><span class="sxs-lookup"><span data-stu-id="11aab-504">'New-AzApiManagementIdentityProvider' and 'Set-AzApiManagementIdentityProvider' Added support for configuring 'Signin Tenant' for AAD B2C Provider [#9784]</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="11aab-505">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="11aab-505">Az.DataLakeStore</span></span>
* <span data-ttu-id="11aab-506">Adicionada referência a System.Buffers explicitamente em csproj e psd1.</span><span class="sxs-lookup"><span data-stu-id="11aab-506">Added reference to System.Buffers explicitly in csproj and psd1.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="11aab-507">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="11aab-507">Az.IotHub</span></span>
* <span data-ttu-id="11aab-508">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="11aab-508">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="11aab-509">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="11aab-509">New Cmdlets are:</span></span>
    - <span data-ttu-id="11aab-510">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="11aab-510">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="11aab-511">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="11aab-511">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="11aab-512">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="11aab-512">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="11aab-513">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="11aab-513">'Set-AzIotHubDevice'</span></span>
* <span data-ttu-id="11aab-514">Adicionado suporte para a gestão de módulos num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="11aab-514">Added support to manage modules on a target Iot device in an Iot Hub.</span></span> <span data-ttu-id="11aab-515">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="11aab-515">New Cmdlets are:</span></span>
    - <span data-ttu-id="11aab-516">"Add-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="11aab-516">'Add-AzIotHubModule'</span></span>
    - <span data-ttu-id="11aab-517">"Get-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="11aab-517">'Get-AzIotHubModule'</span></span>
    - <span data-ttu-id="11aab-518">"Remove-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="11aab-518">'Remove-AzIotHubModule'</span></span>
    - <span data-ttu-id="11aab-519">"Set-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="11aab-519">'Set-AzIotHubModule'</span></span>
* <span data-ttu-id="11aab-520">Adicionado cmdlet para obter a cadeia de ligação de um dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="11aab-520">Added cmdlet to get the connection string of a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="11aab-521">Adicionado cmdlet para obter a cadeia de ligação de um módulo num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="11aab-521">Added cmdlet to get the connection string of a module on a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="11aab-522">Adicionado suporte para obter/definir dispositivo principal de um dispositivo IoT.</span><span class="sxs-lookup"><span data-stu-id="11aab-522">Added support to get/set parent device of an IoT device.</span></span> <span data-ttu-id="11aab-523">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="11aab-523">New Cmdlets are:</span></span>
    - <span data-ttu-id="11aab-524">"Get-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="11aab-524">'Get-AzIotHubDeviceParent'</span></span>
    - <span data-ttu-id="11aab-525">"Set-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="11aab-525">'Set-AzIotHubDeviceParent'</span></span>
* <span data-ttu-id="11aab-526">Adicionado suporte para gerir relações principal-subordinado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="11aab-526">Added support to manage device parent-child relationship.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="11aab-527">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="11aab-527">Az.Monitor</span></span>
* <span data-ttu-id="11aab-528">Corrigido o valor de saída de "Get-AzMetricDefinition" [#9714]</span><span class="sxs-lookup"><span data-stu-id="11aab-528">Fixed output value for 'Get-AzMetricDefinition' [#9714]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-529">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-529">Az.Network</span></span>
* <span data-ttu-id="11aab-530">Sdk Sql Management atualizado.</span><span class="sxs-lookup"><span data-stu-id="11aab-530">Updated Sql Management SDK.</span></span>
* <span data-ttu-id="11aab-531">Corrigido um problema de diferença de nomes na classe PrivateLinkServiceConnectionState.</span><span class="sxs-lookup"><span data-stu-id="11aab-531">Fixed a naming-difference issue in PrivateLinkServiceConnectionState class.</span></span>
    - <span data-ttu-id="11aab-532">Mapeamento do campo ActionsRequired para ActionRequired.</span><span class="sxs-lookup"><span data-stu-id="11aab-532">Mapping the field ActionsRequired to ActionRequired.</span></span>
* <span data-ttu-id="11aab-533">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="11aab-533">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-534">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-534">Az.Resources</span></span>
* <span data-ttu-id="11aab-535">Correção para erro de referência nula em "Get-AzRoleAssignment"</span><span class="sxs-lookup"><span data-stu-id="11aab-535">Fixed for null reference bug in 'Get-AzRoleAssignment'</span></span>
* <span data-ttu-id="11aab-536">Comutadores "-Force" e "-PassThru" marcados como opcionais em "Remove-AzADGroup" [#10849]</span><span class="sxs-lookup"><span data-stu-id="11aab-536">Marked switch '-Force' and '-PassThru' optional in 'Remove-AzADGroup' [#10849]</span></span>
* <span data-ttu-id="11aab-537">Corrigido problema em que "MailNickname" não devolve "Remove-AzADGroup" [#11167]</span><span class="sxs-lookup"><span data-stu-id="11aab-537">Fixed issue that 'MailNickname' doesn't return in 'Remove-AzADGroup' [#11167]</span></span>
* <span data-ttu-id="11aab-538">Corrigido problema em que a operação de pipe "Remove-AzADGroup" não funciona [#11171]</span><span class="sxs-lookup"><span data-stu-id="11aab-538">Fixed issue that 'Remove-AzADGroup' pipe operation doesn't work [#11171]</span></span>
* <span data-ttu-id="11aab-539">Correção para erro de referência nula em GetAzureRoleAssignmentCommand</span><span class="sxs-lookup"><span data-stu-id="11aab-539">Fixed for null reference bug in GetAzureRoleAssignmentCommand</span></span>
* <span data-ttu-id="11aab-540">Adicionados atributos de alterações interruptivas para futuras alterações a cmdlets de política</span><span class="sxs-lookup"><span data-stu-id="11aab-540">Added breaking change attributes for upcoming changes to policy cmdlets</span></span>
* <span data-ttu-id="11aab-541">"Get-AzResourceGroup" atualizado para realizar filtragem de etiqueta de grupo de recursos no lado do servidor</span><span class="sxs-lookup"><span data-stu-id="11aab-541">Updated 'Get-AzResourceGroup' to perform resource group tag filtering on server-side</span></span>
* <span data-ttu-id="11aab-542">Cmdlets Tag alargados para accept -ResourceId</span><span class="sxs-lookup"><span data-stu-id="11aab-542">Extended Tag cmdlets to accept -ResourceId</span></span>
    - <span data-ttu-id="11aab-543">Get-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="11aab-543">Get-AzTag -ResourceId</span></span>
    - <span data-ttu-id="11aab-544">New-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="11aab-544">New-AzTag -ResourceId</span></span>
    - <span data-ttu-id="11aab-545">Remove-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="11aab-545">Remove-AzTag -ResourceId</span></span>
* <span data-ttu-id="11aab-546">Adicionado cmdlet Tag novo</span><span class="sxs-lookup"><span data-stu-id="11aab-546">Added new Tag cmdlet</span></span>
    - <span data-ttu-id="11aab-547">Update-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="11aab-547">Update-AzTag -ResourceId</span></span>
* <span data-ttu-id="11aab-548">ScopedDeployment trazido de SDK 3.3.0</span><span class="sxs-lookup"><span data-stu-id="11aab-548">Brought ScopedDeployment from SDK 3.3.0</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-549">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-549">Az.Sql</span></span>
* <span data-ttu-id="11aab-550">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="11aab-550">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="11aab-551">Adicionado suporte para configuração de cópia de segurança de Retenção de Longo Prazo para Bases de Dados Geridas</span><span class="sxs-lookup"><span data-stu-id="11aab-551">Added support for Long Term Retention backup configuration for Managed Databases</span></span>
    - <span data-ttu-id="11aab-552">Política Get/Set numa base de dados gerida</span><span class="sxs-lookup"><span data-stu-id="11aab-552">Get/Set LTR policy on a managed database</span></span>
    - <span data-ttu-id="11aab-553">Obter cópia(s) de segurança LTR por base de dados gerida, por instância gerida ou por localização</span><span class="sxs-lookup"><span data-stu-id="11aab-553">Get LTR backup(s) by managed database, managed instance, or by location</span></span>
    - <span data-ttu-id="11aab-554">Remover uma cópia de segurança LTR</span><span class="sxs-lookup"><span data-stu-id="11aab-554">Remove an LTR backup</span></span>
    - <span data-ttu-id="11aab-555">Restaurar uma cópia de segurança LTR para criar uma base de dados gerida nova</span><span class="sxs-lookup"><span data-stu-id="11aab-555">Restore an LTR backup to create a new managed database</span></span>
* <span data-ttu-id="11aab-556">Adicionado MinimalTlsVersion a New-AzSqlServer e Set-AzSqlServer</span><span class="sxs-lookup"><span data-stu-id="11aab-556">Added MinimalTlsVersion to New-AzSqlServer and Set-AzSqlServer</span></span>
* <span data-ttu-id="11aab-557">Adicionado MinimalTlsVersion a New-AzSqlInstance e Set-AzSqlInstance</span><span class="sxs-lookup"><span data-stu-id="11aab-557">Added MinimalTlsVersion to New-AzSqlInstance and Set-AzSqlInstance</span></span>
* <span data-ttu-id="11aab-558">Versão de SDK SQL atualizada para Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-558">Bumped SQL SDK version for Az.Network</span></span>

#### <a name="azstorage"></a><span data-ttu-id="11aab-559">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-559">Az.Storage</span></span>
* <span data-ttu-id="11aab-560">AllowProtectedAppendWrite suportada em ImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="11aab-560">Supported AllowProtectedAppendWrite in ImmutabilityPolicy</span></span>
    - <span data-ttu-id="11aab-561">"Set-AzRmStorageContainerImmutabilityPolicy"</span><span class="sxs-lookup"><span data-stu-id="11aab-561">'Set-AzRmStorageContainerImmutabilityPolicy'</span></span>
* <span data-ttu-id="11aab-562">Adicionada uma mensagem de aviso de alteração interruptiva para alteração do tipo AzureStorageTable numa futura versão</span><span class="sxs-lookup"><span data-stu-id="11aab-562">Added breaking change warning message for AzureStorageTable type change in a future release</span></span>
    - <span data-ttu-id="11aab-563">"New-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="11aab-563">'New-AzStorageTable'</span></span>
    - <span data-ttu-id="11aab-564">"Get-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="11aab-564">'Get-AzStorageTable'</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="11aab-565">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="11aab-565">Az.Websites</span></span>
* <span data-ttu-id="11aab-566">Adicionado o parâmetro Tag para "New-AzAppServicePlan" e "Set-AzAppServicePlan"</span><span class="sxs-lookup"><span data-stu-id="11aab-566">Added Tag parameter for 'New-AzAppServicePlan' and 'Set-AzAppServicePlan'</span></span>
* <span data-ttu-id="11aab-567">Paragem da execução de cmdlet caso seja emitida uma exceção ao adicionar um domínio personalizado a um site</span><span class="sxs-lookup"><span data-stu-id="11aab-567">Stop cmdlet execution if an exception is thrown when adding a custom domain to a website</span></span>
* <span data-ttu-id="11aab-568">Adicionado suporte para a realização de operações para Serviços de Aplicações em grupos de recursos diferentes do Plano do Serviço de Aplicações</span><span class="sxs-lookup"><span data-stu-id="11aab-568">Added support to perform operations for App Services not in the same resource group as the App Service Plan</span></span>
* <span data-ttu-id="11aab-569">Aplicada restrição de acesso a WebApp/Função em diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="11aab-569">Applied access restriction to WebApp/Function in different resource groups</span></span>
* <span data-ttu-id="11aab-570">Corrigido problema para definir os nomes de anfitrião personalizados para WebAppSlots</span><span class="sxs-lookup"><span data-stu-id="11aab-570">Fixed issue to set custom hostnames for WebAppSlots</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="11aab-571">3.5.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="11aab-571">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="11aab-572">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="11aab-572">Highlights since the last major release</span></span>
* <span data-ttu-id="11aab-573">Telemetria do lado do cliente atualizada.</span><span class="sxs-lookup"><span data-stu-id="11aab-573">Updated client side telemetry.</span></span>
* <span data-ttu-id="11aab-574">O Az.IotHub adicionou cmdlets para suportar a gestão de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="11aab-574">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="11aab-575">O Az.SqlVirtualMachine adicionou cmdlets ao Serviço de Escuta do Grupo de Disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="11aab-575">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="11aab-576">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-576">Az.Accounts</span></span>
* <span data-ttu-id="11aab-577">SubscriptionId, TenantId e tempo de execução adicionados aos dados de telemetria do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="11aab-577">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="11aab-578">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="11aab-578">Az.Automation</span></span>
* <span data-ttu-id="11aab-579">Foi corrigido o erro no Exemplo 1 na documentação de referência de "New-AzAutomationSoftwareUpdateConfiguration"</span><span class="sxs-lookup"><span data-stu-id="11aab-579">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="11aab-580">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="11aab-580">Az.CognitiveServices</span></span>
* <span data-ttu-id="11aab-581">SDK atualizado para a versão 7.0</span><span class="sxs-lookup"><span data-stu-id="11aab-581">Updated SDK to 7.0</span></span>
* <span data-ttu-id="11aab-582">Mensagem de erro melhorada quando o servidor responde ao corpo vazio</span><span class="sxs-lookup"><span data-stu-id="11aab-582">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-583">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-583">Az.Compute</span></span>
* <span data-ttu-id="11aab-584">Valor vazio permitido para ProximityPlacementGroupId durante a atualização</span><span class="sxs-lookup"><span data-stu-id="11aab-584">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="11aab-585">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="11aab-585">Az.FrontDoor</span></span>
* <span data-ttu-id="11aab-586">Cmdlet adicionado para obter definições de regras geridas que podem ser utilizadas na WAF</span><span class="sxs-lookup"><span data-stu-id="11aab-586">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="11aab-587">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="11aab-587">Az.IotHub</span></span>
* <span data-ttu-id="11aab-588">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="11aab-588">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="11aab-589">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="11aab-589">New Cmdlets are:</span></span>
    - <span data-ttu-id="11aab-590">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="11aab-590">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="11aab-591">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="11aab-591">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="11aab-592">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="11aab-592">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="11aab-593">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="11aab-593">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="11aab-594">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="11aab-594">Az.KeyVault</span></span>
* <span data-ttu-id="11aab-595">Texto duplicado fixo para Add-AzKeyVaultKey.md</span><span class="sxs-lookup"><span data-stu-id="11aab-595">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="11aab-596">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="11aab-596">Az.Monitor</span></span>
* <span data-ttu-id="11aab-597">Descrição fixa do cmdlet Get-AzLog.</span><span class="sxs-lookup"><span data-stu-id="11aab-597">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="11aab-598">Foi adicionado um novo parâmetro chamado ActionGroupId ao comando "New-AzMetricAlertRuleV2".</span><span class="sxs-lookup"><span data-stu-id="11aab-598">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="11aab-599">O utilizador pode fornecer ActionGroupId(string) ou ActionGorup(ActivityLogAlertActionGroup).</span><span class="sxs-lookup"><span data-stu-id="11aab-599">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-600">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-600">Az.Network</span></span>
* <span data-ttu-id="11aab-601">Foi adicionada uma nota de parâmetro adicional para o parâmetro "-EnableProxyProtocol" para o cmdlet "New-AzPrivateLinkService".</span><span class="sxs-lookup"><span data-stu-id="11aab-601">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="11aab-602">Exemplo de FilterData fixo em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="11aab-602">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="11aab-603">Exemplo de Captura de Pacotes adicionado para capturar todos os pacotes internos e externos em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="11aab-603">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="11aab-604">Política do Azure Firewall suportada em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="11aab-604">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="11aab-605">Não foram adicionados novos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="11aab-605">No new cmdlets are added.</span></span> <span data-ttu-id="11aab-606">Simplificação da restrição da política de firewall em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="11aab-606">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="11aab-607">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="11aab-607">Az.RecoveryServices</span></span>
* <span data-ttu-id="11aab-608">Suporte adicionado da funcionalidade Restaurar como ficheiros para Bases de Dados SQL.</span><span class="sxs-lookup"><span data-stu-id="11aab-608">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-609">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-609">Az.Resources</span></span>
* <span data-ttu-id="11aab-610">Cmdlets de implementação de modelos refatorizados</span><span class="sxs-lookup"><span data-stu-id="11aab-610">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="11aab-611">Foram adicionados novos cmdlets para gerir implementações no grupo de gestão: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="11aab-611">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="11aab-612">Foram adicionados novos cmdlets para gerir implementações no inquilino: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="11aab-612">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="11aab-613">Cmdlets \*-AzDeployment refatorizados para trabalhar especificamente no âmbito da subscrição</span><span class="sxs-lookup"><span data-stu-id="11aab-613">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="11aab-614">Foram criados aliases \*-AzSubscriptionDeployment para os cmdlets \*-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="11aab-614">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="11aab-615">"Update-AzADApplication" fixo quando o parâmetro "AvailableToOtherTenants" não está definido</span><span class="sxs-lookup"><span data-stu-id="11aab-615">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="11aab-616">ApplicationObjectWithoutCredentialParameterSet removido para evitar AmbiguousParameterSetException.</span><span class="sxs-lookup"><span data-stu-id="11aab-616">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="11aab-617">Ficheiros de ajuda regenerados</span><span class="sxs-lookup"><span data-stu-id="11aab-617">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-618">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-618">Az.Sql</span></span>
* <span data-ttu-id="11aab-619">Suporte adicionado para restauro para um ponto anterior no tempo entre subscrições nas Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="11aab-619">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="11aab-620">Suporte adicionado para alterar a geração de hardware das Instâncias Geridas de SQL existentes</span><span class="sxs-lookup"><span data-stu-id="11aab-620">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="11aab-621">Exemplos de ajuda "Update-AzSqlServerVulnerabilityAssessmentSetting" fixos: saída do parâmetro/propriedade - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="11aab-621">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="11aab-622">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="11aab-622">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="11aab-623">Cmdlets adicionados para o Serviço de Escuta do Grupo de Disponibilidade</span><span class="sxs-lookup"><span data-stu-id="11aab-623">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="11aab-624">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="11aab-624">Az.StorageSync</span></span>
* <span data-ttu-id="11aab-625">Conjuntos de carateres suportados atualizados em "Invoke-AzStorageSyncCompatibilityCheck".</span><span class="sxs-lookup"><span data-stu-id="11aab-625">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="11aab-626">3.4.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="11aab-626">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="11aab-627">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="11aab-627">Highlights since the last major release</span></span>
* <span data-ttu-id="11aab-628">Versão inicial Az.CosmosDB 0.1.0 lançada</span><span class="sxs-lookup"><span data-stu-id="11aab-628">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="11aab-629">Foi adicionado suporte para Az.Network ConnectionMonitor V2</span><span class="sxs-lookup"><span data-stu-id="11aab-629">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="11aab-630">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-630">Az.Accounts</span></span>
* <span data-ttu-id="11aab-631">Foi desativada a gravação automática de contexto quando AzureRmContext.json não está disponível</span><span class="sxs-lookup"><span data-stu-id="11aab-631">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="11aab-632">Atualização da referência ao Azure Powershell Common para a pré-visualização 1.3.5</span><span class="sxs-lookup"><span data-stu-id="11aab-632">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="11aab-633">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="11aab-633">Az.ApiManagement</span></span>
* <span data-ttu-id="11aab-634">**Get-AzApiManagementApiSchema** Foi corrigido ao obter Open-Api Schema associado a uma API   https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="11aab-634">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="11aab-635">**New-AzApiManagementProduct**\* e **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="11aab-635">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="11aab-636">Foi corrigida a documentação para https://github.com/Azure/azure-powershell/issues/10472</span><span class="sxs-lookup"><span data-stu-id="11aab-636">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="11aab-637">**Set-AzApiManagementApi** Exemplo adicionado para mostrar como atualizar o ServiceUrl com o cmdlet</span><span class="sxs-lookup"><span data-stu-id="11aab-637">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-638">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-638">Az.Compute</span></span>
* <span data-ttu-id="11aab-639">Foi limitado o número de estados de VM a 100 para evitar limitações quando Get-AzVM-Status é executado sem o nome da VM.</span><span class="sxs-lookup"><span data-stu-id="11aab-639">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="11aab-640">Foi adicionado o cmdlet Update-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="11aab-640">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="11aab-641">Foram adicionados os parâmetros EncryptionType e DiskEncryptionSetId aos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="11aab-641">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="11aab-642">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-642">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="11aab-643">Foi adicionado o parâmetro ColocationStatus ao cmdlet Get-AzProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="11aab-643">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="11aab-644">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="11aab-644">Az.DataFactory</span></span>
* <span data-ttu-id="11aab-645">Atualização do SDK .NET do ADF para a versão 4.7.0</span><span class="sxs-lookup"><span data-stu-id="11aab-645">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="11aab-646">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="11aab-646">Az.DeploymentManager</span></span>
* <span data-ttu-id="11aab-647">Adiciona operações LIST para os recursos</span><span class="sxs-lookup"><span data-stu-id="11aab-647">Adds LIST operations for resources</span></span>
* <span data-ttu-id="11aab-648">Adiciona a capacidade de realizar operações nos passos de Verificação de Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="11aab-648">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="11aab-649">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="11aab-649">Az.HDInsight</span></span>
* <span data-ttu-id="11aab-650">Foi corrigido o erro do documento de New-AzHDInsightCluster.</span><span class="sxs-lookup"><span data-stu-id="11aab-650">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="11aab-651">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="11aab-651">Az.KeyVault</span></span>
* <span data-ttu-id="11aab-652">Foi adicionado o alias do Nome ao atributo VaultName para tornar Remove-AzureKeyVault consistente com New-AzureKeyVault.</span><span class="sxs-lookup"><span data-stu-id="11aab-652">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-653">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-653">Az.Network</span></span>
* <span data-ttu-id="11aab-654">Foi adicionado um novo exemplo a Set-AzNetworkWatcherConfigFlowLog.md para demonstrar o cenário de desativação da Análise de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="11aab-654">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="11aab-655">Foi adicionado suporte para atribuir a configuração IP de gestão ao Azure Firewall, uma sub-rede dedicada e IP Público que a firewall utilizará no tráfego de gestão</span><span class="sxs-lookup"><span data-stu-id="11aab-655">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="11aab-656">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="11aab-656">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="11aab-657">Foi adicionado o parâmetro -ManagementPublicIpAddress (não obrigatório) que aceita um objeto de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="11aab-657">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="11aab-658">Foi adicionado o método SetManagementIpConfiguration no objeto de firewall. Requer uma sub-rede e um endereço IP Público como entrada. O nome da sub-rede tem de ser "AzureFirewallManagementSubnet"</span><span class="sxs-lookup"><span data-stu-id="11aab-658">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="11aab-659">Foram corrigidos os exemplos de Get-AzNetworkSecurityGroup para mostrar exemplos de NSGs em vez de interfaces de rede.</span><span class="sxs-lookup"><span data-stu-id="11aab-659">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="11aab-660">Foi corrigido um erro no comando New-AzVpnSite que estava a impedir o ID do recurso de concluir um parâmetro.</span><span class="sxs-lookup"><span data-stu-id="11aab-660">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="11aab-661">Foi adicionado suporte para a Configuração do URL em Reescrever Conjunto de Ações de Regras no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="11aab-661">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="11aab-662">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="11aab-662">New cmdlets added:</span></span>
        - <span data-ttu-id="11aab-663">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="11aab-663">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="11aab-664">Foram atualizados cmdlets com o parâmetro opcional - UrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="11aab-664">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="11aab-665">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="11aab-665">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="11aab-666">Foi adicionado suporte para os recursos do NetworkWatcher ConnectionMonitor versão 2</span><span class="sxs-lookup"><span data-stu-id="11aab-666">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="11aab-667">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="11aab-667">Az.PolicyInsights</span></span>
* <span data-ttu-id="11aab-668">Foi adicionado suporte para avaliar a conformidade antes de determinar o recurso a remediar</span><span class="sxs-lookup"><span data-stu-id="11aab-668">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="11aab-669">Foi adicionado o parâmetro "-ResourceDiscoverMode" a Start-AzPolicyRemediation</span><span class="sxs-lookup"><span data-stu-id="11aab-669">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="11aab-670">Foi adicionado o cmdlet Get-AzPolicyMetadata para obter os recursos de metadados da política</span><span class="sxs-lookup"><span data-stu-id="11aab-670">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="11aab-671">Get-AzPolicyState e Get-AzPolicyStateSummary atualizados para a versão da API 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="11aab-671">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="11aab-672">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="11aab-672">Az.RecoveryServices</span></span>
* <span data-ttu-id="11aab-673">Foi adicionado suporte do Azure Site Recovery para remover um disco replicado.</span><span class="sxs-lookup"><span data-stu-id="11aab-673">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="11aab-674">O Azure Backup adicionou suporte para adicionar etiquetas ao criar um Cofre dos Serviços de Recuperação.</span><span class="sxs-lookup"><span data-stu-id="11aab-674">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-675">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-675">Az.Resources</span></span>
* <span data-ttu-id="11aab-676">-Scope foi tornado opcional nos cmdlets \*-AzPolicyAssignment com subscrição de contexto predefinida</span><span class="sxs-lookup"><span data-stu-id="11aab-676">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="11aab-677">Foram adicionados exemplos de criação de ADServicePrincipal com credenciais de palavras-passe e chaves</span><span class="sxs-lookup"><span data-stu-id="11aab-677">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-678">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-678">Az.Sql</span></span>
<span data-ttu-id="11aab-679">Foi corrigido o cmdlet New-AzSqlDatabaseSecondary para verificar a existência de PartnerDatabaseName em vez da existência de DatabaseName.</span><span class="sxs-lookup"><span data-stu-id="11aab-679">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="11aab-680">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-680">Az.Storage</span></span>
* <span data-ttu-id="11aab-681">Foi definido o suporte de Tipo de Chave de Encriptação na Tabela/Fila em Criar Conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="11aab-681">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="11aab-682">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="11aab-682">New-AzStorageAccount</span></span>
* <span data-ttu-id="11aab-683">Será apresentado RequestId quando StorageException não tiver ExtendedErrorInformation</span><span class="sxs-lookup"><span data-stu-id="11aab-683">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="11aab-684">Foi corrigido o exemplo 6 do cmdlet Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="11aab-684">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="11aab-685">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="11aab-685">Az.Websites</span></span>
* <span data-ttu-id="11aab-686">Set-AzWebapp e Set-AzWebappSlot suportam as propriedades AlwaysOn, MinTls e FtpsState</span><span class="sxs-lookup"><span data-stu-id="11aab-686">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="11aab-687">Foi corrigido o problema em que a definição de HttpsOnly, juntamente com a alteração de AppservicePlan ao utilizar o único comando Set-AzWebApp, estava a repor HttpsOnly para o valor predefinido</span><span class="sxs-lookup"><span data-stu-id="11aab-687">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="11aab-688">3.3.0 – janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="11aab-688">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="11aab-689">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-689">Az.Accounts</span></span>
* <span data-ttu-id="11aab-690">Add-AzEnvironment e Set-AzEnvironment foram atualizados para aceitar os parâmetros AzureAttestationServiceEndpointResourceId e AzureAttestationServiceEndpointSuffix</span><span class="sxs-lookup"><span data-stu-id="11aab-690">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="11aab-691">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="11aab-691">Az.Cdn</span></span>
* <span data-ttu-id="11aab-692">Apresentação dos detalhes da resposta de erro no cmdlet New-AzCdnEndpoint</span><span class="sxs-lookup"><span data-stu-id="11aab-692">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-693">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-693">Az.Compute</span></span>
* <span data-ttu-id="11aab-694">Correção do cmdlet Set-AzVMCustomScriptExtension para uma VM com disco OD gerido sem perfil de SO.</span><span class="sxs-lookup"><span data-stu-id="11aab-694">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="11aab-695">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="11aab-695">Az.ContainerInstance</span></span>
* <span data-ttu-id="11aab-696">Foram corrigidos os nomes de parâmetros utilizados pelo exemplo de New-AzContainerGroup</span><span class="sxs-lookup"><span data-stu-id="11aab-696">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="11aab-697">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="11aab-697">Az.DataBoxEdge</span></span>
* <span data-ttu-id="11aab-698">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="11aab-698">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="11aab-699">Obter o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="11aab-699">Get the Edge Storage Container</span></span>
* <span data-ttu-id="11aab-700">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="11aab-700">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="11aab-701">Criar novo Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="11aab-701">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="11aab-702">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="11aab-702">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="11aab-703">Remover o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="11aab-703">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="11aab-704">Foi adicionado o cmdlet "Invoke-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="11aab-704">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="11aab-705">Invocar ação para atualizar os dados no Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="11aab-705">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="11aab-706">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="11aab-706">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="11aab-707">Obter a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="11aab-707">Get the Edge Storage Account</span></span>
* <span data-ttu-id="11aab-708">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="11aab-708">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="11aab-709">Criar nova Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="11aab-709">Create new Edge Storage Account</span></span>
* <span data-ttu-id="11aab-710">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="11aab-710">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="11aab-711">Remover a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="11aab-711">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="11aab-712">Invocar o cmdlet "Invoke-AzDataBoxEdgeShare"</span><span class="sxs-lookup"><span data-stu-id="11aab-712">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="11aab-713">Invocar ação para atualizar os dados na partilha</span><span class="sxs-lookup"><span data-stu-id="11aab-713">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="11aab-714">Foi adicionado o cmdlet "Set-AzDataBoxEdgeStorageAccountCredential"</span><span class="sxs-lookup"><span data-stu-id="11aab-714">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="11aab-715">Definição de AzDataBoxEdgeStorageAccountCredential</span><span class="sxs-lookup"><span data-stu-id="11aab-715">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="11aab-716">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="11aab-716">Az.DataFactory</span></span>
* <span data-ttu-id="11aab-717">Adição das propriedades AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId e VersionStatus para o cmd Get-AzDataFactoryV2IntegrationRuntime</span><span class="sxs-lookup"><span data-stu-id="11aab-717">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="11aab-718">Atualização do SDK .NET do ADF para a versão 4.6.0</span><span class="sxs-lookup"><span data-stu-id="11aab-718">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="11aab-719">Adição do parâmetro "PublicIPs" para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a criação de Azure-SSIS IR com endereços IP públicos estáticos.</span><span class="sxs-lookup"><span data-stu-id="11aab-719">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="11aab-720">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="11aab-720">Az.DevTestLabs</span></span>
* <span data-ttu-id="11aab-721">Remoção da ligação quebrada em Get-AzDtlAllowedVMSizesPolicy.md</span><span class="sxs-lookup"><span data-stu-id="11aab-721">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="11aab-722">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="11aab-722">Az.EventHub</span></span>
* <span data-ttu-id="11aab-723">Correção do problema 10634: Correção da referência de objeto nulo para remover eventhubnamespace</span><span class="sxs-lookup"><span data-stu-id="11aab-723">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="11aab-724">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="11aab-724">Az.HDInsight</span></span>
* <span data-ttu-id="11aab-725">Correção do erro Invoke-AzHDInsightHiveJob.md.</span><span class="sxs-lookup"><span data-stu-id="11aab-725">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="11aab-726">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="11aab-726">Az.MachineLearning</span></span>
* <span data-ttu-id="11aab-727">Foram removidos os cmdlets abaixo porque MachineLearningCompute já não está disponível</span><span class="sxs-lookup"><span data-stu-id="11aab-727">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="11aab-728">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="11aab-728">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="11aab-729">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="11aab-729">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="11aab-730">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="11aab-730">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="11aab-731">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="11aab-731">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="11aab-732">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="11aab-732">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="11aab-733">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="11aab-733">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="11aab-734">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="11aab-734">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-735">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-735">Az.Network</span></span>
* <span data-ttu-id="11aab-736">Atualização da dependência de Microsoft.Azure.Management.SQL da versão 1.36-preview para 1.37-preview</span><span class="sxs-lookup"><span data-stu-id="11aab-736">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="11aab-737">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="11aab-737">Az.RecoveryServices</span></span>
* <span data-ttu-id="11aab-738">Alteração do Azure Site Recovery para suportar VMs de disco gerido com encriptação inativa com chaves geridas pelo cliente para o fornecedor do Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-738">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="11aab-739">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-739">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="11aab-740">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional ao nível do disco para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-740">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="11aab-741">Suporte do Azure Site Recovery para atualizar o item protegido por replicação com encriptação de discos e definir o mapa para HyperV para o Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-741">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-742">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-742">Az.Resources</span></span>
* <span data-ttu-id="11aab-743">Correção de um erro no documento de ajuda de "Remove-AzTag".</span><span class="sxs-lookup"><span data-stu-id="11aab-743">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-744">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-744">Az.Sql</span></span>
* <span data-ttu-id="11aab-745">Correção da funcionalidade dos cmdlets de linha de base do conjunto de avaliação de vulnerabilidades para funcionar na base de dados mestre da base de dados do Azure e limitá-la nas bases de dados do sistema de instância gerida</span><span class="sxs-lookup"><span data-stu-id="11aab-745">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="11aab-746">Correção de um erro ao criar o grupo de ativação pós-falha de instância SQL</span><span class="sxs-lookup"><span data-stu-id="11aab-746">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="11aab-747">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="11aab-747">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="11aab-748">Adição de DR como um novo tipo de Licença válido</span><span class="sxs-lookup"><span data-stu-id="11aab-748">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="11aab-749">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-749">Az.Storage</span></span>
* <span data-ttu-id="11aab-750">Adição de uma mensagem de aviso de alteração interruptiva para alteração do valor de DefaultAction numa futura versão</span><span class="sxs-lookup"><span data-stu-id="11aab-750">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="11aab-751">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="11aab-751">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="11aab-752">Suporte para obter a hora da última sincronização da conta de armazenamento ao executar get-AzureRMStorageAccount com o parâmetro -IncludeGeoReplicationStats</span><span class="sxs-lookup"><span data-stu-id="11aab-752">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span>
    - <span data-ttu-id="11aab-753">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="11aab-753">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="11aab-754">3.2.0 - Dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-754">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="11aab-755">Geral</span><span class="sxs-lookup"><span data-stu-id="11aab-755">General</span></span>
* <span data-ttu-id="11aab-756">Atualização das referências em .psd1 para utilizar o caminho relativo para todos os módulos</span><span class="sxs-lookup"><span data-stu-id="11aab-756">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="11aab-757">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-757">Az.Accounts</span></span>
* <span data-ttu-id="11aab-758">Definição do UserAgent correto para telemetria do lado do cliente para a pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="11aab-758">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="11aab-759">Apresentação de mensagem de erro amigável de utilizador quando o contexto é nulo na pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="11aab-759">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="11aab-760">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="11aab-760">Az.Batch</span></span>
* <span data-ttu-id="11aab-761">Correção do problema [10602](https://github.com/Azure/azure-powershell/issues/10602), em que **New-AzBatchPool** não enviava corretamente "VirtualMachineConfiguration.ContainerConfiguration" ou "VirtualMachineConfiguration.DataDisks" para o servidor.</span><span class="sxs-lookup"><span data-stu-id="11aab-761">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="11aab-762">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="11aab-762">Az.DataFactory</span></span>
* <span data-ttu-id="11aab-763">Atualização do SDK .NET do ADF para a versão 4.5.0</span><span class="sxs-lookup"><span data-stu-id="11aab-763">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="11aab-764">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="11aab-764">Az.FrontDoor</span></span>
* <span data-ttu-id="11aab-765">Adição do suporte de exclusão de regras geridas pela WAF</span><span class="sxs-lookup"><span data-stu-id="11aab-765">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="11aab-766">Adição de SocketAddr ao preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="11aab-766">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="11aab-767">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="11aab-767">Az.HealthcareApis</span></span>
* <span data-ttu-id="11aab-768">Processamento de Exceções</span><span class="sxs-lookup"><span data-stu-id="11aab-768">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="11aab-769">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="11aab-769">Az.KeyVault</span></span>
* <span data-ttu-id="11aab-770">Correção do erro em que era acedido um valor potencialmente não definido</span><span class="sxs-lookup"><span data-stu-id="11aab-770">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="11aab-771">Gestão de Certificados de Criptografia de Curva Elíptica</span><span class="sxs-lookup"><span data-stu-id="11aab-771">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="11aab-772">Adicionado suporte para especificar a Curva das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="11aab-772">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="11aab-773">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="11aab-773">Az.Monitor</span></span>
* <span data-ttu-id="11aab-774">Adição de um argumento opcional ao comando Adicionar Definições de Diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="11aab-774">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="11aab-775">Um argumento de opção que, se estiver presente, indica que a exportação para o Log Analytics deve ser feita para um esquema fixo (também conhecido como</span><span class="sxs-lookup"><span data-stu-id="11aab-775">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="11aab-776">tipo de dados dedicado)</span><span class="sxs-lookup"><span data-stu-id="11aab-776">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-777">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-777">Az.Network</span></span>
* <span data-ttu-id="11aab-778">Suporte para IpGroups na aplicação AzureFirewall, Nat e Regras de Rede.</span><span class="sxs-lookup"><span data-stu-id="11aab-778">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-779">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-779">Az.Resources</span></span>
* <span data-ttu-id="11aab-780">Correção de um problema em que a implementação do modelo não consegue ler um parâmetro se o nome estiver em conflito com um nome de parâmetro incorporado.</span><span class="sxs-lookup"><span data-stu-id="11aab-780">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="11aab-781">Os cmdlets da política foram atualizados para utilizar a nova versão de API 2019-09-01 que introduz suporte de agrupamento nas definições do conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="11aab-781">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-782">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-782">Az.Sql</span></span>
* <span data-ttu-id="11aab-783">Criação do armazenamento atualizada na ativação automática da Avaliação de Vulnerabilidades para StorageV2</span><span class="sxs-lookup"><span data-stu-id="11aab-783">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="11aab-784">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-784">Az.Storage</span></span>
* <span data-ttu-id="11aab-785">Suporte para gerar um token de SAS baseado na Identidade do Blob/Contentor com Contexto de Armazenamento baseado na autenticação OAuth</span><span class="sxs-lookup"><span data-stu-id="11aab-785">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="11aab-786">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="11aab-786">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="11aab-787">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="11aab-787">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="11aab-788">Suporte para revogar as Chaves de Delegação do Utilizador da Conta de Armazenamento, pelo que todos os tokens de SAS da identidade são revogados</span><span class="sxs-lookup"><span data-stu-id="11aab-788">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="11aab-789">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="11aab-789">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="11aab-790">Atualização de Microsoft.Azure.Management.Storage 14.2.0 para suportar a nova versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="11aab-790">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="11aab-791">Suporte de QuotaGiB (Quota de Partilha em Gibibye) para obter valores superiores a 5120 no plano de Gestão de cmdlets de Partilha de Ficheiros e foi adicionado o alias do parâmetro "Quota" ao parâmetro "QuotaGiB".</span><span class="sxs-lookup"><span data-stu-id="11aab-791">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span>
    - <span data-ttu-id="11aab-792">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="11aab-792">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="11aab-793">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="11aab-793">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="11aab-794">Adição do alias do parâmetro "QuotaGiB" ao parâmetro "Quota"</span><span class="sxs-lookup"><span data-stu-id="11aab-794">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="11aab-795">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="11aab-795">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="11aab-796">Correção do problema em que Set-AzStorageContainerAcl consegue limpar a Política de Acesso armazenada</span><span class="sxs-lookup"><span data-stu-id="11aab-796">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="11aab-797">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="11aab-797">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="11aab-798">3.1.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-798">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="11aab-799">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="11aab-799">Highlights since the last major release</span></span>
* <span data-ttu-id="11aab-800">Az.DataBoxEdge 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="11aab-800">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="11aab-801">Az.SqlVirtualMachine 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="11aab-801">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-802">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-802">Az.Compute</span></span>
* <span data-ttu-id="11aab-803">Funcionalidade de Reaplicação da VM</span><span class="sxs-lookup"><span data-stu-id="11aab-803">VM Reapply feature</span></span>
    - <span data-ttu-id="11aab-804">Adição do parâmetro Reapply ao cmdlet Set-AzVM</span><span class="sxs-lookup"><span data-stu-id="11aab-804">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="11aab-805">Funcionalidade AutomaticRepairs do Conjunto de Dimensionamento de VM:</span><span class="sxs-lookup"><span data-stu-id="11aab-805">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="11aab-806">Adição dos parâmetros EnableAutomaticRepair, AutomaticRepairGracePeriod e AutomaticRepairMaxInstanceRepairsPercent aos seguintes cmdlets:   New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="11aab-806">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="11aab-807">Suporte para imagens de galeria entre inquilinos para New-AzVM</span><span class="sxs-lookup"><span data-stu-id="11aab-807">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="11aab-808">Adição de "Spot" ao preenchedor de argumentos do parâmetro Priority nos cmdlets New-AzVM, New-AzVMConfig e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="11aab-808">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="11aab-809">Adição dos parâmetros DiskIOPSReadWrite e DiskMBpsReadWrite ao cmdlet Add-AzVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="11aab-809">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="11aab-810">Alteração do parâmetro SourceImageId do cmdlet New-AzGalleryImageVersion para opcional</span><span class="sxs-lookup"><span data-stu-id="11aab-810">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="11aab-811">Adição dos parâmetros OSDiskImage e DataDiskImage ao cmdlet New-AzGalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="11aab-811">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="11aab-812">Adição do parâmetro HyperVGeneration ao cmdlet New-AzGalleryImageDefinition</span><span class="sxs-lookup"><span data-stu-id="11aab-812">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="11aab-813">Adição dos parâmetros SkipExtensionsOnOverprovisionedVMs aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="11aab-813">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="11aab-814">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="11aab-814">Az.DataBoxEdge</span></span>
* <span data-ttu-id="11aab-815">Adição do cmdlet `Get-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="11aab-815">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="11aab-816">Obter a Encomenda</span><span class="sxs-lookup"><span data-stu-id="11aab-816">Get the Order</span></span>
* <span data-ttu-id="11aab-817">Adição do cmdlet `New-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="11aab-817">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="11aab-818">Criar nova Encomenda</span><span class="sxs-lookup"><span data-stu-id="11aab-818">Create new Order</span></span>
* <span data-ttu-id="11aab-819">Adição do cmdlet `Remove-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="11aab-819">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="11aab-820">Remover a Encomenda</span><span class="sxs-lookup"><span data-stu-id="11aab-820">Remove the Order</span></span>
* <span data-ttu-id="11aab-821">Alteração no cmdlet `New-AzDataBoxEdgeShare`</span><span class="sxs-lookup"><span data-stu-id="11aab-821">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="11aab-822">Agora cria uma Partilha Local</span><span class="sxs-lookup"><span data-stu-id="11aab-822">Now creates Local Share</span></span>
* <span data-ttu-id="11aab-823">Adição do cmdlet `Set-AzDataBoxEdgeRole`</span><span class="sxs-lookup"><span data-stu-id="11aab-823">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="11aab-824">Agora, o IotRole pode ser mapeado para a Partilha</span><span class="sxs-lookup"><span data-stu-id="11aab-824">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="11aab-825">Adição do cmdlet `Invoke-AzDataBoxEdgeDevice`</span><span class="sxs-lookup"><span data-stu-id="11aab-825">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="11aab-826">Invocar verificação da atualização, transferência da atualização, instalação das atualizações no dispositivo</span><span class="sxs-lookup"><span data-stu-id="11aab-826">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="11aab-827">Adição do cmdlet `Get-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="11aab-827">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="11aab-828">Obtém as informações sobre os Acionadores</span><span class="sxs-lookup"><span data-stu-id="11aab-828">Gets the information about Triggers</span></span>
* <span data-ttu-id="11aab-829">Adição do cmdlet `New-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="11aab-829">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="11aab-830">Criar novos Acionadores</span><span class="sxs-lookup"><span data-stu-id="11aab-830">Create new Triggers</span></span>
* <span data-ttu-id="11aab-831">Adição do cmdlet `Remove-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="11aab-831">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="11aab-832">Remover os Acionadores</span><span class="sxs-lookup"><span data-stu-id="11aab-832">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="11aab-833">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="11aab-833">Az.DataFactory</span></span>
* <span data-ttu-id="11aab-834">Atualização do SDK .NET do ADF para a versão 4.4.0</span><span class="sxs-lookup"><span data-stu-id="11aab-834">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="11aab-835">Adição do parâmetro "ExpressCustomSetup" para o cmdlet "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir configurações e componentes de terceiros sem scripts de configuração personalizados.</span><span class="sxs-lookup"><span data-stu-id="11aab-835">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="11aab-836">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="11aab-836">Az.DataLakeStore</span></span>
* <span data-ttu-id="11aab-837">Atualização da documentação de Get-AzDataLakeStoreDeletedItem e Restore-AzDataLakeStoreDeletedItem</span><span class="sxs-lookup"><span data-stu-id="11aab-837">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="11aab-838">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="11aab-838">Az.EventHub</span></span>
* <span data-ttu-id="11aab-839">Correção do problema 10301: Correção do formato de data do token de SAS</span><span class="sxs-lookup"><span data-stu-id="11aab-839">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="11aab-840">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="11aab-840">Az.FrontDoor</span></span>
* <span data-ttu-id="11aab-841">Adição do parâmetro MinimumTlsVersion a Enable-AzFrontDoorCustomDomainHttps e New-AzFrontDoorFrontendEndpointObject</span><span class="sxs-lookup"><span data-stu-id="11aab-841">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="11aab-842">Adição dos parâmetros HealthProbeMethod e EnabledState a New-AzFrontDoorHealthProbeSettingObject</span><span class="sxs-lookup"><span data-stu-id="11aab-842">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="11aab-843">Adição de um novo cmdlet para criar um objeto BackendPoolsSettings para passar para a criação/atualização do Front Door</span><span class="sxs-lookup"><span data-stu-id="11aab-843">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="11aab-844">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="11aab-844">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-845">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-845">Az.Network</span></span>
* <span data-ttu-id="11aab-846">Alteração dos exemplos de opções FilterData de "Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" e "Start-AzVirtualnetworkGatewayPacketCapture.md".</span><span class="sxs-lookup"><span data-stu-id="11aab-846">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="11aab-847">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="11aab-847">Az.PrivateDns</span></span>
* <span data-ttu-id="11aab-848">Atualização do SDK .NET do PrivateDns para a versão 1.0.0</span><span class="sxs-lookup"><span data-stu-id="11aab-848">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="11aab-849">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="11aab-849">Az.RecoveryServices</span></span>
* <span data-ttu-id="11aab-850">Suporte do Azure Site Recovery para selecionar o tipo de disco ao ativar a proteção.</span><span class="sxs-lookup"><span data-stu-id="11aab-850">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="11aab-851">Correção do Azure Site Recovery para a edição de ações do plano de recuperação.</span><span class="sxs-lookup"><span data-stu-id="11aab-851">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="11aab-852">Suporte de Restauro de SQL do Azure Backup para aceitar BDs de filestream.</span><span class="sxs-lookup"><span data-stu-id="11aab-852">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="11aab-853">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="11aab-853">Az.RedisCache</span></span>
* <span data-ttu-id="11aab-854">Adição do parâmetro "MinimumTlsVersion" nos cmdlets "New-AzRedisCache" e "Set-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="11aab-854">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="11aab-855">Adição, também, de "MinimumTlsVersion" na saída do cmdlet "Get-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="11aab-855">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="11aab-856">Adição da validação no parâmetro "-Size" para os cmdlets "Set-AzRedisCache" e "New-AzRedisCache"</span><span class="sxs-lookup"><span data-stu-id="11aab-856">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-857">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-857">Az.Resources</span></span>
- <span data-ttu-id="11aab-858">Atualização dos cmdlets de política no sentido de utilizar a nova versão de api 2019-06-01, a qual tem a nova propriedade EnforcementMode na atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="11aab-858">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="11aab-859">Atualização do exemplo de ajuda da definição da política de criação</span><span class="sxs-lookup"><span data-stu-id="11aab-859">Updated create policy definition help example</span></span>
- <span data-ttu-id="11aab-860">Correção do erro Remove-AZADServicePrincipal -ServicePrincipalName. Apresentação de uma referência nula quando o nome do principal do serviço não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="11aab-860">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="11aab-861">Correção do erro New-AZADServicePrincipal. Apresentação de uma referência nula quando o inquilino não tem uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="11aab-861">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="11aab-862">Alteração de New-AzAdServicePrincipal para adicionar credenciais apenas a aplicações associadas.</span><span class="sxs-lookup"><span data-stu-id="11aab-862">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-863">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-863">Az.Sql</span></span>
* <span data-ttu-id="11aab-864">Adição de suporte para a base de dados ReadReplicaCount.</span><span class="sxs-lookup"><span data-stu-id="11aab-864">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="11aab-865">Correção de Set-AzSqlDatabase quando a redundância de zona não está definida</span><span class="sxs-lookup"><span data-stu-id="11aab-865">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="11aab-866">3.0.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-866">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="11aab-867">Geral</span><span class="sxs-lookup"><span data-stu-id="11aab-867">General</span></span>
* <span data-ttu-id="11aab-868">Disponibilização do Az.PrivateDns 1.0.0</span><span class="sxs-lookup"><span data-stu-id="11aab-868">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="11aab-869">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-869">Az.Accounts</span></span>
* <span data-ttu-id="11aab-870">Adição de uma mensagem de descontinuação para o alias "Resolve-Error".</span><span class="sxs-lookup"><span data-stu-id="11aab-870">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="11aab-871">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="11aab-871">Az.Advisor</span></span>
* <span data-ttu-id="11aab-872">Adição da nova categoria "Excelência Operacional" ao cmdlet Get-AzAdvisorRecommendation.</span><span class="sxs-lookup"><span data-stu-id="11aab-872">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="11aab-873">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="11aab-873">Az.Batch</span></span>
* <span data-ttu-id="11aab-874">Mudança de nome de `CoreQuota` em `BatchAccountContext` para `DedicatedCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="11aab-874">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="11aab-875">Existe também um novo `LowPriorityCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="11aab-875">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="11aab-876">Isto afeta **Get-AzBatchAccount**.</span><span class="sxs-lookup"><span data-stu-id="11aab-876">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="11aab-877">O parâmetro **New-AzBatchTask** `-ResourceFile` assume agora uma coleção de objetos `PSResourceFile`, os quais podem ser construídos com o novo cmdlet **New-AzBatchResourceFile**.</span><span class="sxs-lookup"><span data-stu-id="11aab-877">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="11aab-878">Novo cmdlet **New-AzBatchResourceFile** para ajudar a criar objetos `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="11aab-878">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="11aab-879">Estes podem ser fornecidos a **New-AzBatchTask** no parâmetro `-ResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="11aab-879">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="11aab-880">Isto suporta dois novos tipos de ficheiro de recursos para além do caminho `HttpUrl` existente:</span><span class="sxs-lookup"><span data-stu-id="11aab-880">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="11aab-881">Os ficheiros de recursos baseados em `AutoStorageContainerName` transferem um contentor integral de armazenamento automático para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="11aab-881">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="11aab-882">Os ficheiros de recursos baseados em `StorageContainerUrl` transferem o contentor especificado no URL para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="11aab-882">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="11aab-883">Remoção da propriedade `ApplicationPackages` de `PSApplication` devolvida por **Get-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="11aab-883">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="11aab-884">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com **Get-AzBatchApplicationPackage**.</span><span class="sxs-lookup"><span data-stu-id="11aab-884">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="11aab-885">Por exemplo: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span><span class="sxs-lookup"><span data-stu-id="11aab-885">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="11aab-886">Mudança de nome de `ApplicationId` para `ApplicationName` em **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication** e **Set-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="11aab-886">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="11aab-887">`ApplicationId` é agora um alias de `ApplicationName`.</span><span class="sxs-lookup"><span data-stu-id="11aab-887">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="11aab-888">Adição da nova propriedade `PSWindowsUserConfiguration` a `PSUserAccount`.</span><span class="sxs-lookup"><span data-stu-id="11aab-888">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="11aab-889">Mudança de nome de `Version` para `Name` em `PSApplicationPackage`.</span><span class="sxs-lookup"><span data-stu-id="11aab-889">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="11aab-890">Mudança de nome de `BlobSource` para `HttpUrl` em `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="11aab-890">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="11aab-891">Remoção da propriedade `OSDisk` de `PSVirtualMachineConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="11aab-891">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="11aab-892">Remoção de **Set-AzBatchPoolOSVersion**.</span><span class="sxs-lookup"><span data-stu-id="11aab-892">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="11aab-893">Esta operação deixou de ser suportada.</span><span class="sxs-lookup"><span data-stu-id="11aab-893">This operation is no longer supported.</span></span>
* <span data-ttu-id="11aab-894">Remoção de `TargetOSVersion` de `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="11aab-894">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="11aab-895">Mudança de nome de `CurrentOSVersion` para `OSVersion` em `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="11aab-895">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="11aab-896">Remoção de `DataEgressGiB` e `DataIngressGiB` de `PSPoolUsageMetrics`.</span><span class="sxs-lookup"><span data-stu-id="11aab-896">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="11aab-897">Remoção de **Get-AzBatchNodeAgentSku** e substituição deste por **Get-AzBatchSupportedImage**.</span><span class="sxs-lookup"><span data-stu-id="11aab-897">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span>
  - <span data-ttu-id="11aab-898">**Get-AzBatchSupportedImage** devolve os mesmos dados de **Get-AzBatchNodeAgentSku**, mas num formato mais acessível.</span><span class="sxs-lookup"><span data-stu-id="11aab-898">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="11aab-899">As novas imagens não verificadas agora também são devolvidas.</span><span class="sxs-lookup"><span data-stu-id="11aab-899">New non-verified images are also now returned.</span></span> <span data-ttu-id="11aab-900">Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.</span><span class="sxs-lookup"><span data-stu-id="11aab-900">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="11aab-901">Adição da capacidade de montagem de sistemas de ficheiros remotos em cada nó de um conjunto através do novo parâmetro `MountConfiguration` de **New-AzBatchPool**.</span><span class="sxs-lookup"><span data-stu-id="11aab-901">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="11aab-902">Adição do suporte a regras de segurança de rede que bloqueiam o acesso de rede a um conjunto com base na porta de origem do tráfego.</span><span class="sxs-lookup"><span data-stu-id="11aab-902">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="11aab-903">Isto ocorre através da propriedade `SourcePortRanges` em `PSNetworkSecurityGroupRule`.</span><span class="sxs-lookup"><span data-stu-id="11aab-903">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="11aab-904">Ao executar um contentor, o Batch agora suporta a execução da tarefa no diretório de trabalho do contentor ou no diretório de trabalho da tarefa do Batch.</span><span class="sxs-lookup"><span data-stu-id="11aab-904">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="11aab-905">Isto é controlado pela propriedade `WorkingDirectory` em `PSTaskContainerSettings`.</span><span class="sxs-lookup"><span data-stu-id="11aab-905">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="11aab-906">Adição da capacidade de especificar uma coleção de IPs públicos em `PSNetworkConfiguration` através da nova propriedade `PublicIPs`.</span><span class="sxs-lookup"><span data-stu-id="11aab-906">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="11aab-907">Isto garante que os nós no Conjunto terão um IP da lista de IPs fornecidos pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="11aab-907">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="11aab-908">Quando não for especificado, o valor predefinido de `WaitForSuccess` em `PSSTartTask` é agora `$True` (era `$False`).</span><span class="sxs-lookup"><span data-stu-id="11aab-908">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="11aab-909">Quando não for especificado, o valor predefinido de `Scope` em `PSAutoUserSpecification` é agora `Pool` (era `Task` no Windows e `Pool` no Linux).</span><span class="sxs-lookup"><span data-stu-id="11aab-909">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="11aab-910">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="11aab-910">Az.Cdn</span></span>
* <span data-ttu-id="11aab-911">Introdução de UrlRewriteAction e CacheKeyQueryStringAction em RulesEngine.</span><span class="sxs-lookup"><span data-stu-id="11aab-911">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="11aab-912">Correção de vários erros como a falta da Entrada "Seletor" no cmdlet New-AzDeliveryRuleCondition.</span><span class="sxs-lookup"><span data-stu-id="11aab-912">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-913">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-913">Az.Compute</span></span>
* <span data-ttu-id="11aab-914">Funcionalidade Conjunto de Encriptação de Discos</span><span class="sxs-lookup"><span data-stu-id="11aab-914">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="11aab-915">Novos cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="11aab-915">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="11aab-916">Adição do parâmetro DiskEncryptionSetId aos seguintes cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="11aab-916">DiskEncryptionSetId parameter is added to the following cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="11aab-917">Adição dos parâmetros DiskEncryptionSetId e EncryptionType aos seguintes cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-917">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="11aab-918">Adição do parâmetro PublicIPAddressVersion a New-AzVmssIPConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-918">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="11aab-919">Movimentação de FileUris da extensão de script personalizado da definição pública para a definição protegida</span><span class="sxs-lookup"><span data-stu-id="11aab-919">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="11aab-920">Adição de ScaleInPolicy aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="11aab-920">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="11aab-921">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="11aab-921">Breaking changes</span></span>
    - <span data-ttu-id="11aab-922">Utilização do parâmetro UploadSizeInBytes em vez de DiskSizeGB para New-AzDiskConfig quando CreateOption é Carregar</span><span class="sxs-lookup"><span data-stu-id="11aab-922">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="11aab-923">Substituição de PublishingProfile.Source.ManagedImage.Id por StorageProfile.Source.Id no objeto GalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="11aab-923">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="11aab-924">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="11aab-924">Az.DataFactory</span></span>
* <span data-ttu-id="11aab-925">Atualização da versão do SDK .Net do ADF para 4.3.0</span><span class="sxs-lookup"><span data-stu-id="11aab-925">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="11aab-926">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="11aab-926">Az.DataLakeStore</span></span>
* <span data-ttu-id="11aab-927">Atualização da versão do SDK ADLS (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) ) com as seguintes correções</span><span class="sxs-lookup"><span data-stu-id="11aab-927">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="11aab-928">Evita a apresentação de uma exceção ao mesmo tempo que não consegue anular a serialização do creationtime do lixo ou da entrada de diretório.</span><span class="sxs-lookup"><span data-stu-id="11aab-928">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="11aab-929">Expõe a definição por tempo limite do pedido em adlsclient</span><span class="sxs-lookup"><span data-stu-id="11aab-929">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="11aab-930">Correção da passagem do syncflag original para a recuperação de badoffset</span><span class="sxs-lookup"><span data-stu-id="11aab-930">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="11aab-931">Correção de EnumerateDirectory para obter o token de continuação após a verificação da resposta</span><span class="sxs-lookup"><span data-stu-id="11aab-931">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="11aab-932">Correção do Erro de Concatenação</span><span class="sxs-lookup"><span data-stu-id="11aab-932">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="11aab-933">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="11aab-933">Az.FrontDoor</span></span>
* <span data-ttu-id="11aab-934">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="11aab-934">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="11aab-935">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="11aab-935">Az.HDInsight</span></span>
* <span data-ttu-id="11aab-936">Correção do erro em que o cliente recebe o erro "Não é uma cadeia Base 64 válida" quando utiliza Get-AzHDInsightCluster para obter o cluster com o armazenamento ADLSGen1.</span><span class="sxs-lookup"><span data-stu-id="11aab-936">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="11aab-937">Adição de um parâmetro com o nome "ApplicationId" a três cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig e New-AzHDInsightCluster para que o cliente consiga fornecer o ID da aplicação do principal de serviço que permite aceder ao Azure Data Lake.</span><span class="sxs-lookup"><span data-stu-id="11aab-937">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="11aab-938">Alteração de Microsoft.Azure.Management.HDInsight da versão 2.1.0 para a 5.1.0</span><span class="sxs-lookup"><span data-stu-id="11aab-938">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="11aab-939">Remoção de cinco cmdlets:</span><span class="sxs-lookup"><span data-stu-id="11aab-939">Removed five cmdlets:</span></span>
    - <span data-ttu-id="11aab-940">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="11aab-940">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="11aab-941">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="11aab-941">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="11aab-942">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="11aab-942">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="11aab-943">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="11aab-943">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="11aab-944">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="11aab-944">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="11aab-945">Adição de três cmdlets:</span><span class="sxs-lookup"><span data-stu-id="11aab-945">Added three cmdlets:</span></span>
    - <span data-ttu-id="11aab-946">Get-AzHDInsightMonitoring para substituir Get-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="11aab-946">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="11aab-947">Enable-AzHDInsightMonitoring para substituir Enable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="11aab-947">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="11aab-948">Disable-AzHDInsightMonitoring para substituir Disable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="11aab-948">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="11aab-949">Correção do cmdlet Get-AzHDInsightProperties para suportar a obtenção de informações sobre capacidades de uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="11aab-949">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="11aab-950">Remoção de conjuntos de parâmetros("Spark1", "Spark2") de Add-AzHDInsightConfigValue.</span><span class="sxs-lookup"><span data-stu-id="11aab-950">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="11aab-951">Adição de exemplos aos documentos de ajuda do cmdlet Add-AzHDInsightSecurityProfile.</span><span class="sxs-lookup"><span data-stu-id="11aab-951">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="11aab-952">Alteração do tipo de saída dos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="11aab-952">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="11aab-953">Alteração do tipo de saída de Get-AzHDInsightProperties de CapabilitiesResponse para AzureHDInsightCapabilities.</span><span class="sxs-lookup"><span data-stu-id="11aab-953">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="11aab-954">Alteração do tipo de saída de Remove-AzHDInsightCluster de ClusterGetResponse para booleano.</span><span class="sxs-lookup"><span data-stu-id="11aab-954">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="11aab-955">Alteração do tipo de saída de Set-AzHDInsightGatewaySettings de HttpConnectivitySettings para GatewaySettings.</span><span class="sxs-lookup"><span data-stu-id="11aab-955">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="11aab-956">Adição de alguns casos de teste de cenários.</span><span class="sxs-lookup"><span data-stu-id="11aab-956">Added some scenario test cases.</span></span>
* <span data-ttu-id="11aab-957">Remoção de alguns alias: "Add-AzHDInsightConfigValues", "Get-AzHDInsightProperties".</span><span class="sxs-lookup"><span data-stu-id="11aab-957">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="11aab-958">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="11aab-958">Az.IotHub</span></span>
* <span data-ttu-id="11aab-959">Alterações interruptivas:</span><span class="sxs-lookup"><span data-stu-id="11aab-959">Breaking changes:</span></span>
    - <span data-ttu-id="11aab-960">O cmdlet "Add-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="11aab-960">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="11aab-961">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Add-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="11aab-961">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="11aab-962">O cmdlet "Get-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="11aab-962">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="11aab-963">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Get-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="11aab-963">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="11aab-964">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="11aab-964">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="11aab-965">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="11aab-965">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="11aab-966">O cmdlet "New-AzIotHubExportDevice" deixou de suportar o alias "New-AzIotHubExportDevices".</span><span class="sxs-lookup"><span data-stu-id="11aab-966">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="11aab-967">O cmdlet "New-AzIotHubImportDevice" deixou de suportar o alias "New-AzIotHubImportDevices".</span><span class="sxs-lookup"><span data-stu-id="11aab-967">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="11aab-968">O cmdlet "Remove-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="11aab-968">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="11aab-969">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Remove-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="11aab-969">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="11aab-970">O cmdlet "Set-AzIotHub" deixou de suportar o parâmetro "OperationsMonitoringProperties" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="11aab-970">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="11aab-971">O conjunto de parâmetros "UpdateOperationsMonitoringProperties" do cmdlet "Set-AzIotHub" foi removido.</span><span class="sxs-lookup"><span data-stu-id="11aab-971">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="11aab-972">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="11aab-972">Az.RecoveryServices</span></span>
* <span data-ttu-id="11aab-973">Suporte do Azure Site Recovery para configurar recursos de rede como NSG, IP público e balanceadores de carga internos do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-973">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="11aab-974">Suporte do Azure Site Recovery para escrever para um disco gerido do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-974">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="11aab-975">Suporte do Azure Site Recovery para redução de NIC do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-975">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="11aab-976">Suporte do Azure Site Recovery para aceleração de rede do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-976">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="11aab-977">Suporte do Azure Site Recovery para a atualização automática do agente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-977">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="11aab-978">Suporte do Azure Site Recovery para SSD Standard do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-978">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="11aab-979">Suporte do Azure Site Recovery para a codificação em dois passos do Azure Disk Encryption do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-979">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="11aab-980">Suporte do Azure Site Recovery para a proteção de um disco adicionado recentemente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-980">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="11aab-981">Adição da funcionalidade SoftDelete para VM e de testes para softdelete</span><span class="sxs-lookup"><span data-stu-id="11aab-981">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-982">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-982">Az.Resources</span></span>
* <span data-ttu-id="11aab-983">Atualização da assemblagem de dependências Microsoft.Extensions.Caching.Memory da versão 1.1.1 para a 2.2</span><span class="sxs-lookup"><span data-stu-id="11aab-983">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-984">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-984">Az.Network</span></span>
* <span data-ttu-id="11aab-985">Alteração de todos os cmdlets para PrivateEndpointConnection para suportar o fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="11aab-985">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="11aab-986">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="11aab-986">Updated cmdlet:</span></span>
        - <span data-ttu-id="11aab-987">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-987">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="11aab-988">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-988">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="11aab-989">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-989">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="11aab-990">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-990">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="11aab-991">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-991">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="11aab-992">Adição de novo cmdlet para PrivateLinkResource também com suporte de fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="11aab-992">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="11aab-993">Novo cmdlet:</span><span class="sxs-lookup"><span data-stu-id="11aab-993">New cmdlet:</span></span>
        - <span data-ttu-id="11aab-994">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="11aab-994">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="11aab-995">Adição de novos campos e parâmetro para a funcionalidade Protocolo de Proxy V2.</span><span class="sxs-lookup"><span data-stu-id="11aab-995">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="11aab-996">Adição da propriedade EnableProxyProtocol em PrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="11aab-996">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="11aab-997">Adição da propriedade LinkIdentifier em PrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-997">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="11aab-998">Atualização de New-AzPrivateLinkService para adicionar um novo parâmetro adicional EnableProxyProtocol.</span><span class="sxs-lookup"><span data-stu-id="11aab-998">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="11aab-999">Correção da descrição incorreta do parâmetro na documentação de referência "New-AzApplicationGatewaySku"</span><span class="sxs-lookup"><span data-stu-id="11aab-999">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="11aab-1000">Novos cmdlets para suportar a política de firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="11aab-1000">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="11aab-1001">Adição de suporte para o recurso subordinado RouteTables de VirtualHub</span><span class="sxs-lookup"><span data-stu-id="11aab-1001">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="11aab-1002">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="11aab-1002">New cmdlets added:</span></span>
        - <span data-ttu-id="11aab-1003">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="11aab-1003">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="11aab-1004">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="11aab-1004">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="11aab-1005">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="11aab-1005">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="11aab-1006">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="11aab-1006">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="11aab-1007">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="11aab-1007">Set-AzVirtualHub</span></span>
* <span data-ttu-id="11aab-1008">Adição de suporte para o SKU de novas propriedades de VirtualHub e VirtualWANType de VirtualWan</span><span class="sxs-lookup"><span data-stu-id="11aab-1008">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="11aab-1009">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="11aab-1009">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="11aab-1010">New-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="11aab-1010">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="11aab-1011">Update-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="11aab-1011">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="11aab-1012">New-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="11aab-1012">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="11aab-1013">Update-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="11aab-1013">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="11aab-1014">Adição de suporte para a propriedade EnableInternetSecurity para HubVnetConnection, VpnConnection e ExpressRouteConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-1014">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="11aab-1015">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="11aab-1015">New cmdlets added:</span></span>
        - <span data-ttu-id="11aab-1016">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-1016">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="11aab-1017">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="11aab-1017">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="11aab-1018">New-AzureRmVirtualHubVnetConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="11aab-1018">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="11aab-1019">New-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="11aab-1019">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="11aab-1020">Update-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="11aab-1020">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="11aab-1021">New-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="11aab-1021">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="11aab-1022">Set-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="11aab-1022">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="11aab-1023">Adição de suporte para Configurar a Política WebApplicationFirewall de Nível Superior</span><span class="sxs-lookup"><span data-stu-id="11aab-1023">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="11aab-1024">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="11aab-1024">New cmdlets added:</span></span>
        - <span data-ttu-id="11aab-1025">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="11aab-1025">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="11aab-1026">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="11aab-1026">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="11aab-1027">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="11aab-1027">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="11aab-1028">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="11aab-1028">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="11aab-1029">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="11aab-1029">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="11aab-1030">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="11aab-1030">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="11aab-1031">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="11aab-1031">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="11aab-1032">New-AzApplicationGatewayFirewallPolicy : adição do parâmetro PolicySetting, ManagedRule</span><span class="sxs-lookup"><span data-stu-id="11aab-1032">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="11aab-1033">Adição de suporte para o operador GeoMatch em CustomRule</span><span class="sxs-lookup"><span data-stu-id="11aab-1033">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="11aab-1034">Adição de GeoMatch ao operador em FirewallCondition</span><span class="sxs-lookup"><span data-stu-id="11aab-1034">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="11aab-1035">Adição de suporte para a Política de firewall perListener e perSite</span><span class="sxs-lookup"><span data-stu-id="11aab-1035">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="11aab-1036">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="11aab-1036">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="11aab-1037">New-AzApplicationGatewayHttpListener : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="11aab-1037">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="11aab-1038">New-AzApplicationGatewayPathRuleConfig : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="11aab-1038">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="11aab-1039">Correção da sub-rede necessária com o nome AzureBastionSubnet em "PSBastion" pode não ser sensível às maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="11aab-1039">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="11aab-1040">Suporte para FQDNs de Destino nas Regras de Rede e para FQDN Traduzido em Regras NAT para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="11aab-1040">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="11aab-1041">Adição de suporte para o recurso de nível superior RouteTables de IpGroup</span><span class="sxs-lookup"><span data-stu-id="11aab-1041">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="11aab-1042">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="11aab-1042">New cmdlets added:</span></span>
        - <span data-ttu-id="11aab-1043">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="11aab-1043">New-AzIpGroup</span></span>
        - <span data-ttu-id="11aab-1044">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="11aab-1044">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="11aab-1045">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="11aab-1045">Get-AzIpGroup</span></span>
        - <span data-ttu-id="11aab-1046">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="11aab-1046">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="11aab-1047">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="11aab-1047">Az.ServiceFabric</span></span>
* <span data-ttu-id="11aab-1048">Remoção do cmdlet Add-AzServiceFabricApplicationCertificate uma vez que este cenário é abrangido por Add-AzVmssSecret.</span><span class="sxs-lookup"><span data-stu-id="11aab-1048">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-1049">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-1049">Az.Sql</span></span>
* <span data-ttu-id="11aab-1050">Adição de suporte para o restauro de bases de dados removidas em Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="11aab-1050">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="11aab-1051">Descontinuação dos cmdlets de auditoria antigos do código.</span><span class="sxs-lookup"><span data-stu-id="11aab-1051">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="11aab-1052">Remoção de aliases descontinuados:</span><span class="sxs-lookup"><span data-stu-id="11aab-1052">Removed deprecated aliases:</span></span>
* <span data-ttu-id="11aab-1053">Get-AzSqlDatabaseIndexRecommendations (utilize antes Get-AzSqlDatabaseIndexRecommendation)</span><span class="sxs-lookup"><span data-stu-id="11aab-1053">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="11aab-1054">Get-AzSqlDatabaseRestorePoints (utilize antes Get-AzSqlDatabaseRestorePoint)</span><span class="sxs-lookup"><span data-stu-id="11aab-1054">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="11aab-1055">Remoção do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="11aab-1055">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="11aab-1056">Remoção dos aliases dos cmdlets descontinuados das Definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="11aab-1056">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="11aab-1057">Descontinuação dos cmdlets das Definições de Deteção Avançada de Ameaças</span><span class="sxs-lookup"><span data-stu-id="11aab-1057">Deprecate Advanced Threat Detection Settings cmdlets</span></span>
* <span data-ttu-id="11aab-1058">Adição de cmdlets para Desativar e Ativar as recomendações de sensibilidade nas colunas de uma base de dados.</span><span class="sxs-lookup"><span data-stu-id="11aab-1058">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="11aab-1059">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-1059">Az.Storage</span></span>
* <span data-ttu-id="11aab-1060">Suporte à ativação da partilha de Ficheiros de Grandes Dimensões ao criar ou atualizar uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="11aab-1060">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="11aab-1061">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="11aab-1061">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="11aab-1062">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="11aab-1062">Set-AzStorageAccount</span></span>
* <span data-ttu-id="11aab-1063">Ao fechar/obter o Identificador de ficheiro, ignorar a verificação do caminho de entrada corresponde a Diretório de ficheiros ou Ficheiro, de forma a evitar a falha com o objeto no estado DeletePending</span><span class="sxs-lookup"><span data-stu-id="11aab-1063">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="11aab-1064">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="11aab-1064">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="11aab-1065">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="11aab-1065">Close-AzStorageFileHandle</span></span>

## <a name="280---october-2019"></a><span data-ttu-id="11aab-1066">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-1066">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="11aab-1067">Geral</span><span class="sxs-lookup"><span data-stu-id="11aab-1067">General</span></span>
* <span data-ttu-id="11aab-1068">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="11aab-1068">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="11aab-1069">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-1069">Az.Accounts</span></span>
* <span data-ttu-id="11aab-1070">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="11aab-1070">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="11aab-1071">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="11aab-1071">Az.ApiManagement</span></span>
* <span data-ttu-id="11aab-1072">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="11aab-1072">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="11aab-1073">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="11aab-1073">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="11aab-1074">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="11aab-1074">Az.Automation</span></span>
* <span data-ttu-id="11aab-1075">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="11aab-1075">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="11aab-1076">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="11aab-1076">Az.Batch</span></span>
* <span data-ttu-id="11aab-1077">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="11aab-1077">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-1078">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-1078">Az.Compute</span></span>
* <span data-ttu-id="11aab-1079">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="11aab-1079">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="11aab-1080">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="11aab-1080">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="11aab-1081">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="11aab-1081">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span>
* <span data-ttu-id="11aab-1082">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="11aab-1082">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="11aab-1083">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="11aab-1083">Az.DataFactory</span></span>
* <span data-ttu-id="11aab-1084">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="11aab-1084">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="11aab-1085">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="11aab-1085">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="11aab-1086">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="11aab-1086">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="11aab-1087">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="11aab-1087">Az.DataLakeStore</span></span>
* <span data-ttu-id="11aab-1088">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="11aab-1088">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="11aab-1089">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="11aab-1089">Az.HealthcareApis</span></span>
* <span data-ttu-id="11aab-1090">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="11aab-1090">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="11aab-1091">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="11aab-1091">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="11aab-1092">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="11aab-1092">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="11aab-1093">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="11aab-1093">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="11aab-1094">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="11aab-1094">Az.IotHub</span></span>
* <span data-ttu-id="11aab-1095">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="11aab-1095">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="11aab-1096">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="11aab-1096">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="11aab-1097">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="11aab-1097">Az.Monitor</span></span>
* <span data-ttu-id="11aab-1098">Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="11aab-1098">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="11aab-1099">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="11aab-1099">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="11aab-1100">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="11aab-1100">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="11aab-1101">Os Webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="11aab-1101">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-1102">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-1102">Az.Network</span></span>
* <span data-ttu-id="11aab-1103">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="11aab-1103">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="11aab-1104">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="11aab-1104">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="11aab-1105">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="11aab-1105">New cmdlets added:</span></span>
        - <span data-ttu-id="11aab-1106">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="11aab-1106">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="11aab-1107">Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-1107">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="11aab-1108">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="11aab-1108">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="11aab-1109">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="11aab-1109">Updated cmdlets:</span></span>
        - <span data-ttu-id="11aab-1110">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-1110">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="11aab-1111">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-1111">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="11aab-1112">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-1112">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="11aab-1113">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="11aab-1113">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="11aab-1114">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="11aab-1114">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="11aab-1115">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="11aab-1115">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="11aab-1116">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="11aab-1116">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="11aab-1117">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="11aab-1117">Az.RedisCache</span></span>
* <span data-ttu-id="11aab-1118">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="11aab-1118">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-1119">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-1119">Az.Sql</span></span>
* <span data-ttu-id="11aab-1120">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="11aab-1120">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="11aab-1121">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-1121">Az.Storage</span></span>
* <span data-ttu-id="11aab-1122">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="11aab-1122">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="11aab-1123">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="11aab-1123">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="11aab-1124">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="11aab-1124">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="11aab-1125">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="11aab-1125">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="11aab-1126">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="11aab-1126">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="11aab-1127">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="11aab-1127">Az.StorageSync</span></span>
* <span data-ttu-id="11aab-1128">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="11aab-1128">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="11aab-1129">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="11aab-1129">Az.Websites</span></span>
* <span data-ttu-id="11aab-1130">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="11aab-1130">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="11aab-1131">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-1131">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="11aab-1132">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="11aab-1132">Az.ApiManagement</span></span>
* <span data-ttu-id="11aab-1133">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="11aab-1133">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="11aab-1134">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="11aab-1134">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="11aab-1135">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="11aab-1135">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="11aab-1136">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="11aab-1136">Az.Automation</span></span>
* <span data-ttu-id="11aab-1137">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="11aab-1137">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="11aab-1138">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="11aab-1138">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="11aab-1139">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="11aab-1139">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-1140">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-1140">Az.Compute</span></span>
* <span data-ttu-id="11aab-1141">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-1141">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="11aab-1142">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-1142">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="11aab-1143">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="11aab-1143">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="11aab-1144">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="11aab-1144">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="11aab-1145">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="11aab-1145">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="11aab-1146">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="11aab-1146">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="11aab-1147">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="11aab-1147">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="11aab-1148">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="11aab-1148">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="11aab-1149">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="11aab-1149">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="11aab-1150">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="11aab-1150">Az.DataFactory</span></span>
* <span data-ttu-id="11aab-1151">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="11aab-1151">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="11aab-1152">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="11aab-1152">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="11aab-1153">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="11aab-1153">Az.HDInsight</span></span>
* <span data-ttu-id="11aab-1154">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="11aab-1154">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="11aab-1155">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="11aab-1155">Az.IotHub</span></span>
* <span data-ttu-id="11aab-1156">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="11aab-1156">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="11aab-1157">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="11aab-1157">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="11aab-1158">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="11aab-1158">New cmdlets are:</span></span>
    - <span data-ttu-id="11aab-1159">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="11aab-1159">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="11aab-1160">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="11aab-1160">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="11aab-1161">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="11aab-1161">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="11aab-1162">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="11aab-1162">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="11aab-1163">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="11aab-1163">Az.Monitor</span></span>
* <span data-ttu-id="11aab-1164">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="11aab-1164">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="11aab-1165">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="11aab-1165">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="11aab-1166">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="11aab-1166">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="11aab-1167">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="11aab-1167">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="11aab-1168">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="11aab-1168">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="11aab-1169">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="11aab-1169">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="11aab-1170">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="11aab-1170">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="11aab-1171">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="11aab-1171">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="11aab-1172">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="11aab-1172">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="11aab-1173">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="11aab-1173">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="11aab-1174">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="11aab-1174">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="11aab-1175">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="11aab-1175">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="11aab-1176">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="11aab-1176">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="11aab-1177">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="11aab-1177">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="11aab-1178">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="11aab-1178">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="11aab-1179">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="11aab-1179">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="11aab-1180">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="11aab-1180">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="11aab-1181">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="11aab-1181">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="11aab-1182">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="11aab-1182">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="11aab-1183">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="11aab-1183">Overall improved help files</span></span>
* <span data-ttu-id="11aab-1184">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="11aab-1184">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-1185">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-1185">Az.Network</span></span>
* <span data-ttu-id="11aab-1186">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="11aab-1186">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span>
* <span data-ttu-id="11aab-1187">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="11aab-1187">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="11aab-1188">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="11aab-1188">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="11aab-1189">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="11aab-1189">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="11aab-1190">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="11aab-1190">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="11aab-1191">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="11aab-1191">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="11aab-1192">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="11aab-1192">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="11aab-1193">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="11aab-1193">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="11aab-1194">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="11aab-1194">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="11aab-1195">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="11aab-1195">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="11aab-1196">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="11aab-1196">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="11aab-1197">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="11aab-1197">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="11aab-1198">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="11aab-1198">New cmdlets</span></span>
        - <span data-ttu-id="11aab-1199">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="11aab-1199">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="11aab-1200">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-1200">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="11aab-1201">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="11aab-1201">Updated cmdlet:</span></span>
        - <span data-ttu-id="11aab-1202">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="11aab-1202">New-VpnSite</span></span>
        - <span data-ttu-id="11aab-1203">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="11aab-1203">Update-VpnSite</span></span>
        - <span data-ttu-id="11aab-1204">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-1204">New-VpnConnection</span></span>
        - <span data-ttu-id="11aab-1205">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-1205">Update-VpnConnection</span></span>
* <span data-ttu-id="11aab-1206">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="11aab-1206">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="11aab-1207">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="11aab-1207">Az.RecoveryServices</span></span>
* <span data-ttu-id="11aab-1208">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="11aab-1208">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="11aab-1209">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="11aab-1209">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-1210">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-1210">Az.Resources</span></span>
* <span data-ttu-id="11aab-1211">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="11aab-1211">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="11aab-1212">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="11aab-1212">Az.ServiceFabric</span></span>
* <span data-ttu-id="11aab-1213">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="11aab-1213">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="11aab-1214">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="11aab-1214">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="11aab-1215">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="11aab-1215">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="11aab-1216">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="11aab-1216">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="11aab-1217">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="11aab-1217">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="11aab-1218">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="11aab-1218">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="11aab-1219">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="11aab-1219">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="11aab-1220">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="11aab-1220">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="11aab-1221">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="11aab-1221">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="11aab-1222">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="11aab-1222">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="11aab-1223">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="11aab-1223">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="11aab-1224">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="11aab-1224">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="11aab-1225">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="11aab-1225">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="11aab-1226">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="11aab-1226">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="11aab-1227">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="11aab-1227">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="11aab-1228">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="11aab-1228">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="11aab-1229">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="11aab-1229">Az.SignalR</span></span>
* <span data-ttu-id="11aab-1230">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="11aab-1230">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-1231">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-1231">Az.Sql</span></span>
* <span data-ttu-id="11aab-1232">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="11aab-1232">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="11aab-1233">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="11aab-1233">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="11aab-1234">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="11aab-1234">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="11aab-1235">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="11aab-1235">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="11aab-1236">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="11aab-1236">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="11aab-1237">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-1237">Az.Storage</span></span>
* <span data-ttu-id="11aab-1238">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="11aab-1238">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="11aab-1239">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="11aab-1239">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="11aab-1240">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="11aab-1240">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="11aab-1241">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="11aab-1241">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="11aab-1242">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="11aab-1242">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="11aab-1243">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="11aab-1243">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="11aab-1244">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="11aab-1244">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="11aab-1245">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="11aab-1245">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="11aab-1246">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="11aab-1246">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="11aab-1247">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="11aab-1247">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="11aab-1248">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="11aab-1248">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="11aab-1249">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="11aab-1249">Az.Websites</span></span>
* <span data-ttu-id="11aab-1250">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="11aab-1250">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="11aab-1251">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="11aab-1251">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="11aab-1252">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="11aab-1252">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="11aab-1253">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-1253">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="11aab-1254">Geral</span><span class="sxs-lookup"><span data-stu-id="11aab-1254">General</span></span>
* <span data-ttu-id="11aab-1255">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="11aab-1255">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="11aab-1256">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-1256">Az.Accounts</span></span>
* <span data-ttu-id="11aab-1257">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="11aab-1257">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="11aab-1258">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="11aab-1258">Az.Aks</span></span>
* <span data-ttu-id="11aab-1259">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="11aab-1259">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="11aab-1260">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="11aab-1260">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="11aab-1261">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="11aab-1261">Az.ApiManagement</span></span>
* <span data-ttu-id="11aab-1262">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="11aab-1262">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="11aab-1263">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="11aab-1263">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="11aab-1264">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="11aab-1264">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="11aab-1265">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="11aab-1265">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="11aab-1266">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="11aab-1266">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="11aab-1267">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="11aab-1267">Az.Batch</span></span>
* <span data-ttu-id="11aab-1268">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="11aab-1268">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="11aab-1269">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="11aab-1269">Az.Cdn</span></span>
* <span data-ttu-id="11aab-1270">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="11aab-1270">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-1271">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-1271">Az.Compute</span></span>
* <span data-ttu-id="11aab-1272">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-1272">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="11aab-1273">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="11aab-1273">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="11aab-1274">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="11aab-1274">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="11aab-1275">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="11aab-1275">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="11aab-1276">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="11aab-1276">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="11aab-1277">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="11aab-1277">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="11aab-1278">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="11aab-1278">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="11aab-1279">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="11aab-1279">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="11aab-1280">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="11aab-1280">Az.DataFactory</span></span>
* <span data-ttu-id="11aab-1281">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="11aab-1281">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="11aab-1282">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="11aab-1282">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="11aab-1283">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="11aab-1283">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="11aab-1284">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="11aab-1284">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="11aab-1285">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="11aab-1285">Az.DataLakeStore</span></span>
* <span data-ttu-id="11aab-1286">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="11aab-1286">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="11aab-1287">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="11aab-1287">Az.EventHub</span></span>
* <span data-ttu-id="11aab-1288">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="11aab-1288">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="11aab-1289">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="11aab-1289">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="11aab-1290">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="11aab-1290">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="11aab-1291">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="11aab-1291">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="11aab-1292">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="11aab-1292">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="11aab-1293">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="11aab-1293">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="11aab-1294">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="11aab-1294">Az.Monitor</span></span>
* <span data-ttu-id="11aab-1295">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="11aab-1295">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-1296">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-1296">Az.Network</span></span>
* <span data-ttu-id="11aab-1297">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="11aab-1297">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="11aab-1298">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="11aab-1298">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="11aab-1299">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="11aab-1299">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="11aab-1300">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="11aab-1300">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="11aab-1301">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="11aab-1301">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span>
* <span data-ttu-id="11aab-1302">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="11aab-1302">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="11aab-1303">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="11aab-1303">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="11aab-1304">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="11aab-1304">Az.OperationalInsights</span></span>
* <span data-ttu-id="11aab-1305">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="11aab-1305">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="11aab-1306">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="11aab-1306">Added example</span></span>
    - <span data-ttu-id="11aab-1307">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="11aab-1307">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="11aab-1308">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="11aab-1308">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="11aab-1309">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="11aab-1309">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="11aab-1310">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="11aab-1310">Az.RecoveryServices</span></span>
* <span data-ttu-id="11aab-1311">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="11aab-1311">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-1312">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-1312">Az.Resources</span></span>
* <span data-ttu-id="11aab-1313">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="11aab-1313">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="11aab-1314">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="11aab-1314">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="11aab-1315">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="11aab-1315">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="11aab-1316">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="11aab-1316">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="11aab-1317">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="11aab-1317">Az.ServiceBus</span></span>
* <span data-ttu-id="11aab-1318">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="11aab-1318">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="11aab-1319">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="11aab-1319">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="11aab-1320">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="11aab-1320">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="11aab-1321">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="11aab-1321">Az.ServiceFabric</span></span>
* <span data-ttu-id="11aab-1322">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="11aab-1322">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="11aab-1323">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="11aab-1323">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="11aab-1324">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="11aab-1324">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="11aab-1325">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="11aab-1325">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="11aab-1326">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="11aab-1326">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="11aab-1327">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="11aab-1327">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-1328">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-1328">Az.Sql</span></span>
* <span data-ttu-id="11aab-1329">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="11aab-1329">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="11aab-1330">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-1330">Az.Storage</span></span>
* <span data-ttu-id="11aab-1331">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="11aab-1331">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="11aab-1332">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="11aab-1332">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="11aab-1333">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="11aab-1333">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="11aab-1334">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="11aab-1334">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="11aab-1335">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="11aab-1335">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="11aab-1336">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="11aab-1336">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="11aab-1337">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="11aab-1337">Az.Websites</span></span>
* <span data-ttu-id="11aab-1338">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="11aab-1338">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="11aab-1339">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-1339">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="11aab-1340">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-1340">Az.Accounts</span></span>
* <span data-ttu-id="11aab-1341">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="11aab-1341">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="11aab-1342">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="11aab-1342">Az.ApplicationInsights</span></span>
* <span data-ttu-id="11aab-1343">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="11aab-1343">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span>

#### <a name="azautomation"></a><span data-ttu-id="11aab-1344">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="11aab-1344">Az.Automation</span></span>
* <span data-ttu-id="11aab-1345">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="11aab-1345">Fix typo in resource string</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="11aab-1346">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="11aab-1346">Az.CognitiveServices</span></span>
* <span data-ttu-id="11aab-1347">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="11aab-1347">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-1348">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-1348">Az.Compute</span></span>
* <span data-ttu-id="11aab-1349">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="11aab-1349">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="11aab-1350">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="11aab-1350">Az.ContainerRegistry</span></span>
* <span data-ttu-id="11aab-1351">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="11aab-1351">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="11aab-1352">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="11aab-1352">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="11aab-1353">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="11aab-1353">Az.DataFactory</span></span>
* <span data-ttu-id="11aab-1354">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="11aab-1354">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="11aab-1355">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="11aab-1355">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="11aab-1356">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="11aab-1356">Az.EventHub</span></span>
* <span data-ttu-id="11aab-1357">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="11aab-1357">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="11aab-1358">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="11aab-1358">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="11aab-1359">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="11aab-1359">Az.KeyVault</span></span>
* <span data-ttu-id="11aab-1360">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="11aab-1360">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="11aab-1361">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="11aab-1361">Az.LogicApp</span></span>
* <span data-ttu-id="11aab-1362">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="11aab-1362">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="11aab-1363">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="11aab-1363">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="11aab-1364">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="11aab-1364">Az.ManagedServices</span></span>
* <span data-ttu-id="11aab-1365">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="11aab-1365">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-1366">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-1366">Az.Network</span></span>
* <span data-ttu-id="11aab-1367">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="11aab-1367">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="11aab-1368">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="11aab-1368">New cmdlets</span></span>
        - <span data-ttu-id="11aab-1369">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="11aab-1369">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="11aab-1370">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="11aab-1370">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="11aab-1371">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-1371">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="11aab-1372">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-1372">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="11aab-1373">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-1373">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="11aab-1374">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-1374">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="11aab-1375">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="11aab-1375">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="11aab-1376">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="11aab-1376">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="11aab-1377">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="11aab-1377">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="11aab-1378">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-1378">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="11aab-1379">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="11aab-1379">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="11aab-1380">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="11aab-1380">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="11aab-1381">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="11aab-1381">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="11aab-1382">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="11aab-1382">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="11aab-1383">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="11aab-1383">Updated cmdlets</span></span>
        - <span data-ttu-id="11aab-1384">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-1384">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="11aab-1385">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-1385">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="11aab-1386">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-1386">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="11aab-1387">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-1387">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="11aab-1388">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="11aab-1388">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="11aab-1389">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="11aab-1389">Updated cmdlet:</span></span>
        - <span data-ttu-id="11aab-1390">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-1390">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="11aab-1391">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-1391">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="11aab-1392">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-1392">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="11aab-1393">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="11aab-1393">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="11aab-1394">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="11aab-1394">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="11aab-1395">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="11aab-1395">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="11aab-1396">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="11aab-1396">Az.OperationalInsights</span></span>
* <span data-ttu-id="11aab-1397">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="11aab-1397">Updated default version for saved searches to be 1.</span></span>
* <span data-ttu-id="11aab-1398">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="11aab-1398">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="11aab-1399">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="11aab-1399">Az.RecoveryServices</span></span>
* <span data-ttu-id="11aab-1400">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="11aab-1400">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="11aab-1401">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="11aab-1401">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="11aab-1402">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="11aab-1402">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="11aab-1403">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="11aab-1403">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="11aab-1404">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="11aab-1404">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="11aab-1405">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="11aab-1405">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="11aab-1406">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="11aab-1406">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="11aab-1407">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="11aab-1407">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="11aab-1408">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="11aab-1408">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="11aab-1409">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="11aab-1409">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-1410">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-1410">Az.Resources</span></span>
- <span data-ttu-id="11aab-1411">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="11aab-1411">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="11aab-1412">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="11aab-1412">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="11aab-1413">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="11aab-1413">Az.ServiceBus</span></span>
* <span data-ttu-id="11aab-1414">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="11aab-1414">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="11aab-1415">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="11aab-1415">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-1416">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-1416">Az.Sql</span></span>
* <span data-ttu-id="11aab-1417">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="11aab-1417">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="11aab-1418">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="11aab-1418">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="11aab-1419">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="11aab-1419">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="11aab-1420">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-1420">Az.Storage</span></span>
* <span data-ttu-id="11aab-1421">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="11aab-1421">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="11aab-1422">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="11aab-1422">Az.StorageSync</span></span>
* <span data-ttu-id="11aab-1423">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="11aab-1423">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="11aab-1424">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="11aab-1424">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="11aab-1425">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="11aab-1425">Az.Websites</span></span>
* <span data-ttu-id="11aab-1426">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="11aab-1426">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="11aab-1427">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="11aab-1427">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="11aab-1428">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="11aab-1428">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="11aab-1429">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-1429">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="11aab-1430">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-1430">Az.Accounts</span></span>
* <span data-ttu-id="11aab-1431">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="11aab-1431">Add support for profile cmdlets</span></span>
* <span data-ttu-id="11aab-1432">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="11aab-1432">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="11aab-1433">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="11aab-1433">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="11aab-1434">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="11aab-1434">Az.Advisor</span></span>
* <span data-ttu-id="11aab-1435">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="11aab-1435">GA release of Az.Advisor</span></span>
* <span data-ttu-id="11aab-1436">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="11aab-1436">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="11aab-1437">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="11aab-1437">Az.ApiManagement</span></span>
* <span data-ttu-id="11aab-1438">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="11aab-1438">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="11aab-1439">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="11aab-1439">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="11aab-1440">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="11aab-1440">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="11aab-1441">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="11aab-1441">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="11aab-1442">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="11aab-1442">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="11aab-1443">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="11aab-1443">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="11aab-1444">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="11aab-1444">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="11aab-1445">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="11aab-1445">Az.Automation</span></span>
* <span data-ttu-id="11aab-1446">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="11aab-1446">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-1447">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-1447">Az.Compute</span></span>
* <span data-ttu-id="11aab-1448">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-1448">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="11aab-1449">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="11aab-1449">Az.DataFactory</span></span>
* <span data-ttu-id="11aab-1450">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="11aab-1450">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="11aab-1451">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="11aab-1451">Az.EventGrid</span></span>
* <span data-ttu-id="11aab-1452">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="11aab-1452">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="11aab-1453">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="11aab-1453">Az.IotHub</span></span>
* <span data-ttu-id="11aab-1454">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="11aab-1454">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-1455">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-1455">Az.Network</span></span>
* <span data-ttu-id="11aab-1456">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="11aab-1456">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="11aab-1457">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="11aab-1457">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="11aab-1458">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="11aab-1458">Az.PolicyInsights</span></span>
* <span data-ttu-id="11aab-1459">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="11aab-1459">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="11aab-1460">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="11aab-1460">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="11aab-1461">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="11aab-1461">Az.OperationalInsights</span></span>
* <span data-ttu-id="11aab-1462">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="11aab-1462">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="11aab-1463">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="11aab-1463">Az.RecoveryServices</span></span>
* <span data-ttu-id="11aab-1464">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="11aab-1464">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-1465">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-1465">Az.Resources</span></span>
    - <span data-ttu-id="11aab-1466">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="11aab-1466">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="11aab-1467">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="11aab-1467">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="11aab-1468">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="11aab-1468">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="11aab-1469">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="11aab-1469">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="11aab-1470">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="11aab-1470">Az.ServiceBus</span></span>
* <span data-ttu-id="11aab-1471">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="11aab-1471">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-1472">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-1472">Az.Sql</span></span>
* <span data-ttu-id="11aab-1473">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="11aab-1473">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="11aab-1474">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="11aab-1474">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="11aab-1475">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="11aab-1475">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="11aab-1476">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="11aab-1476">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="11aab-1477">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="11aab-1477">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="11aab-1478">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="11aab-1478">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="11aab-1479">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="11aab-1479">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="11aab-1480">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="11aab-1480">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="11aab-1481">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="11aab-1481">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="11aab-1482">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-1482">Az.Storage</span></span>
* <span data-ttu-id="11aab-1483">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="11aab-1483">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="11aab-1484">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="11aab-1484">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="11aab-1485">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="11aab-1485">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="11aab-1486">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="11aab-1486">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="11aab-1487">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="11aab-1487">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="11aab-1488">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="11aab-1488">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="11aab-1489">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="11aab-1489">Set-AzStorageAccount</span></span>
* <span data-ttu-id="11aab-1490">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="11aab-1490">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="11aab-1491">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="11aab-1491">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="11aab-1492">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="11aab-1492">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="11aab-1493">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="11aab-1493">Az.StorageSync</span></span>
* <span data-ttu-id="11aab-1494">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="11aab-1494">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="11aab-1495">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-1495">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="11aab-1496">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-1496">Az.Accounts</span></span>
* <span data-ttu-id="11aab-1497">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="11aab-1497">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="11aab-1498">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="11aab-1498">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="11aab-1499">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="11aab-1499">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="11aab-1500">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="11aab-1500">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="11aab-1501">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="11aab-1501">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-1502">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-1502">Az.Compute</span></span>
* <span data-ttu-id="11aab-1503">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="11aab-1503">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="11aab-1504">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="11aab-1504">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="11aab-1505">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="11aab-1505">Az.Dns</span></span>
* <span data-ttu-id="11aab-1506">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="11aab-1506">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="11aab-1507">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="11aab-1507">Az.EventGrid</span></span>
* <span data-ttu-id="11aab-1508">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="11aab-1508">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="11aab-1509">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="11aab-1509">New cmdlets:</span></span>
    - <span data-ttu-id="11aab-1510">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="11aab-1510">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="11aab-1511">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="11aab-1511">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="11aab-1512">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="11aab-1512">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="11aab-1513">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-1513">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="11aab-1514">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="11aab-1514">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="11aab-1515">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="11aab-1515">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="11aab-1516">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="11aab-1516">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="11aab-1517">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="11aab-1517">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="11aab-1518">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="11aab-1518">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="11aab-1519">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="11aab-1519">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="11aab-1520">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="11aab-1520">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="11aab-1521">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="11aab-1521">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="11aab-1522">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="11aab-1522">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="11aab-1523">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="11aab-1523">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span>
    - <span data-ttu-id="11aab-1524">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="11aab-1524">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="11aab-1525">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="11aab-1525">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="11aab-1526">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="11aab-1526">Updated cmdlets:</span></span>
    - <span data-ttu-id="11aab-1527">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="11aab-1527">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="11aab-1528">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="11aab-1528">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="11aab-1529">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="11aab-1529">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="11aab-1530">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="11aab-1530">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="11aab-1531">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="11aab-1531">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="11aab-1532">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="11aab-1532">Event subscription expiration date,</span></span>
            - <span data-ttu-id="11aab-1533">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="11aab-1533">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="11aab-1534">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="11aab-1534">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="11aab-1535">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="11aab-1535">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span>
    - <span data-ttu-id="11aab-1536">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="11aab-1536">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="11aab-1537">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="11aab-1537">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="11aab-1538">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="11aab-1538">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="11aab-1539">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="11aab-1539">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="11aab-1540">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="11aab-1540">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="11aab-1541">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="11aab-1541">Az.FrontDoor</span></span>
* <span data-ttu-id="11aab-1542">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="11aab-1542">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="11aab-1543">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="11aab-1543">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="11aab-1544">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="11aab-1544">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="11aab-1545">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="11aab-1545">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-1546">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-1546">Az.Network</span></span>
* <span data-ttu-id="11aab-1547">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="11aab-1547">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="11aab-1548">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="11aab-1548">New cmdlets</span></span>
        - <span data-ttu-id="11aab-1549">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="11aab-1549">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="11aab-1550">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="11aab-1550">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="11aab-1551">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="11aab-1551">New cmdlets</span></span>
        - <span data-ttu-id="11aab-1552">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="11aab-1552">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="11aab-1553">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="11aab-1553">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="11aab-1554">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="11aab-1554">New cmdlets</span></span>
        - <span data-ttu-id="11aab-1555">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="11aab-1555">Get-AzPrivateLinkService</span></span>
        - <span data-ttu-id="11aab-1556">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="11aab-1556">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="11aab-1557">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="11aab-1557">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="11aab-1558">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-1558">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="11aab-1559">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-1559">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="11aab-1560">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="11aab-1560">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="11aab-1561">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="11aab-1561">New cmdlets</span></span>
        - <span data-ttu-id="11aab-1562">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="11aab-1562">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="11aab-1563">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="11aab-1563">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="11aab-1564">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="11aab-1564">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="11aab-1565">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-1565">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="11aab-1566">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="11aab-1566">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="11aab-1567">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="11aab-1567">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="11aab-1568">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="11aab-1568">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="11aab-1569">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="11aab-1569">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="11aab-1570">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="11aab-1570">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="11aab-1571">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="11aab-1571">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="11aab-1572">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="11aab-1572">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="11aab-1573">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="11aab-1573">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="11aab-1574">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="11aab-1574">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="11aab-1575">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="11aab-1575">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="11aab-1576">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="11aab-1576">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="11aab-1577">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="11aab-1577">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="11aab-1578">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="11aab-1578">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="11aab-1579">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="11aab-1579">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="11aab-1580">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="11aab-1580">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="11aab-1581">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="11aab-1581">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="11aab-1582">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="11aab-1582">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="11aab-1583">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="11aab-1583">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="11aab-1584">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="11aab-1584">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span>
* <span data-ttu-id="11aab-1585">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="11aab-1585">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span>
    - <span data-ttu-id="11aab-1586">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="11aab-1586">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="11aab-1587">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="11aab-1587">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="11aab-1588">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="11aab-1588">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="11aab-1589">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="11aab-1589">Az.OperationalInsights</span></span>
* <span data-ttu-id="11aab-1590">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="11aab-1590">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-1591">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-1591">Az.Resources</span></span>
* <span data-ttu-id="11aab-1592">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="11aab-1592">Support for additional Template Export options</span></span>
    - <span data-ttu-id="11aab-1593">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="11aab-1593">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="11aab-1594">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="11aab-1594">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="11aab-1595">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="11aab-1595">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="11aab-1596">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="11aab-1596">Az.ServiceFabric</span></span>
* <span data-ttu-id="11aab-1597">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="11aab-1597">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-1598">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-1598">Az.Sql</span></span>
* <span data-ttu-id="11aab-1599">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="11aab-1599">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="11aab-1600">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="11aab-1600">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="11aab-1601">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="11aab-1601">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="11aab-1602">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="11aab-1602">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="11aab-1603">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="11aab-1603">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="11aab-1604">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="11aab-1604">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="11aab-1605">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="11aab-1605">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="11aab-1606">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="11aab-1606">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="11aab-1607">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-1607">Az.Storage</span></span>
* <span data-ttu-id="11aab-1608">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="11aab-1608">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="11aab-1609">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="11aab-1609">New-AzStorageAccount</span></span>
* <span data-ttu-id="11aab-1610">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="11aab-1610">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="11aab-1611">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="11aab-1611">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="11aab-1612">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="11aab-1612">Az.Websites</span></span>
* <span data-ttu-id="11aab-1613">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="11aab-1613">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="11aab-1614">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="11aab-1614">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="11aab-1615">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-1615">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="11aab-1616">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="11aab-1616">Az.Cdn</span></span>
* <span data-ttu-id="11aab-1617">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="11aab-1617">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-1618">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-1618">Az.Compute</span></span>
* <span data-ttu-id="11aab-1619">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="11aab-1619">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="11aab-1620">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="11aab-1620">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="11aab-1621">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="11aab-1621">Az.EventHub</span></span>
* <span data-ttu-id="11aab-1622">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="11aab-1622">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="11aab-1623">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="11aab-1623">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-1624">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-1624">Az.Network</span></span>
* <span data-ttu-id="11aab-1625">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="11aab-1625">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="11aab-1626">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="11aab-1626">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="11aab-1627">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="11aab-1627">Az.PolicyInsights</span></span>
* <span data-ttu-id="11aab-1628">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="11aab-1628">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="11aab-1629">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="11aab-1629">Az.RecoveryServices</span></span>
* <span data-ttu-id="11aab-1630">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="11aab-1630">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="11aab-1631">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="11aab-1631">Az.ServiceBus</span></span>
* <span data-ttu-id="11aab-1632">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="11aab-1632">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="11aab-1633">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="11aab-1633">Az.ServiceFabric</span></span>
* <span data-ttu-id="11aab-1634">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="11aab-1634">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="11aab-1635">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="11aab-1635">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-1636">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-1636">Az.Sql</span></span>
* <span data-ttu-id="11aab-1637">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="11aab-1637">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="11aab-1638">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="11aab-1638">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="11aab-1639">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="11aab-1639">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="11aab-1640">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="11aab-1640">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="11aab-1641">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="11aab-1641">Az.Websites</span></span>
* <span data-ttu-id="11aab-1642">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="11aab-1642">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="11aab-1643">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-1643">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="11aab-1644">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="11aab-1644">Az.ApiManagement</span></span>
* <span data-ttu-id="11aab-1645">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="11aab-1645">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="11aab-1646">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="11aab-1646">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="11aab-1647">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="11aab-1647">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="11aab-1648">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="11aab-1648">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="11aab-1649">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="11aab-1649">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="11aab-1650">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="11aab-1650">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="11aab-1651">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="11aab-1651">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="11aab-1652">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="11aab-1652">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="11aab-1653">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="11aab-1653">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="11aab-1654">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="11aab-1654">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="11aab-1655">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="11aab-1655">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="11aab-1656">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="11aab-1656">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="11aab-1657">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="11aab-1657">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="11aab-1658">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="11aab-1658">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="11aab-1659">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="11aab-1659">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="11aab-1660">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="11aab-1660">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="11aab-1661">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="11aab-1661">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="11aab-1662">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="11aab-1662">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="11aab-1663">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="11aab-1663">Created new Cmdlet for generating a User Token.</span></span>
    - <span data-ttu-id="11aab-1664">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="11aab-1664">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="11aab-1665">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="11aab-1665">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="11aab-1666">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="11aab-1666">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="11aab-1667">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="11aab-1667">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="11aab-1668">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="11aab-1668">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span>
    - <span data-ttu-id="11aab-1669">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="11aab-1669">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="11aab-1670">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="11aab-1670">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="11aab-1671">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="11aab-1671">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="11aab-1672">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="11aab-1672">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="11aab-1673">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="11aab-1673">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="11aab-1674">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="11aab-1674">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="11aab-1675">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="11aab-1675">Updated the cmdlet to display Error Messages inline</span></span>
     > <span data-ttu-id="11aab-1676">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="11aab-1676">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="11aab-1677">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="11aab-1677">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="11aab-1678">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="11aab-1678">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="11aab-1679">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="11aab-1679">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="11aab-1680">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="11aab-1680">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="11aab-1681">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="11aab-1681">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="11aab-1682">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="11aab-1682">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="11aab-1683">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="11aab-1683">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="11aab-1684">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="11aab-1684">Updated cmdlet **New-AzApiManagementApi**</span></span>
    - <span data-ttu-id="11aab-1685">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="11aab-1685">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="11aab-1686">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="11aab-1686">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="11aab-1687">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="11aab-1687">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="11aab-1688">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="11aab-1688">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="11aab-1689">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="11aab-1689">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="11aab-1690">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="11aab-1690">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="11aab-1691">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="11aab-1691">To updated an API into an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="11aab-1692">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="11aab-1692">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="11aab-1693">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="11aab-1693">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="11aab-1694">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="11aab-1694">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="11aab-1695">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="11aab-1695">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="11aab-1696">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="11aab-1696">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="11aab-1697">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="11aab-1697">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="11aab-1698">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="11aab-1698">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="11aab-1699">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="11aab-1699">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="11aab-1700">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="11aab-1700">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="11aab-1701">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="11aab-1701">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="11aab-1702">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="11aab-1702">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="11aab-1703">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="11aab-1703">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="11aab-1704">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="11aab-1704">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="11aab-1705">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="11aab-1705">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="11aab-1706">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="11aab-1706">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="11aab-1707">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="11aab-1707">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="11aab-1708">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="11aab-1708">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="11aab-1709">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="11aab-1709">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="11aab-1710">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="11aab-1710">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="11aab-1711">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="11aab-1711">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="11aab-1712">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="11aab-1712">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="11aab-1713">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="11aab-1713">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="11aab-1714">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="11aab-1714">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="11aab-1715">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="11aab-1715">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="11aab-1716">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="11aab-1716">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="11aab-1717">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="11aab-1717">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="11aab-1718">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="11aab-1718">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="11aab-1719">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="11aab-1719">'Get-AzApiManagementCertificate'</span></span>
    - <span data-ttu-id="11aab-1720">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="11aab-1720">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="11aab-1721">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="11aab-1721">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="11aab-1722">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="11aab-1722">Az.Automation</span></span>
* <span data-ttu-id="11aab-1723">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="11aab-1723">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="11aab-1724">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="11aab-1724">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="11aab-1725">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="11aab-1725">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="11aab-1726">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="11aab-1726">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="11aab-1727">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="11aab-1727">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="11aab-1728">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="11aab-1728">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="11aab-1729">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="11aab-1729">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-1730">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-1730">Az.Compute</span></span>
* <span data-ttu-id="11aab-1731">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="11aab-1731">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="11aab-1732">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="11aab-1732">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="11aab-1733">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="11aab-1733">Az.DataLakeStore</span></span>
* <span data-ttu-id="11aab-1734">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="11aab-1734">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="11aab-1735">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="11aab-1735">Az.Monitor</span></span>
* <span data-ttu-id="11aab-1736">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="11aab-1736">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-1737">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-1737">Az.Network</span></span>
* <span data-ttu-id="11aab-1738">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="11aab-1738">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="11aab-1739">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="11aab-1739">Updated cmdlet:</span></span>
        - <span data-ttu-id="11aab-1740">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="11aab-1740">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="11aab-1741">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="11aab-1741">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-1742">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-1742">Az.Resources</span></span>
* <span data-ttu-id="11aab-1743">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="11aab-1743">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-1744">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-1744">Az.Sql</span></span>
* <span data-ttu-id="11aab-1745">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="11aab-1745">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="11aab-1746">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-1746">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="11aab-1747">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-1747">Az.Accounts</span></span>
* <span data-ttu-id="11aab-1748">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="11aab-1748">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="11aab-1749">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="11aab-1749">Az.CognitiveServices</span></span>
* <span data-ttu-id="11aab-1750">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="11aab-1750">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="11aab-1751">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="11aab-1751">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-1752">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-1752">Az.Compute</span></span>
* <span data-ttu-id="11aab-1753">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="11aab-1753">Proximity placement group feature.</span></span>
    - <span data-ttu-id="11aab-1754">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="11aab-1754">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="11aab-1755">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-1755">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="11aab-1756">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="11aab-1756">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="11aab-1757">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="11aab-1757">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="11aab-1758">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="11aab-1758">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>
* <span data-ttu-id="11aab-1759">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="11aab-1759">Breaking changes</span></span>
    - <span data-ttu-id="11aab-1760">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="11aab-1760">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="11aab-1761">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="11aab-1761">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="11aab-1762">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="11aab-1762">Az.DeploymentManager</span></span>
* <span data-ttu-id="11aab-1763">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="11aab-1763">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="11aab-1764">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="11aab-1764">Az.Dns</span></span>
* <span data-ttu-id="11aab-1765">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="11aab-1765">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="11aab-1766">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="11aab-1766">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="11aab-1767">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="11aab-1767">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="11aab-1768">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="11aab-1768">Az.FrontDoor</span></span>
* <span data-ttu-id="11aab-1769">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="11aab-1769">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="11aab-1770">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="11aab-1770">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="11aab-1771">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="11aab-1771">Az.HDInsight</span></span>
* <span data-ttu-id="11aab-1772">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="11aab-1772">Removed two cmdlets:</span></span>
    - <span data-ttu-id="11aab-1773">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="11aab-1773">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="11aab-1774">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="11aab-1774">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="11aab-1775">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="11aab-1775">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="11aab-1776">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="11aab-1776">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="11aab-1777">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="11aab-1777">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="11aab-1778">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="11aab-1778">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="11aab-1779">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="11aab-1779">Az.Monitor</span></span>
* <span data-ttu-id="11aab-1780">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="11aab-1780">New cmdlets for SQR API (Scheduled Query Rule)</span></span>
    - <span data-ttu-id="11aab-1781">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="11aab-1781">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="11aab-1782">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="11aab-1782">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="11aab-1783">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="11aab-1783">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="11aab-1784">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="11aab-1784">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="11aab-1785">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="11aab-1785">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="11aab-1786">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="11aab-1786">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="11aab-1787">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="11aab-1787">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="11aab-1788">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="11aab-1788">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="11aab-1789">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="11aab-1789">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="11aab-1790">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="11aab-1790">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="11aab-1791">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="11aab-1791">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="11aab-1792">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="11aab-1792">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="11aab-1793">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="11aab-1793">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-1794">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-1794">Az.Network</span></span>
* <span data-ttu-id="11aab-1795">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="11aab-1795">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="11aab-1796">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="11aab-1796">New cmdlets</span></span>
        - <span data-ttu-id="11aab-1797">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="11aab-1797">New-AzNatGateway</span></span>
        - <span data-ttu-id="11aab-1798">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="11aab-1798">Get-AzNatGateway</span></span>
        - <span data-ttu-id="11aab-1799">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="11aab-1799">Set-AzNatGateway</span></span>
        - <span data-ttu-id="11aab-1800">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="11aab-1800">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="11aab-1801">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="11aab-1801">Updated cmdlets</span></span>
        - <span data-ttu-id="11aab-1802">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="11aab-1802">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="11aab-1803">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="11aab-1803">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="11aab-1804">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="11aab-1804">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="11aab-1805">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="11aab-1805">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="11aab-1806">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="11aab-1806">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="11aab-1807">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="11aab-1807">Az.PolicyInsights</span></span>
* <span data-ttu-id="11aab-1808">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="11aab-1808">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="11aab-1809">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="11aab-1809">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="11aab-1810">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="11aab-1810">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="11aab-1811">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="11aab-1811">Az.RecoveryServices</span></span>
* <span data-ttu-id="11aab-1812">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="11aab-1812">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="11aab-1813">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="11aab-1813">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="11aab-1814">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="11aab-1814">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="11aab-1815">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-1815">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="11aab-1816">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="11aab-1816">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="11aab-1817">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="11aab-1817">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="11aab-1818">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="11aab-1818">Az.Relay</span></span>
* <span data-ttu-id="11aab-1819">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="11aab-1819">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="11aab-1820">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="11aab-1820">Az.ServiceBus</span></span>
* <span data-ttu-id="11aab-1821">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="11aab-1821">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="11aab-1822">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-1822">Az.Storage</span></span>
* <span data-ttu-id="11aab-1823">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="11aab-1823">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="11aab-1824">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="11aab-1824">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="11aab-1825">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="11aab-1825">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="11aab-1826">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="11aab-1826">New-AzStorageAccount</span></span>
* <span data-ttu-id="11aab-1827">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="11aab-1827">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="11aab-1828">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="11aab-1828">New-AzStorageAccount</span></span>
    - <span data-ttu-id="11aab-1829">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="11aab-1829">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="11aab-1830">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="11aab-1830">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="11aab-1831">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="11aab-1831">Az.Websites</span></span>
* <span data-ttu-id="11aab-1832">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="11aab-1832">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="11aab-1833">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="11aab-1833">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="11aab-1834">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-1834">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="11aab-1835">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="11aab-1835">Highlights since the last major release</span></span>
* <span data-ttu-id="11aab-1836">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="11aab-1836">General availability of `Az` module</span></span>
* <span data-ttu-id="11aab-1837">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="11aab-1837">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="11aab-1838">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="11aab-1838">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="11aab-1839">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-1839">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="11aab-1840">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="11aab-1840">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="11aab-1841">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="11aab-1841">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="11aab-1842">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="11aab-1842">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="11aab-1843">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-1843">Az.Accounts</span></span>
* <span data-ttu-id="11aab-1844">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="11aab-1844">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="11aab-1845">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="11aab-1845">Az.Batch</span></span>
* <span data-ttu-id="11aab-1846">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="11aab-1846">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="11aab-1847">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="11aab-1847">Az.Cdn</span></span>
* <span data-ttu-id="11aab-1848">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="11aab-1848">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="11aab-1849">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="11aab-1849">Az.CognitiveServices</span></span>
* <span data-ttu-id="11aab-1850">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="11aab-1850">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-1851">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-1851">Az.Compute</span></span>
* <span data-ttu-id="11aab-1852">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="11aab-1852">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="11aab-1853">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="11aab-1853">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="11aab-1854">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="11aab-1854">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="11aab-1855">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="11aab-1855">Az.DataFactory</span></span>
* <span data-ttu-id="11aab-1856">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="11aab-1856">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="11aab-1857">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="11aab-1857">Az.DataLakeStore</span></span>
* <span data-ttu-id="11aab-1858">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="11aab-1858">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="11aab-1859">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="11aab-1859">Az.EventGrid</span></span>
* <span data-ttu-id="11aab-1860">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="11aab-1860">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="11aab-1861">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="11aab-1861">Az.EventHub</span></span>
* <span data-ttu-id="11aab-1862">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="11aab-1862">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="11aab-1863">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="11aab-1863">Az.HDInsight</span></span>
* <span data-ttu-id="11aab-1864">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="11aab-1864">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="11aab-1865">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="11aab-1865">Az.IotHub</span></span>
* <span data-ttu-id="11aab-1866">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="11aab-1866">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="11aab-1867">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="11aab-1867">Az.KeyVault</span></span>
* <span data-ttu-id="11aab-1868">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="11aab-1868">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="11aab-1869">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="11aab-1869">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="11aab-1870">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="11aab-1870">Az.MachineLearning</span></span>
* <span data-ttu-id="11aab-1871">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="11aab-1871">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="11aab-1872">Az.Media</span><span class="sxs-lookup"><span data-stu-id="11aab-1872">Az.Media</span></span>
* <span data-ttu-id="11aab-1873">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="11aab-1873">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="11aab-1874">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="11aab-1874">Az.Monitor</span></span>
  * <span data-ttu-id="11aab-1875">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="11aab-1875">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="11aab-1876">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="11aab-1876">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="11aab-1877">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="11aab-1877">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="11aab-1878">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="11aab-1878">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="11aab-1879">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="11aab-1879">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="11aab-1880">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="11aab-1880">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="11aab-1881">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="11aab-1881">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-1882">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-1882">Az.Network</span></span>
* <span data-ttu-id="11aab-1883">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="11aab-1883">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="11aab-1884">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="11aab-1884">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="11aab-1885">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="11aab-1885">Az.NotificationHubs</span></span>
* <span data-ttu-id="11aab-1886">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="11aab-1886">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="11aab-1887">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="11aab-1887">Az.OperationalInsights</span></span>
* <span data-ttu-id="11aab-1888">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="11aab-1888">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="11aab-1889">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="11aab-1889">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="11aab-1890">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="11aab-1890">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="11aab-1891">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="11aab-1891">Az.RecoveryServices</span></span>
* <span data-ttu-id="11aab-1892">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="11aab-1892">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="11aab-1893">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="11aab-1893">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="11aab-1894">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="11aab-1894">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="11aab-1895">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="11aab-1895">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="11aab-1896">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="11aab-1896">Az.RedisCache</span></span>
* <span data-ttu-id="11aab-1897">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="11aab-1897">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-1898">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-1898">Az.Resources</span></span>
* <span data-ttu-id="11aab-1899">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="11aab-1899">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-1900">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-1900">Az.Sql</span></span>
* <span data-ttu-id="11aab-1901">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="11aab-1901">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="11aab-1902">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="11aab-1902">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="11aab-1903">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="11aab-1903">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="11aab-1904">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="11aab-1904">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="11aab-1905">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="11aab-1905">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="11aab-1906">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="11aab-1906">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="11aab-1907">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="11aab-1907">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="11aab-1908">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="11aab-1908">Az.Websites</span></span>
* <span data-ttu-id="11aab-1909">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="11aab-1909">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="11aab-1910">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="11aab-1910">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="11aab-1911">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="11aab-1911">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="11aab-1912">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="11aab-1912">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="11aab-1913">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-1913">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="11aab-1914">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="11aab-1914">Highlights since the last major release</span></span>
* <span data-ttu-id="11aab-1915">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="11aab-1915">General availability of `Az` module</span></span>
* <span data-ttu-id="11aab-1916">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="11aab-1916">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="11aab-1917">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="11aab-1917">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="11aab-1918">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-1918">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="11aab-1919">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="11aab-1919">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="11aab-1920">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="11aab-1920">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="11aab-1921">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="11aab-1921">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="11aab-1922">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-1922">Az.Accounts</span></span>
* <span data-ttu-id="11aab-1923">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="11aab-1923">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="11aab-1924">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="11aab-1924">Az.AnalysisServices</span></span>
* <span data-ttu-id="11aab-1925">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="11aab-1925">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="11aab-1926">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="11aab-1926">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="11aab-1927">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="11aab-1927">Az.Automation</span></span>
* <span data-ttu-id="11aab-1928">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="11aab-1928">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="11aab-1929">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="11aab-1929">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="11aab-1930">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="11aab-1930">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-1931">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-1931">Az.Compute</span></span>
* <span data-ttu-id="11aab-1932">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-1932">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="11aab-1933">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="11aab-1933">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="11aab-1934">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="11aab-1934">Az.ContainerInstance</span></span>
* <span data-ttu-id="11aab-1935">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="11aab-1935">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="11aab-1936">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="11aab-1936">Az.DataFactory</span></span>
* <span data-ttu-id="11aab-1937">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="11aab-1937">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="11aab-1938">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="11aab-1938">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-1939">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-1939">Az.Resources</span></span>
* <span data-ttu-id="11aab-1940">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="11aab-1940">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="11aab-1941">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="11aab-1941">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="11aab-1942">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="11aab-1942">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="11aab-1943">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="11aab-1943">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="11aab-1944">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="11aab-1944">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="11aab-1945">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="11aab-1945">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-1946">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-1946">Az.Sql</span></span>
* <span data-ttu-id="11aab-1947">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="11aab-1947">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="11aab-1948">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-1948">Az.Storage</span></span>
* <span data-ttu-id="11aab-1949">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="11aab-1949">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="11aab-1950">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="11aab-1950">New-AzStorageContext</span></span>
* <span data-ttu-id="11aab-1951">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="11aab-1951">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="11aab-1952">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="11aab-1952">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="11aab-1953">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="11aab-1953">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="11aab-1954">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="11aab-1954">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="11aab-1955">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="11aab-1955">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="11aab-1956">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="11aab-1956">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="11aab-1957">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="11aab-1957">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="11aab-1958">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="11aab-1958">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="11aab-1959">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="11aab-1959">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="11aab-1960">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="11aab-1960">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="11aab-1961">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-1961">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="11aab-1962">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="11aab-1962">Highlights since the last major release</span></span>
* <span data-ttu-id="11aab-1963">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="11aab-1963">General availability of `Az` module</span></span>
* <span data-ttu-id="11aab-1964">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="11aab-1964">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="11aab-1965">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="11aab-1965">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="11aab-1966">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-1966">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="11aab-1967">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="11aab-1967">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="11aab-1968">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="11aab-1968">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="11aab-1969">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="11aab-1969">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="11aab-1970">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="11aab-1970">Az.Automation</span></span>
* <span data-ttu-id="11aab-1971">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="11aab-1971">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="11aab-1972">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="11aab-1972">Dynamic grouping</span></span>
    * <span data-ttu-id="11aab-1973">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="11aab-1973">Pre-Post script</span></span>
    * <span data-ttu-id="11aab-1974">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="11aab-1974">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-1975">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-1975">Az.Compute</span></span>
* <span data-ttu-id="11aab-1976">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="11aab-1976">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="11aab-1977">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="11aab-1977">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="11aab-1978">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="11aab-1978">Az.KeyVault</span></span>
* <span data-ttu-id="11aab-1979">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="11aab-1979">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-1980">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-1980">Az.Network</span></span>
* <span data-ttu-id="11aab-1981">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="11aab-1981">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="11aab-1982">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="11aab-1982">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="11aab-1983">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="11aab-1983">Az.RecoveryServices</span></span>
* <span data-ttu-id="11aab-1984">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="11aab-1984">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="11aab-1985">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="11aab-1985">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-1986">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-1986">Az.Resources</span></span>
* <span data-ttu-id="11aab-1987">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="11aab-1987">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="11aab-1988">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="11aab-1988">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-1989">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-1989">Az.Sql</span></span>
* <span data-ttu-id="11aab-1990">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="11aab-1990">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="11aab-1991">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-1991">Az.Storage</span></span>
* <span data-ttu-id="11aab-1992">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="11aab-1992">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="11aab-1993">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="11aab-1993">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="11aab-1994">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="11aab-1994">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="11aab-1995">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="11aab-1995">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="11aab-1996">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="11aab-1996">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="11aab-1997">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="11aab-1997">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="11aab-1998">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="11aab-1998">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="11aab-1999">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="11aab-1999">Az.Websites</span></span>
* <span data-ttu-id="11aab-2000">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="11aab-2000">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="11aab-2001">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-2001">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="11aab-2002">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-2002">Az.Accounts</span></span>
* <span data-ttu-id="11aab-2003">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="11aab-2003">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="11aab-2004">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="11aab-2004">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="11aab-2005">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="11aab-2005">Az.Automation</span></span>
* <span data-ttu-id="11aab-2006">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="11aab-2006">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="11aab-2007">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="11aab-2007">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="11aab-2008">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="11aab-2008">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="11aab-2009">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="11aab-2009">Az.Cdn</span></span>
* <span data-ttu-id="11aab-2010">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="11aab-2010">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-2011">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-2011">Az.Compute</span></span>
* <span data-ttu-id="11aab-2012">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="11aab-2012">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="11aab-2013">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="11aab-2013">Az.DataFactory</span></span>
* <span data-ttu-id="11aab-2014">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="11aab-2014">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="11aab-2015">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="11aab-2015">Az.LogicApp</span></span>
* <span data-ttu-id="11aab-2016">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="11aab-2016">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-2017">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-2017">Az.Network</span></span>
* <span data-ttu-id="11aab-2018">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="11aab-2018">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="11aab-2019">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="11aab-2019">Az.RecoveryServices</span></span>
* <span data-ttu-id="11aab-2020">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="11aab-2020">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="11aab-2021">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="11aab-2021">SDK Update</span></span>
* <span data-ttu-id="11aab-2022">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="11aab-2022">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="11aab-2023">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="11aab-2023">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-2024">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-2024">Az.Resources</span></span>
* <span data-ttu-id="11aab-2025">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="11aab-2025">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="11aab-2026">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="11aab-2026">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="11aab-2027">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="11aab-2027">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="11aab-2028">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="11aab-2028">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="11aab-2029">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="11aab-2029">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="11aab-2030">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="11aab-2030">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-2031">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-2031">Az.Sql</span></span>
* <span data-ttu-id="11aab-2032">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="11aab-2032">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="11aab-2033">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="11aab-2033">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="11aab-2034">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-2034">Az.Storage</span></span>
* <span data-ttu-id="11aab-2035">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="11aab-2035">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="11aab-2036">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-2036">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="11aab-2037">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="11aab-2037">Az.AnalysisServices</span></span>
* <span data-ttu-id="11aab-2038">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="11aab-2038">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="11aab-2039">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="11aab-2039">Az.Automation</span></span>
* <span data-ttu-id="11aab-2040">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="11aab-2040">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="11aab-2041">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="11aab-2041">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="11aab-2042">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="11aab-2042">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="11aab-2043">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="11aab-2043">Az.CognitiveServices</span></span>
* <span data-ttu-id="11aab-2044">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="11aab-2044">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-2045">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-2045">Az.Compute</span></span>
* <span data-ttu-id="11aab-2046">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="11aab-2046">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="11aab-2047">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="11aab-2047">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="11aab-2048">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="11aab-2048">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="11aab-2049">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="11aab-2049">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="11aab-2050">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="11aab-2050">Az.DataLakeStore</span></span>
* <span data-ttu-id="11aab-2051">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="11aab-2051">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="11aab-2052">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="11aab-2052">Az.EventHub</span></span>
* <span data-ttu-id="11aab-2053">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="11aab-2053">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="11aab-2054">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="11aab-2054">Az.KeyVault</span></span>
* <span data-ttu-id="11aab-2055">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="11aab-2055">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="11aab-2056">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="11aab-2056">Az.LogicApp</span></span>
* <span data-ttu-id="11aab-2057">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="11aab-2057">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="11aab-2058">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="11aab-2058">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="11aab-2059">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="11aab-2059">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="11aab-2060">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="11aab-2060">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="11aab-2061">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="11aab-2061">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="11aab-2062">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="11aab-2062">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="11aab-2063">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="11aab-2063">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="11aab-2064">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="11aab-2064">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="11aab-2065">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="11aab-2065">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="11aab-2066">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="11aab-2066">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="11aab-2067">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="11aab-2067">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="11aab-2068">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="11aab-2068">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="11aab-2069">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="11aab-2069">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="11aab-2070">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="11aab-2070">Az.Monitor</span></span>
* <span data-ttu-id="11aab-2071">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="11aab-2071">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-2072">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-2072">Az.Network</span></span>
* <span data-ttu-id="11aab-2073">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="11aab-2073">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="11aab-2074">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="11aab-2074">Az.OperationalInsights</span></span>
* <span data-ttu-id="11aab-2075">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="11aab-2075">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="11aab-2076">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="11aab-2076">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="11aab-2077">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="11aab-2077">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-2078">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-2078">Az.Resources</span></span>
* <span data-ttu-id="11aab-2079">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="11aab-2079">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="11aab-2080">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="11aab-2080">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="11aab-2081">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="11aab-2081">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="11aab-2082">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="11aab-2082">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-2083">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-2083">Az.Sql</span></span>
* <span data-ttu-id="11aab-2084">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="11aab-2084">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="11aab-2085">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="11aab-2085">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="11aab-2086">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="11aab-2086">Az.Websites</span></span>
* <span data-ttu-id="11aab-2087">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="11aab-2087">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="11aab-2088">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-2088">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="11aab-2089">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-2089">Az.Accounts</span></span>
* <span data-ttu-id="11aab-2090">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="11aab-2090">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="11aab-2091">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="11aab-2091">Az.AnalysisServices</span></span>
<span data-ttu-id="11aab-2092">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="11aab-2092">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-2093">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-2093">Az.Compute</span></span>
* <span data-ttu-id="11aab-2094">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="11aab-2094">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="11aab-2095">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="11aab-2095">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="11aab-2096">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="11aab-2096">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="11aab-2097">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="11aab-2097">Az.RecoveryServices</span></span>
<span data-ttu-id="11aab-2098">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="11aab-2098">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-2099">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-2099">Az.Resources</span></span>
* <span data-ttu-id="11aab-2100">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="11aab-2100">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="11aab-2101">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="11aab-2101">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="11aab-2102">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="11aab-2102">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="11aab-2103">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="11aab-2103">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-2104">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-2104">Az.Sql</span></span>
* <span data-ttu-id="11aab-2105">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="11aab-2105">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="11aab-2106">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="11aab-2106">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="11aab-2107">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="11aab-2107">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="11aab-2108">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-2108">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="11aab-2109">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-2109">Az.Accounts</span></span>
* <span data-ttu-id="11aab-2110">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="11aab-2110">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="11aab-2111">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="11aab-2111">Az.AnalysisServices</span></span>
* <span data-ttu-id="11aab-2112">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="11aab-2112">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="11aab-2113">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="11aab-2113">Az.RecoveryServices</span></span>
* <span data-ttu-id="11aab-2114">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="11aab-2114">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="11aab-2115">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-2115">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="11aab-2116">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-2116">Az.Accounts</span></span>
* <span data-ttu-id="11aab-2117">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="11aab-2117">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="11aab-2118">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="11aab-2118">Update incorrect online help URLs</span></span>
* <span data-ttu-id="11aab-2119">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="11aab-2119">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="11aab-2120">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="11aab-2120">Az.Aks</span></span>
* <span data-ttu-id="11aab-2121">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="11aab-2121">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="11aab-2122">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="11aab-2122">Az.Automation</span></span>
* <span data-ttu-id="11aab-2123">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="11aab-2123">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="11aab-2124">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="11aab-2124">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="11aab-2125">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="11aab-2125">Az.Cdn</span></span>
* <span data-ttu-id="11aab-2126">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="11aab-2126">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-2127">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-2127">Az.Compute</span></span>
* <span data-ttu-id="11aab-2128">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="11aab-2128">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="11aab-2129">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="11aab-2129">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="11aab-2130">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="11aab-2130">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="11aab-2131">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="11aab-2131">Az.ContainerRegistry</span></span>
* <span data-ttu-id="11aab-2132">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="11aab-2132">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="11aab-2133">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="11aab-2133">Az.DataFactory</span></span>
* <span data-ttu-id="11aab-2134">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="11aab-2134">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="11aab-2135">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="11aab-2135">Az.DataLakeStore</span></span>
* <span data-ttu-id="11aab-2136">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="11aab-2136">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="11aab-2137">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="11aab-2137">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="11aab-2138">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="11aab-2138">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="11aab-2139">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="11aab-2139">Az.IotHub</span></span>
* <span data-ttu-id="11aab-2140">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="11aab-2140">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="11aab-2141">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="11aab-2141">Az.KeyVault</span></span>
* <span data-ttu-id="11aab-2142">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="11aab-2142">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-2143">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-2143">Az.Network</span></span>
* <span data-ttu-id="11aab-2144">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="11aab-2144">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-2145">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-2145">Az.Resources</span></span>
* <span data-ttu-id="11aab-2146">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="11aab-2146">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="11aab-2147">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="11aab-2147">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="11aab-2148">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="11aab-2148">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="11aab-2149">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="11aab-2149">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="11aab-2150">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="11aab-2150">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="11aab-2151">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="11aab-2151">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="11aab-2152">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="11aab-2152">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="11aab-2153">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="11aab-2153">Az.ServiceFabric</span></span>
* <span data-ttu-id="11aab-2154">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="11aab-2154">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="11aab-2155">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="11aab-2155">Fix some error messages.</span></span>
* <span data-ttu-id="11aab-2156">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="11aab-2156">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="11aab-2157">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="11aab-2157">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="11aab-2158">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="11aab-2158">Az.SignalR</span></span>
* <span data-ttu-id="11aab-2159">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="11aab-2159">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-2160">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-2160">Az.Sql</span></span>
* <span data-ttu-id="11aab-2161">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="11aab-2161">Update incorrect online help URLs</span></span>
* <span data-ttu-id="11aab-2162">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="11aab-2162">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="11aab-2163">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="11aab-2163">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="11aab-2164">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="11aab-2164">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="11aab-2165">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-2165">Az.Storage</span></span>
* <span data-ttu-id="11aab-2166">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="11aab-2166">Update incorrect online help URLs</span></span>
* <span data-ttu-id="11aab-2167">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="11aab-2167">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="11aab-2168">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="11aab-2168">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="11aab-2169">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="11aab-2169">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="11aab-2170">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="11aab-2170">Az.TrafficManager</span></span>
* <span data-ttu-id="11aab-2171">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="11aab-2171">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="11aab-2172">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="11aab-2172">Az.Websites</span></span>
* <span data-ttu-id="11aab-2173">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="11aab-2173">Update incorrect online help URLs</span></span>
* <span data-ttu-id="11aab-2174">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="11aab-2174">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="11aab-2175">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="11aab-2175">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="11aab-2176">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="11aab-2176">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="11aab-2177">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-2177">Az.Accounts</span></span>
* <span data-ttu-id="11aab-2178">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="11aab-2178">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-2179">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-2179">Az.Compute</span></span>
* <span data-ttu-id="11aab-2180">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="11aab-2180">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="11aab-2181">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="11aab-2181">Updated the description of ID in help files</span></span>
* <span data-ttu-id="11aab-2182">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-2182">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="11aab-2183">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="11aab-2183">Az.DataLakeStore</span></span>
* <span data-ttu-id="11aab-2184">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="11aab-2184">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="11aab-2185">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="11aab-2185">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="11aab-2186">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="11aab-2186">Az.EventGrid</span></span>
* <span data-ttu-id="11aab-2187">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="11aab-2187">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="11aab-2188">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="11aab-2188">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="11aab-2189">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="11aab-2189">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="11aab-2190">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="11aab-2190">Event Time-To-Live,</span></span>
        - <span data-ttu-id="11aab-2191">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="11aab-2191">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="11aab-2192">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="11aab-2192">Dead letter endpoint.</span></span>
    - <span data-ttu-id="11aab-2193">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="11aab-2193">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="11aab-2194">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="11aab-2194">Event Time-To-Live,</span></span>
        - <span data-ttu-id="11aab-2195">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="11aab-2195">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="11aab-2196">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="11aab-2196">Dead letter endpoint.</span></span>
* <span data-ttu-id="11aab-2197">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="11aab-2197">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="11aab-2198">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="11aab-2198">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="11aab-2199">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="11aab-2199">Az.IotHub</span></span>
* <span data-ttu-id="11aab-2200">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="11aab-2200">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="11aab-2201">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="11aab-2201">Az.LogicApp</span></span>
* <span data-ttu-id="11aab-2202">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="11aab-2202">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-2203">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-2203">Az.Resources</span></span>
* <span data-ttu-id="11aab-2204">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="11aab-2204">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="11aab-2205">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="11aab-2205">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="11aab-2206">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="11aab-2206">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="11aab-2207">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="11aab-2207">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="11aab-2208">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="11aab-2208">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="11aab-2209">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="11aab-2209">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="11aab-2210">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="11aab-2210">Az.SignalR</span></span>
* <span data-ttu-id="11aab-2211">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-2211">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-2212">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-2212">Az.Sql</span></span>
* <span data-ttu-id="11aab-2213">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="11aab-2213">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="11aab-2214">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-2214">Az.Storage</span></span>
* <span data-ttu-id="11aab-2215">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="11aab-2215">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="11aab-2216">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="11aab-2216">New-AzStorageContext</span></span>
* <span data-ttu-id="11aab-2217">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="11aab-2217">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="11aab-2218">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="11aab-2218">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="11aab-2219">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="11aab-2219">Az.Websites</span></span>
* <span data-ttu-id="11aab-2220">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="11aab-2220">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="11aab-2221">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-2221">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="11aab-2222">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="11aab-2222">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="11aab-2223">Geral</span><span class="sxs-lookup"><span data-stu-id="11aab-2223">General</span></span>

- <span data-ttu-id="11aab-2224">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="11aab-2224">General Availability of Az Module</span></span>
- <span data-ttu-id="11aab-2225">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="11aab-2225">Online help for each module</span></span>
- <span data-ttu-id="11aab-2226">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="11aab-2226">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="11aab-2227">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="11aab-2227">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="11aab-2228">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-2228">Az.Accounts</span></span>
- <span data-ttu-id="11aab-2229">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="11aab-2229">Changed from Az.Profile</span></span>
- <span data-ttu-id="11aab-2230">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="11aab-2230">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="11aab-2231">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="11aab-2231">Az.ApiManagement</span></span>
- <span data-ttu-id="11aab-2232">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="11aab-2232">Fixes for #7002</span></span>
- <span data-ttu-id="11aab-2233">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="11aab-2233">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="11aab-2234">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="11aab-2234">Az.Batch</span></span>
- <span data-ttu-id="11aab-2235">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="11aab-2235">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="11aab-2236">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="11aab-2236">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="11aab-2237">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="11aab-2237">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="11aab-2238">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="11aab-2238">Az.Billing</span></span>
- <span data-ttu-id="11aab-2239">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="11aab-2239">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="11aab-2240">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="11aab-2240">Az.CognitivServices</span></span>
- <span data-ttu-id="11aab-2241">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="11aab-2241">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="11aab-2242">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="11aab-2242">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="11aab-2243">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="11aab-2243">Az.ContainerInstance</span></span>
- <span data-ttu-id="11aab-2244">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="11aab-2244">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="11aab-2245">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="11aab-2245">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="11aab-2246">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="11aab-2246">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="11aab-2247">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="11aab-2247">Az.DataLakeStore</span></span>
- <span data-ttu-id="11aab-2248">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="11aab-2248">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="11aab-2249">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="11aab-2249">Az.Monitor</span></span>
- <span data-ttu-id="11aab-2250">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="11aab-2250">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="11aab-2251">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="11aab-2251">Az.KeyVault</span></span>
- <span data-ttu-id="11aab-2252">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="11aab-2252">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="11aab-2253">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="11aab-2253">Az.MachineLearning</span></span>
- <span data-ttu-id="11aab-2254">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="11aab-2254">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="11aab-2255">Az.Media</span><span class="sxs-lookup"><span data-stu-id="11aab-2255">Az.Media</span></span>
- <span data-ttu-id="11aab-2256">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="11aab-2256">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="11aab-2257">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-2257">Az.Network</span></span>
<span data-ttu-id="11aab-2258">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="11aab-2258">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="11aab-2259">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="11aab-2259">New cmdlets added:</span></span>
        - <span data-ttu-id="11aab-2260">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="11aab-2260">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="11aab-2261">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="11aab-2261">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="11aab-2262">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="11aab-2262">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="11aab-2263">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="11aab-2263">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="11aab-2264">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="11aab-2264">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="11aab-2265">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="11aab-2265">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="11aab-2266">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="11aab-2266">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="11aab-2267">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="11aab-2267">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="11aab-2268">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="11aab-2268">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="11aab-2269">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="11aab-2269">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="11aab-2270">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="11aab-2270">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="11aab-2271">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="11aab-2271">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="11aab-2272">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-2272">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="11aab-2273">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-2273">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="11aab-2274">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="11aab-2274">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="11aab-2275">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="11aab-2275">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="11aab-2276">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="11aab-2276">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="11aab-2277">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="11aab-2277">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="11aab-2278">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="11aab-2278">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="11aab-2279">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="11aab-2279">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="11aab-2280">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="11aab-2280">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="11aab-2281">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="11aab-2281">Az.OperationalInsights</span></span>
- <span data-ttu-id="11aab-2282">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="11aab-2282">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="11aab-2283">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="11aab-2283">Az.Profile</span></span>
- <span data-ttu-id="11aab-2284">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="11aab-2284">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="11aab-2285">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="11aab-2285">Az.RecoveryServices</span></span>
- <span data-ttu-id="11aab-2286">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="11aab-2286">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="11aab-2287">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-2287">Az.Resources</span></span>
- <span data-ttu-id="11aab-2288">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="11aab-2288">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="11aab-2289">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="11aab-2289">Az.ServiceFabric</span></span>
- <span data-ttu-id="11aab-2290">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="11aab-2290">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="11aab-2291">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="11aab-2291">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="11aab-2292">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="11aab-2292">Az.SIgnalR</span></span>
- <span data-ttu-id="11aab-2293">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="11aab-2293">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="11aab-2294">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-2294">Az.Sql</span></span>
- <span data-ttu-id="11aab-2295">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="11aab-2295">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="11aab-2296">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="11aab-2296">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="11aab-2297">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="11aab-2297">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="11aab-2298">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-2298">Az.Storage</span></span>
- <span data-ttu-id="11aab-2299">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="11aab-2299">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="11aab-2300">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="11aab-2300">Az.Websites</span></span>
- <span data-ttu-id="11aab-2301">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="11aab-2301">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="11aab-2302">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="11aab-2302">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="11aab-2303">Geral</span><span class="sxs-lookup"><span data-stu-id="11aab-2303">General</span></span>

* <span data-ttu-id="11aab-2304">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="11aab-2304">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="11aab-2305">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-2305">Az.Compute</span></span>

* <span data-ttu-id="11aab-2306">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="11aab-2306">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="11aab-2307">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="11aab-2307">Az.DataLakeStore</span></span>

* <span data-ttu-id="11aab-2308">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="11aab-2308">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="11aab-2309">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="11aab-2309">Az.FrontDoor</span></span>

* <span data-ttu-id="11aab-2310">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="11aab-2310">Fixed some broken links</span></span>
    - <span data-ttu-id="11aab-2311">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="11aab-2311">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="11aab-2312">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="11aab-2312">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="11aab-2313">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="11aab-2313">Az.RecoveryServices</span></span>

* <span data-ttu-id="11aab-2314">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-2314">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="11aab-2315">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="11aab-2315">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="11aab-2316">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-2316">Az.Resources</span></span>

* <span data-ttu-id="11aab-2317">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="11aab-2317">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="11aab-2318">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="11aab-2318">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="11aab-2319">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-2319">Az.Sql</span></span>

* <span data-ttu-id="11aab-2320">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="11aab-2320">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="11aab-2321">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="11aab-2321">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="11aab-2322">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="11aab-2322">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="11aab-2323">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-2323">Az.Storage</span></span>

* <span data-ttu-id="11aab-2324">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="11aab-2324">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="11aab-2325">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="11aab-2325">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="11aab-2326">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="11aab-2326">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="11aab-2327">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="11aab-2327">Support Static Website configuration</span></span>
    - <span data-ttu-id="11aab-2328">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="11aab-2328">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="11aab-2329">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="11aab-2329">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="11aab-2330">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="11aab-2330">Az.Websites</span></span>

* <span data-ttu-id="11aab-2331">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="11aab-2331">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="11aab-2332">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="11aab-2332">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="11aab-2333">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-2333">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="11aab-2334">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="11aab-2334">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="11aab-2335">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="11aab-2335">Az.ApiManagement</span></span>
* <span data-ttu-id="11aab-2336">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="11aab-2336">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="11aab-2337">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="11aab-2337">Az.Automation</span></span>
* <span data-ttu-id="11aab-2338">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="11aab-2338">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="11aab-2339">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="11aab-2339">Added Update Management cmdlets</span></span>
* <span data-ttu-id="11aab-2340">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="11aab-2340">Added Source Control cmdlets</span></span>
* <span data-ttu-id="11aab-2341">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="11aab-2341">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="11aab-2342">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="11aab-2342">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="11aab-2343">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-2343">Az.Compute</span></span>
* <span data-ttu-id="11aab-2344">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="11aab-2344">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="11aab-2345">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="11aab-2345">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="11aab-2346">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="11aab-2346">Az.ContainerInstance</span></span>
* <span data-ttu-id="11aab-2347">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="11aab-2347">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="11aab-2348">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="11aab-2348">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="11aab-2349">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="11aab-2349">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="11aab-2350">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-2350">Az.Network</span></span>
* <span data-ttu-id="11aab-2351">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="11aab-2351">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="11aab-2352">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="11aab-2352">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="11aab-2353">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="11aab-2353">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="11aab-2354">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="11aab-2354">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="11aab-2355">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="11aab-2355">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="11aab-2356">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="11aab-2356">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="11aab-2357">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="11aab-2357">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="11aab-2358">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="11aab-2358">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="11aab-2359">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="11aab-2359">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="11aab-2360">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="11aab-2360">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="11aab-2361">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="11aab-2361">Az.Relay</span></span>
* <span data-ttu-id="11aab-2362">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="11aab-2362">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="11aab-2363">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-2363">Az.Resources</span></span>
* <span data-ttu-id="11aab-2364">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="11aab-2364">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="11aab-2365">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="11aab-2365">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="11aab-2366">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="11aab-2366">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="11aab-2367">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="11aab-2367">Az.ServiceFabric</span></span>
* <span data-ttu-id="11aab-2368">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="11aab-2368">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="11aab-2369">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-2369">Az.Sql</span></span>
* <span data-ttu-id="11aab-2370">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="11aab-2370">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="11aab-2371">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="11aab-2371">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="11aab-2372">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="11aab-2372">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="11aab-2373">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="11aab-2373">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="11aab-2374">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="11aab-2374">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="11aab-2375">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="11aab-2375">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="11aab-2376">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="11aab-2376">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="11aab-2377">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="11aab-2377">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="11aab-2378">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="11aab-2378">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="11aab-2379">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="11aab-2379">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="11aab-2380">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="11aab-2380">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="11aab-2381">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="11aab-2381">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="11aab-2382">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="11aab-2382">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="11aab-2383">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="11aab-2383">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="11aab-2384">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="11aab-2384">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="11aab-2385">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="11aab-2385">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="11aab-2386">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="11aab-2386">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="11aab-2387">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="11aab-2387">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="11aab-2388">Geral</span><span class="sxs-lookup"><span data-stu-id="11aab-2388">General</span></span>
* <span data-ttu-id="11aab-2389">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="11aab-2389">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="11aab-2390">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="11aab-2390">Az.Profile</span></span>
* <span data-ttu-id="11aab-2391">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="11aab-2391">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="11aab-2392">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="11aab-2392">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="11aab-2393">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="11aab-2393">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="11aab-2394">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="11aab-2394">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="11aab-2395">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="11aab-2395">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="11aab-2396">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="11aab-2396">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="11aab-2397">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="11aab-2397">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="11aab-2398">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="11aab-2398">Az.CognitiveServices</span></span>
* <span data-ttu-id="11aab-2399">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="11aab-2399">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-2400">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-2400">Az.Compute</span></span>
* <span data-ttu-id="11aab-2401">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="11aab-2401">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="11aab-2402">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="11aab-2402">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="11aab-2403">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="11aab-2403">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="11aab-2404">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="11aab-2404">Az.DataLakeStore</span></span>
* <span data-ttu-id="11aab-2405">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="11aab-2405">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="11aab-2406">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="11aab-2406">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="11aab-2407">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="11aab-2407">Az.Insights</span></span>
* <span data-ttu-id="11aab-2408">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="11aab-2408">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="11aab-2409">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="11aab-2409">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="11aab-2410">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="11aab-2410">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="11aab-2411">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="11aab-2411">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-2412">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-2412">Az.Network</span></span>
* <span data-ttu-id="11aab-2413">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="11aab-2413">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="11aab-2414">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="11aab-2414">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="11aab-2415">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="11aab-2415">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="11aab-2416">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="11aab-2416">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="11aab-2417">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="11aab-2417">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="11aab-2418">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="11aab-2418">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="11aab-2419">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="11aab-2419">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="11aab-2420">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="11aab-2420">Az.PolicyInsights</span></span>
* <span data-ttu-id="11aab-2421">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="11aab-2421">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-2422">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-2422">Az.Resources</span></span>
* <span data-ttu-id="11aab-2423">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="11aab-2423">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="11aab-2424">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="11aab-2424">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="11aab-2425">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="11aab-2425">Az.ServiceBus</span></span>
* <span data-ttu-id="11aab-2426">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="11aab-2426">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="11aab-2427">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="11aab-2427">Az.ServiceFabric</span></span>
* <span data-ttu-id="11aab-2428">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="11aab-2428">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="11aab-2429">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="11aab-2429">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="11aab-2430">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="11aab-2430">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="11aab-2431">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="11aab-2431">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="11aab-2432">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="11aab-2432">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="11aab-2433">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="11aab-2433">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="11aab-2434">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="11aab-2434">Az.Profile</span></span>
* <span data-ttu-id="11aab-2435">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="11aab-2435">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="11aab-2436">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="11aab-2436">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-2437">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-2437">Az.Compute</span></span>
* <span data-ttu-id="11aab-2438">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="11aab-2438">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="11aab-2439">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="11aab-2439">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="11aab-2440">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="11aab-2440">Az.DataLakeStore</span></span>
* <span data-ttu-id="11aab-2441">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="11aab-2441">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="11aab-2442">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-2442">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="11aab-2443">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="11aab-2443">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="11aab-2444">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="11aab-2444">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="11aab-2445">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="11aab-2445">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-2446">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-2446">Az.Network</span></span>
* <span data-ttu-id="11aab-2447">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="11aab-2447">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="11aab-2448">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="11aab-2448">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-2449">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-2449">Az.Resources</span></span>
* <span data-ttu-id="11aab-2450">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="11aab-2450">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="11aab-2451">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="11aab-2451">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="11aab-2452">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="11aab-2452">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="11aab-2453">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="11aab-2453">Azure.Storage</span></span>
* <span data-ttu-id="11aab-2454">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="11aab-2454">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="11aab-2455">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="11aab-2455">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="11aab-2456">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="11aab-2456">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="11aab-2457">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="11aab-2457">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="11aab-2458">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="11aab-2458">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="11aab-2459">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="11aab-2459">Az.CognitiveServices</span></span>
* <span data-ttu-id="11aab-2460">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="11aab-2460">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="11aab-2461">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="11aab-2461">Az.Compute</span></span>
* <span data-ttu-id="11aab-2462">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="11aab-2462">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="11aab-2463">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="11aab-2463">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="11aab-2464">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="11aab-2464">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="11aab-2465">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="11aab-2465">Az.DataFactoryV2</span></span>
* <span data-ttu-id="11aab-2466">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="11aab-2466">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="11aab-2467">Az.Network</span><span class="sxs-lookup"><span data-stu-id="11aab-2467">Az.Network</span></span>
* <span data-ttu-id="11aab-2468">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="11aab-2468">Added NetworkProfile functionality.</span></span> <span data-ttu-id="11aab-2469">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="11aab-2469">new cmdlets added</span></span>
    - <span data-ttu-id="11aab-2470">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="11aab-2470">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="11aab-2471">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="11aab-2471">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="11aab-2472">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="11aab-2472">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="11aab-2473">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="11aab-2473">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="11aab-2474">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-2474">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="11aab-2475">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-2475">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="11aab-2476">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="11aab-2476">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="11aab-2477">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="11aab-2477">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="11aab-2478">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="11aab-2478">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="11aab-2479">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="11aab-2479">Az.RedisCache</span></span>
* <span data-ttu-id="11aab-2480">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="11aab-2480">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="11aab-2481">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="11aab-2481">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="11aab-2482">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="11aab-2482">Az.Resources</span></span>
* <span data-ttu-id="11aab-2483">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="11aab-2483">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="11aab-2484">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="11aab-2484">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="11aab-2485">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="11aab-2485">Az.Sql</span></span>
* <span data-ttu-id="11aab-2486">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="11aab-2486">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="11aab-2487">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="11aab-2487">Az.Websites</span></span>
* <span data-ttu-id="11aab-2488">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="11aab-2488">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="11aab-2489">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="11aab-2489">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="11aab-2490">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="11aab-2490">0.2.0 - September 2018</span></span>
 <span data-ttu-id="11aab-2491">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="11aab-2491">Initial Release</span></span>
